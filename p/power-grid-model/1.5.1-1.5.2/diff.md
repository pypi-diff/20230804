# Comparing `tmp/power-grid-model-1.5.1.tar.gz` & `tmp/power-grid-model-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.1.tar", last modified: Thu Aug  3 09:14:54 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.2.tar", last modified: Thu Aug  3 14:42:39 2023, max compression
```

## Comparing `power-grid-model-1.5.1.tar` & `power-grid-model-1.5.2.tar`

### file list

```diff
@@ -1,593 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 09:14:08.000000 power-grid-model-1.5.1/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.174337 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.182336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.182336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.182336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    61599 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24917 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    56026 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.186336 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    94102 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.174337 power-grid-model-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-03 09:14:54.000000 power-grid-model-1.5.1/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-08-03 09:14:54.000000 power-grid-model-1.5.1/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:14:54.000000 power-grid-model-1.5.1/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 09:14:54.000000 power-grid-model-1.5.1/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 09:14:54.000000 power-grid-model-1.5.1/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.190336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.194336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.194336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.194336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.198336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.198336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.202336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.206336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.206336 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.210336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.214336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.214336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.214336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.214336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.214336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.218336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.218336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.218336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.218336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.218336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.222336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.222336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.226336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.226336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.226336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.230336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.230336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.230336 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.234336 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.234336 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.234336 power-grid-model-1.5.1/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.238336 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.238336 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   255637 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.238336 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    62578 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.242336 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   250520 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.242336 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   255901 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.178336 power-grid-model-1.5.1/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.242336 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.242336 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.246336 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:14:54.250336 power-grid-model-1.5.1/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-08-03 09:14:05.000000 power-grid-model-1.5.1/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.332875 power-grid-model-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-03 14:42:39.332875 power-grid-model-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 14:42:00.000000 power-grid-model-1.5.2/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.264875 power-grid-model-1.5.2/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.264875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.256875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.264875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.268875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.268875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.268875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.268875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    61284 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41156 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30676 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56026 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    94102 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:42:39.332875 power-grid-model-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.256875 power-grid-model-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.272875 power-grid-model-1.5.2/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.276875 power-grid-model-1.5.2/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.276875 power-grid-model-1.5.2/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.276875 power-grid-model-1.5.2/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-03 14:42:39.000000 power-grid-model-1.5.2/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-08-03 14:42:39.000000 power-grid-model-1.5.2/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:42:39.000000 power-grid-model-1.5.2/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-03 14:42:39.000000 power-grid-model-1.5.2/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 14:42:39.000000 power-grid-model-1.5.2/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.264875 power-grid-model-1.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.276875 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.280875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.280875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.280875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.284875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.284875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.284875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.288875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.288875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.288875 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.288875 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.288875 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.292875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.292875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.292875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.292875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.296875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.296875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.296875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.296875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.300875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.300875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.300875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.300875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.300875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.304875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.304875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.304875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.304875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.308875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.308875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.308875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.308875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.312875 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.312875 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.312875 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.312875 power-grid-model-1.5.2/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.316875 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.260875 power-grid-model-1.5.2/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.316875 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   255637 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.316875 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    62578 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.320875 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   250520 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.320875 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   255901 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.264875 power-grid-model-1.5.2/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.320875 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.324875 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.324875 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.324875 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.324875 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.324875 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.328875 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.328875 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.328875 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.328875 power-grid-model-1.5.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:39.332875 power-grid-model-1.5.2/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-08-03 14:41:57.000000 power-grid-model-1.5.2/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.1/LICENSE` & `power-grid-model-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/PKG-INFO` & `power-grid-model-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.1/README.md` & `power-grid-model-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -25,10 +25,10 @@
 
 namespace power_grid_model {
 
 using AllComponents =
     ComponentList<Node, Line, Link, Transformer, ThreeWindingTransformer, Shunt, Source, SymGenerator, AsymGenerator,
                   SymLoad, AsymLoad, SymPowerSensor, AsymPowerSensor, SymVoltageSensor, AsymVoltageSensor, Fault>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
-#endif  // POWER_GRID_MODEL_ALL_COMPONENTS_HPP
+#endif // POWER_GRID_MODEL_ALL_COMPONENTS_HPP
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,100 +20,89 @@
 // the dataset can also be a batch of sets with different length per batch
 //     the indptr is an integer array, for i-th sets,
 //          the set data is in the range [ indptr[i], indptr[i + 1] )
 // the dataset can also be a batch of sets with the same length per batch
 //     the indptr is a nullptr, for i-th sets,
 //          the set data is in the range [ i * elements_per_scenario, (i + 1) * elements_per_scenario )
 
-template <bool is_const>
-class DataPointer {
-    template <class T>
-    using ptr_t = std::conditional_t<is_const, T const*, T*>;
+template <bool is_const> class DataPointer {
+    template <class T> using ptr_t = std::conditional_t<is_const, T const*, T*>;
 
-   public:
-    DataPointer() : ptr_{nullptr}, indptr_{nullptr}, batch_size_{}, elements_per_scenario_{} {
-    }
+  public:
+    DataPointer() : ptr_{nullptr}, indptr_{nullptr}, batch_size_{}, elements_per_scenario_{} {}
 
     // single batch dataset
     DataPointer(ptr_t<void> ptr, Idx single_length)
-        : ptr_{ptr}, indptr_{nullptr}, batch_size_{1}, elements_per_scenario_{single_length} {
-    }
+        : ptr_{ptr}, indptr_{nullptr}, batch_size_{1}, elements_per_scenario_{single_length} {}
 
     // fix batch length
     DataPointer(ptr_t<void> ptr, Idx batch_size, Idx elements_per_scenario)
-        : ptr_{ptr}, indptr_{nullptr}, batch_size_{batch_size}, elements_per_scenario_{elements_per_scenario} {
-    }
+        : ptr_{ptr}, indptr_{nullptr}, batch_size_{batch_size}, elements_per_scenario_{elements_per_scenario} {}
 
     // variable batches
     DataPointer(ptr_t<void> ptr, Idx const* indptr, Idx batch_size)
-        : ptr_{ptr}, indptr_{indptr}, batch_size_{batch_size}, elements_per_scenario_{-1} {
-    }
+        : ptr_{ptr}, indptr_{indptr}, batch_size_{batch_size}, elements_per_scenario_{-1} {}
 
     // copy to const constructor
     DataPointer(ptr_t<void> ptr, Idx const* indptr, Idx batch_size, Idx elements_per_scenario)
-        : ptr_{ptr}, indptr_{indptr}, batch_size_{batch_size}, elements_per_scenario_{elements_per_scenario} {
-    }
+        : ptr_{ptr}, indptr_{indptr}, batch_size_{batch_size}, elements_per_scenario_{elements_per_scenario} {}
 
-    template <class T>
-    std::pair<ptr_t<T>, ptr_t<T>> get_iterators(Idx pos) const {
+    template <class T> std::pair<ptr_t<T>, ptr_t<T>> get_iterators(Idx pos) const {
         assert(pos < batch_size_);
         ptr_t<T> const ptr = reinterpret_cast<ptr_t<T>>(ptr_);
         if (indptr_) {
             if (pos < 0) {
                 return std::make_pair(ptr, ptr + indptr_[batch_size_]);
             }
             return std::make_pair(ptr + indptr_[pos], ptr + indptr_[pos + 1]);
         }
         if (pos < 0) {
             return std::make_pair(ptr, ptr + elements_per_scenario_ * batch_size_);
         }
         return std::make_pair(ptr + elements_per_scenario_ * pos, ptr + elements_per_scenario_ * (pos + 1));
     }
 
-    Idx batch_size() const {
-        return (Idx)batch_size_;
-    }
+    Idx batch_size() const { return (Idx)batch_size_; }
 
     Idx elements_per_scenario(Idx pos) const {
         assert(pos >= 0);
         assert(pos < batch_size_);
         if (indptr_) {
             return indptr_[pos + 1] - indptr_[pos];
         }
         return (Idx)elements_per_scenario_;
     }
 
-    ptr_t<void> raw_ptr() const {
-        return ptr_;
-    }
+    ptr_t<void> raw_ptr() const { return ptr_; }
 
     // check if the dataset is one empty batch
     // the length of data should be zero
     bool is_empty() const {
         if (indptr_) {
             return (indptr_[batch_size_] == 0);
         }
         return batch_size_ == 0 || elements_per_scenario_ == 0;
     }
 
     // conversion to const iterator
     template <class UX = DataPointer<true>>
-    requires(!is_const) explicit operator UX() const {
+        requires(!is_const)
+    explicit operator UX() const {
         return DataPointer<true>{ptr_, indptr_, batch_size_, elements_per_scenario_};
     }
 
-   private:
+  private:
     ptr_t<void> ptr_;
     Idx const* indptr_;
-    Idx batch_size_;             // number of batches
-    Idx elements_per_scenario_;  // number of data points per batch, -1 for variable batches
+    Idx batch_size_;            // number of batches
+    Idx elements_per_scenario_; // number of data points per batch, -1 for variable batches
 };
 
 using MutableDataPointer = DataPointer<false>;
 using ConstDataPointer = DataPointer<true>;
 
 using Dataset = std::map<std::string, MutableDataPointer>;
 using ConstDataset = std::map<std::string, ConstDataPointer>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -13,84 +13,63 @@
 
 #include <bit>
 #include <string>
 
 namespace power_grid_model::meta_data {
 
 // pointer to member
-template <class T>
-struct trait_pointer_to_member;
-template <class StructType, class ValueType>
-struct trait_pointer_to_member<ValueType StructType::*> {
+template <class T> struct trait_pointer_to_member;
+template <class StructType, class ValueType> struct trait_pointer_to_member<ValueType StructType::*> {
     using value_type = ValueType;
 };
-template <class StructType, auto member_ptr>
-inline size_t get_offset() {
+template <class StructType, auto member_ptr> inline size_t get_offset() {
     StructType const obj{};
     return (size_t)(&(obj.*member_ptr)) - (size_t)&obj;
 }
 
 // empty template functor classes to generate attributes list
-template <class T>
-struct get_attributes_list;
-template <class T>
-struct get_component_nan;
+template <class T> struct get_attributes_list;
+template <class T> struct get_component_nan;
 
 // ctype string
-template <class T>
-struct ctype_t;
-template <>
-struct ctype_t<double> {
+template <class T> struct ctype_t;
+template <> struct ctype_t<double> {
     static constexpr CType value = CType::c_double;
 };
-template <>
-struct ctype_t<int32_t> {
+template <> struct ctype_t<int32_t> {
     static constexpr CType value = CType::c_int32;
 };
-template <>
-struct ctype_t<int8_t> {
+template <> struct ctype_t<int8_t> {
     static constexpr CType value = CType::c_int8;
 };
 
-template <>
-struct ctype_t<RealValue<false>> {
+template <> struct ctype_t<RealValue<false>> {
     static constexpr CType value = CType::c_double3;
 };
 template <class T>
-requires std::is_enum_v<T>
-struct ctype_t<T> : ctype_t<std::underlying_type_t<T>> {
-};
-template <class T>
-constexpr CType ctype_v = ctype_t<T>::value;
+    requires std::is_enum_v<T>
+struct ctype_t<T> : ctype_t<std::underlying_type_t<T>> {};
+template <class T> constexpr CType ctype_v = ctype_t<T>::value;
 
 // set nan
-inline void set_nan(double& x) {
-    x = nan;
-}
-inline void set_nan(IntS& x) {
-    x = na_IntS;
-}
-inline void set_nan(ID& x) {
-    x = na_IntID;
-}
-inline void set_nan(RealValue<false>& x) {
-    x = RealValue<false>{nan};
-}
+inline void set_nan(double& x) { x = nan; }
+inline void set_nan(IntS& x) { x = na_IntS; }
+inline void set_nan(ID& x) { x = na_IntID; }
+inline void set_nan(RealValue<false>& x) { x = RealValue<false>{nan}; }
 template <class Enum>
-requires std::same_as<std::underlying_type_t<Enum>, IntS>
+    requires std::same_as<std::underlying_type_t<Enum>, IntS>
 inline void set_nan(Enum& x) {
     x = static_cast<Enum>(na_IntS);
 }
 
-using RawDataPtr = void*;             // raw mutable data ptr
-using RawDataConstPtr = void const*;  // raw read-only data ptr
+using RawDataPtr = void*;            // raw mutable data ptr
+using RawDataConstPtr = void const*; // raw read-only data ptr
 
 // meta attribute
-template <class StructType, auto member_ptr>
-struct MetaAttributeImpl {
+template <class StructType, auto member_ptr> struct MetaAttributeImpl {
     using ValueType = typename trait_pointer_to_member<decltype(member_ptr)>::value_type;
     static bool check_nan(RawDataConstPtr buffer_ptr, Idx pos) {
         return is_nan((reinterpret_cast<StructType const*>(buffer_ptr) + pos)->*member_ptr);
     }
     static void set_value(RawDataPtr buffer_ptr, RawDataConstPtr value_ptr, Idx pos) {
         (reinterpret_cast<StructType*>(buffer_ptr) + pos)->*member_ptr = *reinterpret_cast<ValueType const*>(value_ptr);
     }
@@ -98,52 +77,47 @@
         *reinterpret_cast<ValueType*>(value_ptr) = (reinterpret_cast<StructType const*>(buffer_ptr) + pos)->*member_ptr;
     }
     static bool compare_value(RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol, double rtol, Idx pos) {
         ValueType const& x = (reinterpret_cast<StructType const*>(ptr_x) + pos)->*member_ptr;
         ValueType const& y = (reinterpret_cast<StructType const*>(ptr_y) + pos)->*member_ptr;
         if constexpr (std::same_as<ValueType, double>) {
             return std::abs(y - x) < (std::abs(x) * rtol + atol);
-        }
-        else if constexpr (std::same_as<ValueType, RealValue<false>>) {
+        } else if constexpr (std::same_as<ValueType, RealValue<false>>) {
             return (abs(y - x) < (abs(x) * rtol + atol)).all();
-        }
-        else {
+        } else {
             return x == y;
         }
     }
 };
 
-}  // namespace power_grid_model::meta_data
+} // namespace power_grid_model::meta_data
 
 // attribute in global namespace
 struct PGM_MetaAttribute {
     using Idx = power_grid_model::Idx;
     using CType = power_grid_model::CType;
-    template <class T>
-    using trait_pointer_to_member = power_grid_model::meta_data::trait_pointer_to_member<T>;
+    template <class T> using trait_pointer_to_member = power_grid_model::meta_data::trait_pointer_to_member<T>;
     template <class StructType, auto member_ptr>
     using MetaAttributeImpl = power_grid_model::meta_data::MetaAttributeImpl<StructType, member_ptr>;
     using RawDataConstPtr = power_grid_model::meta_data::RawDataConstPtr;
     using RawDataPtr = power_grid_model::meta_data::RawDataPtr;
-    template <class T>
-    static constexpr CType ctype_v = power_grid_model::meta_data::ctype_v<T>;
+    template <class T> static constexpr CType ctype_v = power_grid_model::meta_data::ctype_v<T>;
 
     template <class StructType, auto member_ptr,
               class ValueType = typename trait_pointer_to_member<decltype(member_ptr)>::value_type>
     PGM_MetaAttribute(MetaAttributeImpl<StructType, member_ptr>, std::string const& attr_name)
         : name{attr_name},
           ctype{ctype_v<ValueType>},
           offset{power_grid_model::meta_data::get_offset<StructType, member_ptr>()},
           size{sizeof(ValueType)},
           component_size{sizeof(StructType)},
           check_nan{MetaAttributeImpl<StructType, member_ptr>::check_nan},
           set_value{MetaAttributeImpl<StructType, member_ptr>::set_value},
           get_value{MetaAttributeImpl<StructType, member_ptr>::get_value},
-          compare_value{MetaAttributeImpl<StructType, member_ptr>::compare_value} {
-    }
+          compare_value{MetaAttributeImpl<StructType, member_ptr>::compare_value} {}
 
     // meta data
     std::string name;
     CType ctype{};
     size_t offset{};
     size_t size{};
     size_t component_size{};
@@ -157,65 +131,56 @@
 
 namespace power_grid_model::meta_data {
 
 // include inside meta data namespace
 using MetaAttribute = PGM_MetaAttribute;
 
 // meta component
-template <class StructType>
-struct MetaComponentImpl {
-    static RawDataPtr create_buffer(Idx size) {
-        return new StructType[size];
-    }
-    static void destroy_buffer(RawDataConstPtr buffer_ptr) {
-        delete[] reinterpret_cast<StructType const*>(buffer_ptr);
-    }
+template <class StructType> struct MetaComponentImpl {
+    static RawDataPtr create_buffer(Idx size) { return new StructType[size]; }
+    static void destroy_buffer(RawDataConstPtr buffer_ptr) { delete[] reinterpret_cast<StructType const*>(buffer_ptr); }
     static void set_nan(RawDataPtr buffer_ptr, Idx pos, Idx size) {
         static StructType const nan_value = get_component_nan<StructType>{}();
         StructType* ptr = reinterpret_cast<StructType*>(buffer_ptr);
         std::fill(ptr + pos, ptr + pos + size, nan_value);
     }
 };
 
-}  // namespace power_grid_model::meta_data
+} // namespace power_grid_model::meta_data
 
 // component in global name space
 struct PGM_MetaComponent {
-    template <class StructType>
-    using MetaComponentImpl = power_grid_model::meta_data::MetaComponentImpl<StructType>;
+    template <class StructType> using MetaComponentImpl = power_grid_model::meta_data::MetaComponentImpl<StructType>;
     using MetaAttribute = power_grid_model::meta_data::MetaAttribute;
     using Idx = power_grid_model::Idx;
     using RawDataConstPtr = power_grid_model::meta_data::RawDataConstPtr;
     using RawDataPtr = power_grid_model::meta_data::RawDataPtr;
 
     template <class StructType>
     PGM_MetaComponent(MetaComponentImpl<StructType>, std::string const& comp_name)
         : name{comp_name},
           size{sizeof(StructType)},
           alignment{alignof(StructType)},
           attributes{power_grid_model::meta_data::get_attributes_list<StructType>{}()},
           set_nan{MetaComponentImpl<StructType>::set_nan},
           create_buffer{MetaComponentImpl<StructType>::create_buffer},
-          destroy_buffer{MetaComponentImpl<StructType>::destroy_buffer} {
-    }
+          destroy_buffer{MetaComponentImpl<StructType>::destroy_buffer} {}
 
     // meta data
     std::string name;
     size_t size;
     size_t alignment;
     std::vector<MetaAttribute> attributes;
 
     // function pointers
     std::add_pointer_t<void(RawDataPtr, Idx, Idx)> set_nan;
     std::add_pointer_t<RawDataPtr(Idx)> create_buffer;
     std::add_pointer_t<void(RawDataConstPtr)> destroy_buffer;
 
-    Idx n_attributes() const {
-        return static_cast<Idx>(attributes.size());
-    }
+    Idx n_attributes() const { return static_cast<Idx>(attributes.size()); }
 
     MetaAttribute const& get_attribute(std::string const& attribute_name) const {
         Idx const found = find_attribute(attribute_name);
         if (found < 0) {
             throw std::out_of_range{"Cannot find attribute with name: " + attribute_name + "!\n"};
         }
         return attributes[found];
@@ -226,36 +191,32 @@
             if (attributes[i].name == attribute_name) {
                 return i;
             }
         }
         return -1;
     }
 
-    Idx has_attribute(std::string const& attribute_name) const {
-        return find_attribute(attribute_name) >= 0;
-    }
+    Idx has_attribute(std::string const& attribute_name) const { return find_attribute(attribute_name) >= 0; }
 };
 
 namespace power_grid_model::meta_data {
 
 using MetaComponent = PGM_MetaComponent;
 
-}  // namespace power_grid_model::meta_data
+} // namespace power_grid_model::meta_data
 
 // meta dataset in global namespace
 struct PGM_MetaDataset {
     using MetaComponent = power_grid_model::meta_data::MetaComponent;
     using Idx = power_grid_model::Idx;
 
     std::string name;
     std::vector<MetaComponent> components;
 
-    Idx n_components() const {
-        return static_cast<Idx>(components.size());
-    }
+    Idx n_components() const { return static_cast<Idx>(components.size()); }
 
     MetaComponent const& get_component(std::string const& component_name) const {
         for (auto const& component : components) {
             if (component.name == component_name) {
                 return component;
             }
         }
@@ -267,29 +228,25 @@
 
 using MetaDataset = PGM_MetaDataset;
 
 // meta data
 struct MetaData {
     std::vector<MetaDataset> datasets;
 
-    Idx n_datasets() const {
-        return static_cast<Idx>(datasets.size());
-    }
+    Idx n_datasets() const { return static_cast<Idx>(datasets.size()); }
 
     MetaDataset const& get_dataset(std::string const& dataset_name) const {
         for (auto const& dataset : datasets) {
             if (dataset.name == dataset_name) {
                 return dataset;
             }
         }
         throw std::out_of_range{"Cannot find dataset with name: " + dataset_name + "!\n"};
     }
 };
 
 // little endian
-constexpr bool is_little_endian() {
-    return std::endian::native == std::endian::little;
-}
+constexpr bool is_little_endian() { return std::endian::native == std::endian::little; }
 
-}  // namespace power_grid_model::meta_data
+} // namespace power_grid_model::meta_data
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -25,28 +25,25 @@
 
 namespace meta_data {
 
 using DatasetMap = std::map<std::string, MetaComponent>;
 using AllDatasetMap = std::map<std::string, DatasetMap>;
 
 // template function to add meta data
-template <class CT>
-void add_meta_data(AllDatasetMap& meta) {
+template <class CT> void add_meta_data(AllDatasetMap& meta) {
     meta["input"].try_emplace(CT::name, MetaComponentImpl<typename CT::InputType>{}, CT::name);
     meta["update"].try_emplace(CT::name, MetaComponentImpl<typename CT::UpdateType>{}, CT::name);
     meta["sym_output"].try_emplace(CT::name, MetaComponentImpl<typename CT::template OutputType<true>>{}, CT::name);
     meta["asym_output"].try_emplace(CT::name, MetaComponentImpl<typename CT::template OutputType<false>>{}, CT::name);
     meta["sc_output"].try_emplace(CT::name, MetaComponentImpl<typename CT::ShortCircuitOutputType>{}, CT::name);
 }
 
-template <class T>
-struct MetaDataGeneratorImpl;
+template <class T> struct MetaDataGeneratorImpl;
 
-template <class... ComponentType>
-struct MetaDataGeneratorImpl<ComponentList<ComponentType...>> {
+template <class... ComponentType> struct MetaDataGeneratorImpl<ComponentList<ComponentType...>> {
     using FuncPtr = std::add_pointer_t<void(AllDatasetMap& meta)>;
     static constexpr std::array<FuncPtr, sizeof...(ComponentType)> func_arr{&add_meta_data<ComponentType>...};
 
     static MetaData create_meta() {
         // get all dataset map
         AllDatasetMap all_map{};
         for (auto const func : func_arr) {
@@ -71,12 +68,12 @@
 using MetaDataGenerator = MetaDataGeneratorImpl<AllComponents>;
 
 inline MetaData const& meta_data() {
     static MetaData const meta_data = MetaDataGenerator::create_meta();
     return meta_data;
 }
 
-}  // namespace meta_data
+} // namespace meta_data
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -11,91 +11,68 @@
 #include "three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 // Entry of YBus, node addmittance matrix
 struct YBusElement {
     YBusElementType element_type;
-    Idx idx;  // index of the component
+    Idx idx; // index of the component
 };
 
 // everything here always per unit
 
 // branch math calculation parameter and math output
-template <bool sym>
-struct BranchCalcParam {
+template <bool sym> struct BranchCalcParam {
     std::array<ComplexTensor<sym>, 4> value;
     // getter
-    ComplexTensor<sym>& yff() {
-        return value[0];
-    }
-    ComplexTensor<sym> const& yff() const {
-        return value[0];
-    }
-    ComplexTensor<sym>& yft() {
-        return value[1];
-    }
-    ComplexTensor<sym> const& yft() const {
-        return value[1];
-    }
-    ComplexTensor<sym>& ytf() {
-        return value[2];
-    }
-    ComplexTensor<sym> const& ytf() const {
-        return value[2];
-    }
-    ComplexTensor<sym>& ytt() {
-        return value[3];
-    }
-    ComplexTensor<sym> const& ytt() const {
-        return value[3];
-    }
+    ComplexTensor<sym>& yff() { return value[0]; }
+    ComplexTensor<sym> const& yff() const { return value[0]; }
+    ComplexTensor<sym>& yft() { return value[1]; }
+    ComplexTensor<sym> const& yft() const { return value[1]; }
+    ComplexTensor<sym>& ytf() { return value[2]; }
+    ComplexTensor<sym> const& ytf() const { return value[2]; }
+    ComplexTensor<sym>& ytt() { return value[3]; }
+    ComplexTensor<sym> const& ytt() const { return value[3]; }
 };
 
-template <bool sym>
-struct BranchMathOutput {
+template <bool sym> struct BranchMathOutput {
     ComplexValue<sym> s_f;
     ComplexValue<sym> s_t;
     ComplexValue<sym> i_f;
     ComplexValue<sym> i_t;
 };
 
-template <bool sym>
-struct BranchShortCircuitMathOutput {
+template <bool sym> struct BranchShortCircuitMathOutput {
     ComplexValue<sym> i_f;
     ComplexValue<sym> i_t;
 };
 
 // fault math calculation parameters and math output
 struct FaultCalcParam {
     DoubleComplex y_fault;
     FaultType fault_type;
     FaultPhase fault_phase;
 };
 
-template <bool sym>
-struct FaultShortCircuitMathOutput {
+template <bool sym> struct FaultShortCircuitMathOutput {
     ComplexValue<sym> i_fault;
 };
 
 // appliance math output, always injection direction
 // s > 0, energy appliance -> node
-template <bool sym>
-struct ApplianceMathOutput {
+template <bool sym> struct ApplianceMathOutput {
     ComplexValue<sym> s;
     ComplexValue<sym> i;
 };
-template <bool sym>
-struct ApplianceShortCircuitMathOutput {
+template <bool sym> struct ApplianceShortCircuitMathOutput {
     ComplexValue<sym> i;
 };
 
 // sensor calculation parameters for state estimation
-template <bool sym>
-struct SensorCalcParam {
+template <bool sym> struct SensorCalcParam {
     // measured value of the sensor in p.u.
     // for voltage it is a complex voltage
     // 	   If the imaginary part is NaN, it means the angle calculation is not correct
     // for power it is a complex power
     //      for appliance it is always in injection direction
     //      for branch the direction is node -> branch
     ComplexValue<sym> value;
@@ -116,85 +93,58 @@
     std::vector<BranchIdx> branch_bus_idx;
     std::vector<BranchIdx> fill_in;
     IdxVector source_bus_indptr;
     IdxVector shunt_bus_indptr;
     IdxVector load_gen_bus_indptr;
     std::vector<LoadGenType> load_gen_type;
     IdxVector voltage_sensor_indptr;
-    IdxVector source_power_sensor_indptr;       // indptr of the source
-    IdxVector load_gen_power_sensor_indptr;     // indptr of the load_gen
-    IdxVector shunt_power_sensor_indptr;        // indptr of the shunt
-    IdxVector branch_from_power_sensor_indptr;  // indptr of the branch
-    IdxVector branch_to_power_sensor_indptr;    // indptr of the branch
-    IdxVector bus_power_sensor_indptr;          // indptr of the bus
+    IdxVector source_power_sensor_indptr;      // indptr of the source
+    IdxVector load_gen_power_sensor_indptr;    // indptr of the load_gen
+    IdxVector shunt_power_sensor_indptr;       // indptr of the shunt
+    IdxVector branch_from_power_sensor_indptr; // indptr of the branch
+    IdxVector branch_to_power_sensor_indptr;   // indptr of the branch
+    IdxVector bus_power_sensor_indptr;         // indptr of the bus
 
-    Idx n_bus() const {
-        return static_cast<Idx>(phase_shift.size());
-    }
+    Idx n_bus() const { return static_cast<Idx>(phase_shift.size()); }
 
-    Idx n_branch() const {
-        return static_cast<Idx>(branch_bus_idx.size());
-    }
+    Idx n_branch() const { return static_cast<Idx>(branch_bus_idx.size()); }
 
-    Idx n_source() const {
-        return source_bus_indptr.back();
-    }
+    Idx n_source() const { return source_bus_indptr.back(); }
 
-    Idx n_shunt() const {
-        return shunt_bus_indptr.back();
-    }
+    Idx n_shunt() const { return shunt_bus_indptr.back(); }
 
-    Idx n_load_gen() const {
-        return load_gen_bus_indptr.back();
-    }
+    Idx n_load_gen() const { return load_gen_bus_indptr.back(); }
 
-    Idx n_voltage_sensor() const {
-        return voltage_sensor_indptr.back();
-    }
+    Idx n_voltage_sensor() const { return voltage_sensor_indptr.back(); }
 
-    Idx n_source_power_sensor() const {
-        return source_power_sensor_indptr.back();
-    }
+    Idx n_source_power_sensor() const { return source_power_sensor_indptr.back(); }
 
-    Idx n_load_gen_power_sensor() const {
-        return load_gen_power_sensor_indptr.back();
-    }
+    Idx n_load_gen_power_sensor() const { return load_gen_power_sensor_indptr.back(); }
 
-    Idx n_shunt_power_power_sensor() const {
-        return shunt_power_sensor_indptr.back();
-    }
+    Idx n_shunt_power_power_sensor() const { return shunt_power_sensor_indptr.back(); }
 
-    Idx n_branch_from_power_sensor() const {
-        return branch_from_power_sensor_indptr.back();
-    }
+    Idx n_branch_from_power_sensor() const { return branch_from_power_sensor_indptr.back(); }
 
-    Idx n_branch_to_power_sensor() const {
-        return branch_to_power_sensor_indptr.back();
-    }
+    Idx n_branch_to_power_sensor() const { return branch_to_power_sensor_indptr.back(); }
 
-    Idx n_bus_power_sensor() const {
-        return bus_power_sensor_indptr.back();
-    }
+    Idx n_bus_power_sensor() const { return bus_power_sensor_indptr.back(); }
 };
 
-template <bool sym>
-struct MathModelParam {
+template <bool sym> struct MathModelParam {
     std::vector<BranchCalcParam<sym>> branch_param;
     ComplexTensorVector<sym> shunt_param;
     ComplexTensorVector<sym> source_param;
 };
 
-template <bool sym>
-struct PowerFlowInput {
-    ComplexVector source;                 // Complex u_ref of each source
-    ComplexValueVector<sym> s_injection;  // Specified injection power of each load_gen
+template <bool sym> struct PowerFlowInput {
+    ComplexVector source;                // Complex u_ref of each source
+    ComplexValueVector<sym> s_injection; // Specified injection power of each load_gen
 };
 
-template <bool sym>
-struct StateEstimationInput {
+template <bool sym> struct StateEstimationInput {
     // connection status of shunt, load_gen, source
     // this is needed to determine if a measurement is relevant
     // if the shunt/load_gen/source is disconnected, all its measurements are discarded
     IntSVector shunt_status;
     IntSVector load_gen_status;
     IntSVector source_status;
     // measured value
@@ -204,31 +154,29 @@
     std::vector<SensorCalcParam<sym>> measured_shunt_power;
     std::vector<SensorCalcParam<sym>> measured_branch_from_power;
     std::vector<SensorCalcParam<sym>> measured_branch_to_power;
     std::vector<SensorCalcParam<sym>> measured_bus_injection;
 };
 
 struct ShortCircuitInput {
-    IdxVector fault_bus_indptr;  // indptr of the fault
+    IdxVector fault_bus_indptr; // indptr of the fault
     std::vector<FaultCalcParam> faults;
-    ComplexVector source;  // Complex u_ref of each source
+    ComplexVector source; // Complex u_ref of each source
 };
 
-template <bool sym>
-struct MathOutput {
+template <bool sym> struct MathOutput {
     std::vector<ComplexValue<sym>> u;
     std::vector<ComplexValue<sym>> bus_injection;
     std::vector<BranchMathOutput<sym>> branch;
     std::vector<ApplianceMathOutput<sym>> source;
     std::vector<ApplianceMathOutput<sym>> shunt;
     std::vector<ApplianceMathOutput<sym>> load_gen;
 };
 
-template <bool sym>
-struct ShortCircuitMathOutput {
+template <bool sym> struct ShortCircuitMathOutput {
     std::vector<ComplexValue<sym>> u_bus;
     std::vector<FaultShortCircuitMathOutput<sym>> fault;
     std::vector<BranchShortCircuitMathOutput<sym>> branch;
     std::vector<ApplianceShortCircuitMathOutput<sym>> source;
     std::vector<ApplianceShortCircuitMathOutput<sym>> shunt;
 };
 
@@ -263,17 +211,16 @@
 
 static_assert(!short_circuit_math_output_type<MathOutput<true>>);
 static_assert(!short_circuit_math_output_type<MathOutput<false>>);
 static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<true>>);
 static_assert(short_circuit_math_output_type<ShortCircuitMathOutput<false>>);
 
 template <typename T>
-concept math_output_type = (symmetric_math_output_type<T> ||
-                            asymmetric_math_output_type<T>)&&(steady_state_math_output_type<T> ||
-                                                              short_circuit_math_output_type<T>);
+concept math_output_type = (symmetric_math_output_type<T> || asymmetric_math_output_type<T>) &&
+                           (steady_state_math_output_type<T> || short_circuit_math_output_type<T>);
 
 static_assert(math_output_type<MathOutput<true>>);
 static_assert(math_output_type<MathOutput<false>>);
 static_assert(math_output_type<ShortCircuitMathOutput<true>>);
 static_assert(math_output_type<ShortCircuitMathOutput<false>>);
 
 // component indices at physical model side
@@ -285,20 +232,18 @@
     std::vector<BranchIdx> branch_node_idx;
     std::vector<Branch3Idx> branch3_node_idx;
     IdxVector shunt_node_idx;
     IdxVector source_node_idx;
     IdxVector load_gen_node_idx;
     std::vector<LoadGenType> load_gen_type;
     IdxVector voltage_sensor_node_idx;
-    IdxVector power_sensor_object_idx;  // the index is relative to branch, source, shunt, or load_gen
+    IdxVector power_sensor_object_idx; // the index is relative to branch, source, shunt, or load_gen
     std::vector<MeasuredTerminalType> power_sensor_terminal_type;
 
-    inline Idx n_node_total() const {
-        return n_node + (Idx)branch3_node_idx.size();
-    }
+    inline Idx n_node_total() const { return n_node + (Idx)branch3_node_idx.size(); }
 };
 
 // connection property
 using BranchConnected = std::array<IntS, 2>;
 using Branch3Connected = std::array<IntS, 3>;
 
 // component connection property at model side
@@ -345,23 +290,23 @@
     std::vector<Idx2D> node;
     std::vector<Idx2D> branch;
     std::vector<Idx2DBranch3> branch3;
     std::vector<Idx2D> shunt;
     std::vector<Idx2D> load_gen;
     std::vector<Idx2D> source;
     std::vector<Idx2D> voltage_sensor;
-    std::vector<Idx2D> power_sensor;  // can be coupled to branch-from/to, source, load_gen, or shunt sensor
+    std::vector<Idx2D> power_sensor; // can be coupled to branch-from/to, source, load_gen, or shunt sensor
 };
 
 // change of update cause topology and param change, or just param change
 struct UpdateChange {
     bool topo{};
     bool param{};
 
     friend constexpr UpdateChange operator||(UpdateChange const& x, UpdateChange const& y) {
         return UpdateChange{x.topo || y.topo, x.param || y.param};
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -14,91 +14,76 @@
 #include "../calculation_parameters.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Appliance : public Base {
-   public:
+  public:
     using InputType = ApplianceInput;
     using UpdateType = ApplianceUpdate;
-    template <bool sym>
-    using OutputType = ApplianceOutput<sym>;
+    template <bool sym> using OutputType = ApplianceOutput<sym>;
     using ShortCircuitOutputType = ApplianceShortCircuitOutput;
     static constexpr char const* name = "appliance";
 
     Appliance(ApplianceInput const& appliance_input, double u)
         : Base{appliance_input},
           node_{appliance_input.node},
           status_{appliance_input.status != 0},
-          base_i_{base_power_3p / u / sqrt3} {
-    }
+          base_i_{base_power_3p / u / sqrt3} {}
 
     // getter
-    ID node() const {
-        return node_;
-    }
-    bool status() const {
-        return status_;
-    }
-    double base_i() const {
-        return base_i_;
-    }
-    bool energized(bool is_connected_to_source) const final {
-        return is_connected_to_source && status_;
-    }
+    ID node() const { return node_; }
+    bool status() const { return status_; }
+    double base_i() const { return base_i_; }
+    bool energized(bool is_connected_to_source) const final { return is_connected_to_source && status_; }
 
     // setter
     bool set_status(IntS new_status) {
         if (new_status == na_IntS) {
             return false;
         }
         if (static_cast<bool>(new_status) == status_) {
             return false;
         }
         status_ = static_cast<bool>(new_status);
         return true;
     }
 
     // empty output
-    template <bool sym>
-    ApplianceOutput<sym> get_null_output() const {
+    template <bool sym> ApplianceOutput<sym> get_null_output() const {
         ApplianceOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
     ApplianceShortCircuitOutput get_null_sc_output() const {
         ApplianceShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
-    template <bool sym>
-    ApplianceOutput<sym> get_output(ApplianceMathOutput<sym> const& appliance_math_output) const {
+    template <bool sym> ApplianceOutput<sym> get_output(ApplianceMathOutput<sym> const& appliance_math_output) const {
         ApplianceOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(energized(true));
         output.p = base_power<sym> * real(appliance_math_output.s) * injection_direction();
         output.q = base_power<sym> * imag(appliance_math_output.s) * injection_direction();
         output.s = base_power<sym> * cabs(appliance_math_output.s);
         output.i = base_i_ * cabs(appliance_math_output.i);
         // pf
         if constexpr (sym) {
             if (output.s < numerical_tolerance) {
                 output.pf = 0.0;
-            }
-            else {
+            } else {
                 output.pf = output.p / output.s;
             }
-        }
-        else {
+        } else {
             for (size_t j = 0; j != 3; ++j) {
                 if (output.s(j) < numerical_tolerance) {
                     output.pf(j) = 0.0;
-                }
-                else {
+                } else {
                     output.pf(j) = output.p(j) / output.s(j);
                 }
             }
         }
         return output;
     }
     ApplianceShortCircuitOutput get_sc_output(ComplexValue<false> const& i) const {
@@ -108,36 +93,34 @@
         output.i_angle = arg(i * injection_direction());
         return output;
     }
     ApplianceShortCircuitOutput get_sc_output(ComplexValue<true> const& i) const {
         ComplexValue<false> const iabc{i};
         return get_sc_output(iabc);
     }
-    template <bool sym>
-    ApplianceOutput<sym> get_output(ComplexValue<sym> const& u) const {
+    template <bool sym> ApplianceOutput<sym> get_output(ComplexValue<sym> const& u) const {
         if constexpr (sym) {
             return get_output<true>(sym_u2si(u));
-        }
-        else {
+        } else {
             return get_output<false>(asym_u2si(u));
         }
     }
     template <bool sym>
     ApplianceShortCircuitOutput get_sc_output(ApplianceShortCircuitMathOutput<sym> const& appliance_math_output) const {
         return get_sc_output(appliance_math_output.i);
     }
 
-   private:
+  private:
     ID node_;
     bool status_;
     double base_i_;
 
     // pure virtual functions for translate from u to s/i
     virtual ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const = 0;
     virtual ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const = 0;
 
     virtual double injection_direction() const = 0;
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -11,40 +11,36 @@
 #include "../auxiliary/update.hpp"
 #include "../enum.hpp"
 #include "../power_grid_model.hpp"
 
 namespace power_grid_model {
 
 class Base {
-   public:
+  public:
     using InputType = BaseInput;
     using UpdateType = BaseUpdate;
-    template <bool sym>
-    using OutputType = BaseOutput;
+    template <bool sym> using OutputType = BaseOutput;
     static constexpr char const* name = "base";
     virtual ComponentType math_model_type() const = 0;
 
-    explicit Base(BaseInput const& base_input) : id_{base_input.id} {
-    }
+    explicit Base(BaseInput const& base_input) : id_{base_input.id} {}
     virtual ~Base() = default;
-    constexpr ID id() const noexcept {
-        return id_;
-    }
+    constexpr ID id() const noexcept { return id_; }
     constexpr BaseOutput base_output(bool is_energized) const {
         return BaseOutput{id_, static_cast<IntS>(is_energized)};
     }
     virtual bool energized(bool is_connected_to_source) const = 0;
 
     Base(Base&&) = default;
     Base& operator=(Base&&) = default;
 
-   protected:
+  protected:
     Base(const Base&) = default;
     Base& operator=(const Base&) = default;
 
-   private:
+  private:
     ID id_;
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,90 +15,73 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Branch : public Base {
-   public:
+  public:
     using InputType = BranchInput;
     using UpdateType = BranchUpdate;
-    template <bool sym>
-    using OutputType = BranchOutput<sym>;
+    template <bool sym> using OutputType = BranchOutput<sym>;
     using ShortCircuitOutputType = BranchShortCircuitOutput;
     static constexpr char const* name = "branch";
-    ComponentType math_model_type() const final {
-        return ComponentType::branch;
-    }
+    ComponentType math_model_type() const final { return ComponentType::branch; }
 
     explicit Branch(BranchInput const& branch_input)
         : Base{branch_input},
           from_node_{branch_input.from_node},
           to_node_{branch_input.to_node},
           from_status_{static_cast<bool>(branch_input.from_status)},
           to_status_{static_cast<bool>(branch_input.to_status)} {
         if (from_node_ == to_node_) {
             throw InvalidBranch{id(), from_node_};
         }
     }
 
     // getter
-    ID from_node() const {
-        return from_node_;
-    }
-    ID to_node() const {
-        return to_node_;
-    }
-    bool from_status() const {
-        return from_status_;
-    }
-    bool to_status() const {
-        return to_status_;
-    }
-    bool branch_status() const {
-        return from_status_ && to_status_;
-    }
-    template <bool sym>
-    BranchCalcParam<sym> calc_param(bool is_connected_to_source = true) const {
+    ID from_node() const { return from_node_; }
+    ID to_node() const { return to_node_; }
+    bool from_status() const { return from_status_; }
+    bool to_status() const { return to_status_; }
+    bool branch_status() const { return from_status_ && to_status_; }
+    template <bool sym> BranchCalcParam<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return BranchCalcParam<sym>{};
         }
         if constexpr (sym) {
             return sym_calc_param();
-        }
-        else {
+        } else {
             return asym_calc_param();
         }
     }
 
     // virtual getter
     bool energized(bool is_connected_to_source) const final {
         return is_connected_to_source && (from_status_ || to_status_);
     }
     virtual double base_i_from() const = 0;
     virtual double base_i_to() const = 0;
     virtual double loading(double max_s, double max_i) const = 0;
-    virtual double phase_shift() const = 0;  // shift theta_from - theta_to
+    virtual double phase_shift() const = 0; // shift theta_from - theta_to
     virtual bool is_param_mutable() const = 0;
 
-    template <bool sym>
-    BranchOutput<sym> get_output(ComplexValue<sym> const& u_f, ComplexValue<sym> const& u_t) const {
+    template <bool sym> BranchOutput<sym> get_output(ComplexValue<sym> const& u_f, ComplexValue<sym> const& u_t) const {
         // calculate flow
         BranchCalcParam<sym> const param = calc_param<sym>();
         BranchMathOutput<sym> branch_math_output{};
         branch_math_output.i_f = dot(param.yff(), u_f) + dot(param.yft(), u_t);
         branch_math_output.i_t = dot(param.ytf(), u_f) + dot(param.ytt(), u_t);
         branch_math_output.s_f = u_f * conj(branch_math_output.i_f);
         branch_math_output.s_t = u_t * conj(branch_math_output.i_t);
         // calculate result
         return get_output<sym>(branch_math_output);
     }
 
-    template <bool sym>
-    BranchOutput<sym> get_output(BranchMathOutput<sym> const& branch_math_output) const {
+    template <bool sym> BranchOutput<sym> get_output(BranchMathOutput<sym> const& branch_math_output) const {
         // result object
         BranchOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         // calculate result
         output.p_from = base_power<sym> * real(branch_math_output.s_f);
         output.q_from = base_power<sym> * imag(branch_math_output.s_f);
         output.i_from = base_i_from() * cabs(branch_math_output.i_f);
@@ -132,16 +115,15 @@
     }
 
     BranchShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<true> const& branch_math_output) const {
         return get_sc_output(BranchShortCircuitMathOutput<false>{.i_f = ComplexValue<false>{branch_math_output.i_f},
                                                                  .i_t = ComplexValue<false>{branch_math_output.i_t}});
     }
 
-    template <bool sym>
-    BranchOutput<sym> get_null_output() const {
+    template <bool sym> BranchOutput<sym> get_null_output() const {
         BranchOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     BranchShortCircuitOutput get_null_sc_output() const {
         BranchShortCircuitOutput output{};
@@ -169,32 +151,31 @@
     UpdateChange update(BranchUpdate const& update) {
         assert(update.id == id());
         bool const changed = set_status(update.from_status, update.to_status);
         // change branch connection will change both topo and param
         return {changed, changed};
     }
 
-   protected:
+  protected:
     // calculate branch param based on symmetric component
-    BranchCalcParam<true> calc_param_y_sym(
-        DoubleComplex const& y_series,  // y_series must be converted to the "to" side of the branch
-        DoubleComplex const& y_shunt,   // y_shunt must be converted to the "to" side of the branch
-        DoubleComplex const& tap_ratio) const {
+    BranchCalcParam<true>
+    calc_param_y_sym(DoubleComplex const& y_series, // y_series must be converted to the "to" side of the branch
+                     DoubleComplex const& y_shunt,  // y_shunt must be converted to the "to" side of the branch
+                     DoubleComplex const& tap_ratio) const {
         double const tap = cabs(tap_ratio);
         BranchCalcParam<true> param{};
         // not both connected
         if (!(from_status_ && to_status_)) {
             // single connected
             if (from_status_ || to_status_) {
                 DoubleComplex branch_shunt;
                 // shunt value
                 if (cabs(y_shunt) < numerical_tolerance) {
                     branch_shunt = 0.0;
-                }
-                else {
+                } else {
                     // branch_shunt = y_shunt/2 + 1/(1/y_series + 2/y_shunt)
                     branch_shunt = 0.5 * y_shunt + 1.0 / (1.0 / y_series + 2.0 / y_shunt);
                 }
                 // from or to connected
                 param.yff() = from_status_ ? (1.0 / tap / tap) * branch_shunt : 0.0;
                 param.ytt() = to_status_ ? branch_shunt : 0.0;
             }
@@ -223,20 +204,20 @@
         for (size_t i = 0; i < 4; ++i) {
             param.value[i] = ComplexTensor<false>{(2.0 * param1.value[i] + param0.value[i]) / 3.0,
                                                   (param0.value[i] - param1.value[i]) / 3.0};
         }
         return param;
     }
 
-   private:
+  private:
     ID from_node_;
     ID to_node_;
     bool from_status_;
     bool to_status_;
 
     virtual BranchCalcParam<true> sym_calc_param() const = 0;
     virtual BranchCalcParam<false> asym_calc_param() const = 0;
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,21 @@
 #include "../auxiliary/update.hpp"
 #include "../calculation_parameters.hpp"
 #include "../exception.hpp"
 
 namespace power_grid_model {
 
 class Branch3 : public Base {
-   public:
+  public:
     using InputType = Branch3Input;
     using UpdateType = Branch3Update;
-    template <bool sym>
-    using OutputType = Branch3Output<sym>;
+    template <bool sym> using OutputType = Branch3Output<sym>;
     using ShortCircuitOutputType = Branch3ShortCircuitOutput;
     static constexpr char const* name = "branch3";
-    ComponentType math_model_type() const final {
-        return ComponentType::branch3;
-    }
+    ComponentType math_model_type() const final { return ComponentType::branch3; }
 
     explicit Branch3(Branch3Input const& branch3_input)
         : Base{branch3_input},
           node_1_{branch3_input.node_1},
           node_2_{branch3_input.node_2},
           node_3_{branch3_input.node_3},
           status_1_{static_cast<bool>(branch3_input.status_1)},
@@ -38,55 +35,41 @@
           status_3_{static_cast<bool>(branch3_input.status_3)} {
         if (node_1_ == node_2_ || node_1_ == node_3_ || node_2_ == node_3_) {
             throw InvalidBranch3{id(), node_1_, node_2_, node_3_};
         }
     }
 
     // getter
-    ID node_1() const {
-        return node_1_;
-    }
-    ID node_2() const {
-        return node_2_;
-    }
-    ID node_3() const {
-        return node_3_;
-    }
-    bool status_1() const {
-        return status_1_;
-    }
-    bool status_2() const {
-        return status_2_;
-    }
-    bool status_3() const {
-        return status_3_;
-    }
+    ID node_1() const { return node_1_; }
+    ID node_2() const { return node_2_; }
+    ID node_3() const { return node_3_; }
+    bool status_1() const { return status_1_; }
+    bool status_2() const { return status_2_; }
+    bool status_3() const { return status_3_; }
     bool branch3_status() const {
-        return status_1_ && status_2_ && status_3_;  // TODO: check if this makes sense for branch3
+        return status_1_ && status_2_ && status_3_; // TODO: check if this makes sense for branch3
     }
 
     // virtual getter
     bool energized(bool is_connected_to_source = true) const final {
         return is_connected_to_source && (status_1_ || status_2_ || status_3_);
     }
     virtual double base_i_1() const = 0;
     virtual double base_i_2() const = 0;
     virtual double base_i_3() const = 0;
     virtual double loading(double s_1, double s_2, double s_3) const = 0;
     virtual std::array<double, 3> phase_shift() const = 0;
 
-    template <bool sym>
-    std::array<BranchCalcParam<sym>, 3> calc_param(bool is_connected_to_source = true) const {
+    template <bool sym> std::array<BranchCalcParam<sym>, 3> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return std::array<BranchCalcParam<sym>, 3>{};
         }
         if constexpr (sym) {
             return sym_calc_param();
-        }
-        else {
+        } else {
             return asym_calc_param();
         }
     }
 
     template <bool sym>
     Branch3Output<sym> get_output(BranchMathOutput<sym> const& branch_math_output1,
                                   BranchMathOutput<sym> const& branch_math_output2,
@@ -139,16 +122,15 @@
     template <bool sym>
     Branch3ShortCircuitOutput get_sc_output(BranchShortCircuitMathOutput<sym> const& branch_math_output1,
                                             BranchShortCircuitMathOutput<sym> const& branch_math_output2,
                                             BranchShortCircuitMathOutput<sym> const& branch_math_output3) const {
         return get_sc_output(branch_math_output1.i_f, branch_math_output2.i_f, branch_math_output3.i_f);
     }
 
-    template <bool sym>
-    Branch3Output<sym> get_null_output() const {
+    template <bool sym> Branch3Output<sym> get_null_output() const {
         Branch3Output<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     Branch3ShortCircuitOutput get_null_sc_output() const {
         Branch3ShortCircuitOutput output{};
@@ -181,22 +163,22 @@
     UpdateChange update(Branch3Update const& update) {
         assert(update.id == id());
         bool const changed = set_status(update.status_1, update.status_2, update.status_3);
         // change in branch3 connection will change both topo and param
         return {changed, changed};
     }
 
-   private:
+  private:
     ID node_1_;
     ID node_2_;
     ID node_3_;
     bool status_1_;
     bool status_2_;
     bool status_3_;
 
     virtual std::array<BranchCalcParam<true>, 3> sym_calc_param() const = 0;
     virtual std::array<BranchCalcParam<false>, 3> asym_calc_param() const = 0;
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 #include "../calculation_parameters.hpp"
 #include "../enum.hpp"
 #include "../exception.hpp"
 
 namespace power_grid_model {
 
 class Fault final : public Base {
-   public:
+  public:
     using InputType = FaultInput;
     using UpdateType = FaultUpdate;
-    template <bool sym>
-    using OutputType = FaultOutput;
+    template <bool sym> using OutputType = FaultOutput;
     using ShortCircuitOutputType = FaultShortCircuitOutput;
     static constexpr char const* name = "fault";
-    ComponentType math_model_type() const final {
-        return ComponentType::fault;
-    }
+    ComponentType math_model_type() const final { return ComponentType::fault; }
 
     explicit Fault(FaultInput const& fault_input)
         : Base{fault_input},
           status_{static_cast<bool>(fault_input.status)},
           fault_type_{fault_input.fault_type},
           fault_phase_{fault_input.fault_phase == FaultPhase::nan ? FaultPhase::default_value
                                                                   : fault_input.fault_phase},
@@ -57,25 +54,21 @@
         }
         // calculate the fault admittance in p.u.
         double const base_z = u_rated * u_rated / base_power_3p;
         param.y_fault = base_z / (r_f_ + 1.0i * x_f_);
         return param;
     }
 
-    FaultOutput get_null_output() const {
-        return get_null_output_impl<FaultOutput>();
-    }
+    FaultOutput get_null_output() const { return get_null_output_impl<FaultOutput>(); }
     FaultOutput get_output() const {
         // During power flow and state estimation the fault object will have an empty output
         return get_null_output();
     }
 
-    FaultShortCircuitOutput get_null_sc_output() const {
-        return get_null_output_impl<FaultShortCircuitOutput>();
-    }
+    FaultShortCircuitOutput get_null_sc_output() const { return get_null_output_impl<FaultShortCircuitOutput>(); }
     FaultShortCircuitOutput get_sc_output(ComplexValue<false> i_f, double const u_rated) const {
         // translate pu to A
         double const base_i = base_power_3p / u_rated / sqrt3;
         i_f = i_f * base_i;
         // result object
         FaultShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(true);
@@ -111,24 +104,20 @@
         if (!is_nan(update.r_f)) {
             r_f_ = update.r_f;
         }
         if (!is_nan(update.x_f)) {
             x_f_ = update.x_f;
         }
         check_sanity();
-        return {false, false};  // topology and parameters do not change
+        return {false, false}; // topology and parameters do not change
     }
 
-    constexpr bool energized(bool is_connected_to_source) const final {
-        return is_connected_to_source;
-    }
+    constexpr bool energized(bool is_connected_to_source) const final { return is_connected_to_source; }
 
-    constexpr bool status() const {
-        return status_;
-    }
+    constexpr bool status() const { return status_; }
 
     // setter
     constexpr bool set_status(IntS new_status) {
         if (new_status == na_IntS) {
             return false;
         }
         if (static_cast<bool>(new_status) == status_) {
@@ -154,71 +143,68 @@
         using enum FaultType;
 
         if (fault_phase_ == FaultPhase::default_value) {
             auto const default_phase = [](FaultType fault_type) {
                 switch (fault_type) {
                     using enum FaultPhase;
 
-                    case three_phase:
-                        return abc;
-                    case single_phase_to_ground:
-                        return a;
-                    case two_phase:
-                        [[fallthrough]];
-                    case two_phase_to_ground:
-                        return bc;
-                    default:
-                        throw InvalidShortCircuitType(fault_type);
+                case three_phase:
+                    return abc;
+                case single_phase_to_ground:
+                    return a;
+                case two_phase:
+                    [[fallthrough]];
+                case two_phase_to_ground:
+                    return bc;
+                default:
+                    throw InvalidShortCircuitType(fault_type);
                 }
             }(fault_type_);
             return default_phase;
         }
         return fault_phase_;
     }
-    constexpr ID get_fault_object() const {
-        return fault_object_;
-    }
+    constexpr ID get_fault_object() const { return fault_object_; }
 
-   private:
+  private:
     // short circuit parameters
     bool status_;
     FaultType fault_type_;
     FaultPhase fault_phase_;
     ID fault_object_;
     double r_f_;
     double x_f_;
 
-    template <std::derived_from<BaseOutput> T>
-    T get_null_output_impl() const {
+    template <std::derived_from<BaseOutput> T> T get_null_output_impl() const {
         T output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     void check_sanity() {
         using enum FaultPhase;
 
         auto const check_supported = [&](auto const& iterable) {
             if (std::find(cbegin(iterable), cend(iterable), fault_phase_) == cend(iterable)) {
                 throw InvalidShortCircuitPhases(fault_type_, fault_phase_);
             }
         };
         switch (fault_type_) {
-            case FaultType::three_phase:
-                return check_supported(std::array{FaultPhase::nan, default_value, abc});
-            case FaultType::single_phase_to_ground:
-                return check_supported(std::array{FaultPhase::nan, default_value, a, b, c});
-            case FaultType::two_phase:
-                [[fallthrough]];
-            case FaultType::two_phase_to_ground:
-                return check_supported(std::array{FaultPhase::nan, default_value, ab, ac, bc});
-            case FaultType::nan:
-                return check_supported(std::array{FaultPhase::nan, default_value, abc, a, b, c, ab, ac, bc});
-            default:
-                throw InvalidShortCircuitType(fault_type_);
+        case FaultType::three_phase:
+            return check_supported(std::array{FaultPhase::nan, default_value, abc});
+        case FaultType::single_phase_to_ground:
+            return check_supported(std::array{FaultPhase::nan, default_value, a, b, c});
+        case FaultType::two_phase:
+            [[fallthrough]];
+        case FaultType::two_phase_to_ground:
+            return check_supported(std::array{FaultPhase::nan, default_value, ab, ac, bc});
+        case FaultType::nan:
+            return check_supported(std::array{FaultPhase::nan, default_value, abc, a, b, c, ab, ac, bc});
+        default:
+            throw InvalidShortCircuitType(fault_type_);
         }
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Line final : public Branch {
-   public:
+  public:
     using InputType = LineInput;
     using UpdateType = BranchUpdate;
     static constexpr char const* name = "line";
 
     explicit Line(LineInput const& line_input, double system_frequency, double u1, double u2)
         : Branch{line_input}, i_n_{line_input.i_n}, base_i_{base_power_3p / u1 / sqrt3} {
         if (cabs(u1 - u2) > numerical_tolerance) {
@@ -33,42 +33,30 @@
         y1_series_ = 1.0 / (line_input.r1 + 1.0i * line_input.x1) / base_y;
         y1_shunt_ = 2.0 * pi * system_frequency * line_input.c1 / base_y * (line_input.tan1 + 1.0i);
         y0_series_ = 1.0 / (line_input.r0 + 1.0i * line_input.x0) / base_y;
         y0_shunt_ = 2.0 * pi * system_frequency * line_input.c0 / base_y * (line_input.tan0 + 1.0i);
     }
 
     // override getter
-    double base_i_from() const final {
-        return base_i_;
-    }
-    double base_i_to() const final {
-        return base_i_;
-    }
-    double loading(double, double max_i) const final {
-        return max_i / i_n_;
-    };
-    double phase_shift() const final {
-        return 0.0;
-    }
-    bool is_param_mutable() const final {
-        return false;
-    }
+    double base_i_from() const final { return base_i_; }
+    double base_i_to() const final { return base_i_; }
+    double loading(double, double max_i) const final { return max_i / i_n_; };
+    double phase_shift() const final { return 0.0; }
+    bool is_param_mutable() const final { return false; }
 
-   private:
+  private:
     double i_n_;
     double base_i_;
     DoubleComplex y1_series_;
     DoubleComplex y1_shunt_;
     DoubleComplex y0_series_;
     DoubleComplex y0_shunt_;
 
-    BranchCalcParam<true> sym_calc_param() const final {
-        return calc_param_y_sym(y1_series_, y1_shunt_, 1.0);
-    }
+    BranchCalcParam<true> sym_calc_param() const final { return calc_param_y_sym(y1_series_, y1_shunt_, 1.0); }
     BranchCalcParam<false> asym_calc_param() const final {
         return calc_param_y_asym(y1_series_, y1_shunt_, y0_series_, y0_shunt_, 1.0);
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -15,46 +15,31 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Link final : public Branch {
-   public:
+  public:
     using InputType = LinkInput;
     using UpdateType = BranchUpdate;
     static constexpr char const* name = "link";
 
     explicit Link(LinkInput const& link_input, double u1, double u2)
-        : Branch{link_input}, base_i_from_{base_power_3p / u1 / sqrt3}, base_i_to_{base_power_3p / u2 / sqrt3} {
-    }
+        : Branch{link_input}, base_i_from_{base_power_3p / u1 / sqrt3}, base_i_to_{base_power_3p / u2 / sqrt3} {}
 
     // override getter
-    double base_i_from() const final {
-        return base_i_from_;
-    }
-    double base_i_to() const final {
-        return base_i_to_;
-    }
-    double loading(double, double) const final {
-        return 0.0;
-    };
-    double phase_shift() const final {
-        return 0.0;
-    }
-    bool is_param_mutable() const final {
-        return false;
-    }
+    double base_i_from() const final { return base_i_from_; }
+    double base_i_to() const final { return base_i_to_; }
+    double loading(double, double) const final { return 0.0; };
+    double phase_shift() const final { return 0.0; }
+    bool is_param_mutable() const final { return false; }
 
-   private:
+  private:
     double base_i_from_;
     double base_i_to_;
-    BranchCalcParam<true> sym_calc_param() const final {
-        return calc_param_y_sym(y_link, 0.0, 1.0);
-    }
-    BranchCalcParam<false> asym_calc_param() const final {
-        return calc_param_y_asym(y_link, 0.0, y_link, 0.0, 1.0);
-    }
+    BranchCalcParam<true> sym_calc_param() const final { return calc_param_y_sym(y_link, 0.0, 1.0); }
+    BranchCalcParam<false> asym_calc_param() const final { return calc_param_y_asym(y_link, 0.0, y_link, 0.0, 1.0); }
 };
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -16,62 +16,55 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class GenericLoadGen : public Appliance {
-   public:
+  public:
     using InputType = GenericLoadGenInput;
     static constexpr char const* name = "generic_load_gen";
-    ComponentType math_model_type() const final {
-        return ComponentType::generic_load_gen;
-    }
+    ComponentType math_model_type() const final { return ComponentType::generic_load_gen; }
 
     explicit GenericLoadGen(GenericLoadGenInput const& generic_load_gen_input, double u)
-        : Appliance{generic_load_gen_input, u}, type_{generic_load_gen_input.type} {
-    }
+        : Appliance{generic_load_gen_input, u}, type_{generic_load_gen_input.type} {}
 
     // getter for load type
-    LoadGenType type() const {
-        return type_;
-    }
+    LoadGenType type() const { return type_; }
     // getter for calculation param, power injection
-    template <bool sym>
-    ComplexValue<sym> calc_param(bool is_connected_to_source = true) const {
+    template <bool sym> ComplexValue<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return ComplexValue<sym>{};
         }
         if constexpr (sym) {
             return sym_calc_param();
-        }
-        else {
+        } else {
             return asym_calc_param();
         }
     }
 
-   private:
+  private:
     LoadGenType type_;
     virtual ComplexValue<true> sym_calc_param() const = 0;
     virtual ComplexValue<false> asym_calc_param() const = 0;
 };
 
 // abstraction of load/generation
 class GenericLoad : public GenericLoadGen {
-   public:
+  public:
     using GenericLoadGen::GenericLoadGen;
 };
 class GenericGenerator : public GenericLoadGen {
-   public:
+  public:
     using GenericLoadGen::GenericLoadGen;
 };
 
 template <bool sym, bool is_gen>
 class LoadGen final : public std::conditional_t<is_gen, GenericGenerator, GenericLoad> {
-   public:
+  public:
     using InputType = LoadGenInput<sym>;
     using UpdateType = LoadGenUpdate<sym>;
     using BaseClass = std::conditional_t<is_gen, GenericGenerator, GenericLoad>;
     static constexpr char const* name = sym ? (is_gen ? "sym_gen" : "sym_load") : (is_gen ? "asym_gen" : "asym_load");
 
     LoadGen(LoadGenInput<sym> const& load_gen_input, double u) : BaseClass{load_gen_input, u} {
         set_power(load_gen_input.p_specified, load_gen_input.q_specified);
@@ -92,60 +85,48 @@
         assert(update.id == this->id());
         this->set_status(update.status);
         set_power(update.p_specified, update.q_specified);
         // change load connection and/or value will not change topology or parameters
         return {false, false};
     }
 
-   private:
-    ComplexValue<sym> s_specified_{};  // specified power injection
+  private:
+    ComplexValue<sym> s_specified_{}; // specified power injection
 
     // direction of load_gen
     static constexpr double direction_ = is_gen ? 1.0 : -1.0;
 
     // override calc_param
-    ComplexValue<true> sym_calc_param() const final {
-        return mean_val(s_specified_);
-    }
-    ComplexValue<false> asym_calc_param() const final {
-        return piecewise_complex_value(s_specified_);
-    }
-    template <bool sym_calc>
-    ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
+    ComplexValue<true> sym_calc_param() const final { return mean_val(s_specified_); }
+    ComplexValue<false> asym_calc_param() const final { return piecewise_complex_value(s_specified_); }
+    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
         ApplianceMathOutput<sym_calc> appliance_math_output;
         appliance_math_output.s = scale_power<sym_calc>(u);
         appliance_math_output.i = conj(appliance_math_output.s / u);
         return appliance_math_output;
     }
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final {
-        return u2si<true>(u);
-    }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final {
-        return u2si<false>(u);
-    }
+    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final { return u2si<true>(u); }
+    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final { return u2si<false>(u); }
 
-    double injection_direction() const final {
-        return direction_;
-    }
+    double injection_direction() const final { return direction_; }
 
     // scale load
-    template <bool sym_calc>
-    ComplexValue<sym_calc> scale_power(ComplexValue<sym_calc> u) const {
+    template <bool sym_calc> ComplexValue<sym_calc> scale_power(ComplexValue<sym_calc> u) const {
         using enum LoadGenType;
 
         ComplexValue<sym_calc> s = this->template calc_param<sym_calc>();
         switch (this->type()) {
-            case const_pq:
-                return s;
-            case const_y:
-                return s * abs2(u);
-            case const_i:
-                return s * cabs(u);
-            default:
-                throw MissingCaseForEnumError(std::string(this->name) + " power scaling factor", this->type());
+        case const_pq:
+            return s;
+        case const_y:
+            return s * abs2(u);
+        case const_i:
+            return s * cabs(u);
+        default:
+            throw MissingCaseForEnumError(std::string(this->name) + " power scaling factor", this->type());
         }
     }
 };
 
 // explicit instantiation
 template class LoadGen<true, true>;
 template class LoadGen<true, false>;
@@ -153,10 +134,10 @@
 template class LoadGen<false, false>;
 // alias
 using SymGenerator = LoadGen<true, true>;
 using AsymGenerator = LoadGen<false, true>;
 using SymLoad = LoadGen<true, false>;
 using AsymLoad = LoadGen<false, false>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -14,31 +14,25 @@
 #include "../calculation_parameters.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Node final : public Base {
-   public:
+  public:
     using InputType = NodeInput;
-    template <bool sym>
-    using OutputType = NodeOutput<sym>;
+    template <bool sym> using OutputType = NodeOutput<sym>;
     using ShortCircuitOutputType = NodeShortCircuitOutput;
     static constexpr char const* name = "node";
-    constexpr ComponentType math_model_type() const final {
-        return ComponentType::node;
-    }
+    constexpr ComponentType math_model_type() const final { return ComponentType::node; }
 
-    explicit Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {
-    }
+    explicit Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {}
 
     // update node, nothing happens here
-    static constexpr UpdateChange update(BaseUpdate const&) {
-        return {false, false};
-    }
+    static constexpr UpdateChange update(BaseUpdate const&) { return {false, false}; }
 
     // energized
     template <bool sym>
     NodeOutput<sym> get_output(ComplexValue<sym> const& u_pu, ComplexValue<sym> const& bus_injection) const {
         NodeOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(true);
         output.u_pu = cabs(u_pu);
@@ -59,34 +53,29 @@
         return output;
     }
     NodeShortCircuitOutput get_sc_output(ComplexValue<true> const& u_pu) const {
         // Convert the input positive sequence voltage to phase voltage
         ComplexValue<false> const uabc_pu{u_pu};
         return get_sc_output(uabc_pu);
     }
-    template <bool sym>
-    NodeOutput<sym> get_null_output() const {
+    template <bool sym> NodeOutput<sym> get_null_output() const {
         NodeOutput<sym> output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
     NodeShortCircuitOutput get_null_sc_output() const {
         NodeShortCircuitOutput output{};
         static_cast<BaseOutput&>(output) = base_output(false);
         return output;
     }
 
-    constexpr double u_rated() const {
-        return u_rated_;
-    }
-    constexpr bool energized(bool is_connected_to_source) const final {
-        return is_connected_to_source;
-    }
+    constexpr double u_rated() const { return u_rated_; }
+    constexpr bool energized(bool is_connected_to_source) const final { return is_connected_to_source; }
 
-   private:
+  private:
     double u_rated_;
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,68 +12,56 @@
 #include "../enum.hpp"
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 
 namespace power_grid_model {
 
 class GenericPowerSensor : public Sensor {
-   public:
+  public:
     static constexpr char const* name = "generic_power_sensor";
 
     explicit GenericPowerSensor(GenericPowerSensorInput const& generic_power_sensor_input)
-        : Sensor{generic_power_sensor_input}, terminal_type_{generic_power_sensor_input.measured_terminal_type} {
-    }
+        : Sensor{generic_power_sensor_input}, terminal_type_{generic_power_sensor_input.measured_terminal_type} {}
 
-    MeasuredTerminalType get_terminal_type() const {
-        return terminal_type_;
-    }
+    MeasuredTerminalType get_terminal_type() const { return terminal_type_; }
 
-    template <bool sym>
-    PowerSensorOutput<sym> get_output(ComplexValue<sym> const& s) const {
+    template <bool sym> PowerSensorOutput<sym> get_output(ComplexValue<sym> const& s) const {
         if constexpr (sym) {
             return get_sym_output(s);
-        }
-        else {
+        } else {
             return get_asym_output(s);
         }
     }
 
-    template <bool sym>
-    PowerSensorOutput<sym> get_null_output() const {
-        return {{id(), false}, {}, {}};
-    }
+    template <bool sym> PowerSensorOutput<sym> get_null_output() const { return {{id(), false}, {}, {}}; }
 
-    SensorShortCircuitOutput get_null_sc_output() const {
-        return {{id(), false}};
-    }
+    SensorShortCircuitOutput get_null_sc_output() const { return {{id(), false}}; }
 
-   protected:
+  protected:
     double convert_direction() const {
         if (terminal_type_ == MeasuredTerminalType::load || terminal_type_ == MeasuredTerminalType::shunt) {
-            return -1.0;  // For shunt and load the direction in the math model is opposite to the direction in the
-                          // physical model
+            return -1.0; // For shunt and load the direction in the math model is opposite to the direction in the
+                         // physical model
         }
         return 1.0;
     }
 
-   private:
+  private:
     MeasuredTerminalType terminal_type_;
 
     virtual PowerSensorOutput<true> get_sym_output(ComplexValue<true> const& s) const = 0;
     virtual PowerSensorOutput<false> get_asym_output(ComplexValue<false> const& s) const = 0;
 };
 
-template <bool sym>
-class PowerSensor : public GenericPowerSensor {
-   public:
+template <bool sym> class PowerSensor : public GenericPowerSensor {
+  public:
     static constexpr char const* name = sym ? "sym_power_sensor" : "asym_power_sensor";
     using InputType = PowerSensorInput<sym>;
     using UpdateType = PowerSensorUpdate<sym>;
-    template <bool sym_calc>
-    using OutputType = PowerSensorOutput<sym_calc>;
+    template <bool sym_calc> using OutputType = PowerSensorOutput<sym_calc>;
 
     explicit PowerSensor(PowerSensorInput<sym> const& power_sensor_input)
         : GenericPowerSensor{power_sensor_input}, power_sigma_{power_sensor_input.power_sigma / base_power<sym>} {
         set_power(power_sensor_input.p_measured, power_sensor_input.q_measured);
     };
 
     UpdateChange update(PowerSensorUpdate<sym> const& power_sensor_update) {
@@ -81,15 +69,15 @@
 
         if (!is_nan(power_sensor_update.power_sigma)) {
             power_sigma_ = power_sensor_update.power_sigma / base_power<sym>;
         }
         return {false, false};
     }
 
-   private:
+  private:
     ComplexValue<sym> s_measured_{};
     double power_sigma_;
 
     void set_power(RealValue<sym> const& p_measured, RealValue<sym> const& q_measured) {
         double const scalar = convert_direction() / base_power<sym>;
         RealValue<sym> ps = real(s_measured_);
         RealValue<sym> qs = imag(s_measured_);
@@ -112,26 +100,25 @@
     }
     PowerSensorOutput<true> get_sym_output(ComplexValue<true> const& s) const final {
         return get_generic_output<true>(s);
     }
     PowerSensorOutput<false> get_asym_output(ComplexValue<false> const& s) const final {
         return get_generic_output<false>(s);
     }
-    template <bool sym_calc>
-    PowerSensorOutput<sym_calc> get_generic_output(ComplexValue<sym_calc> const& s) const {
+    template <bool sym_calc> PowerSensorOutput<sym_calc> get_generic_output(ComplexValue<sym_calc> const& s) const {
         PowerSensorOutput<sym_calc> output{};
         ComplexValue<sym_calc> const s_residual{process_mean_val<sym_calc>(s_measured_ - s) * convert_direction() *
                                                 base_power<sym_calc>};
         output.id = id();
-        output.energized = 1;  // power sensor is always energized
+        output.energized = 1; // power sensor is always energized
         output.p_residual = real(s_residual);
         output.q_residual = imag(s_residual);
         return output;
     }
 };
 
 using SymPowerSensor = PowerSensor<true>;
 using AsymPowerSensor = PowerSensor<false>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -15,38 +15,34 @@
 #include "../calculation_parameters.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Shunt : public Appliance {
-   public:
+  public:
     using InputType = ShuntInput;
     using UpdateType = ApplianceUpdate;
     static constexpr char const* name = "shunt";
-    ComponentType math_model_type() const final {
-        return ComponentType::shunt;
-    }
+    ComponentType math_model_type() const final { return ComponentType::shunt; }
 
     explicit Shunt(ShuntInput const& shunt_input, double u) : Appliance{shunt_input, u} {
         double const base_y = base_i() / (u / sqrt3);
         y1_ = (shunt_input.g1 + 1.0i * shunt_input.b1) / base_y;
         y0_ = (shunt_input.g0 + 1.0i * shunt_input.b0) / base_y;
     }
 
     // getter for calculation param, shunt y
-    template <bool sym>
-    ComplexTensor<sym> calc_param(bool is_connected_to_source = true) const {
+    template <bool sym> ComplexTensor<sym> calc_param(bool is_connected_to_source = true) const {
         if (!energized(is_connected_to_source)) {
             return ComplexTensor<sym>{};
         }
         if constexpr (sym) {
             return y1_;
-        }
-        else {
+        } else {
             // abc matrix
             // 1/3 *
             // [[2y1+y0, y0-y1, y0-y1],
             //  [y0-y1, 2y1+y0, y0-y1],
             //  [y0-y1, y0-y1, 2y1+y0]]
             return ComplexTensor<false>{(2.0 * y1_ + y0_) / 3.0, (y0_ - y1_) / 3.0};
         }
@@ -56,34 +52,27 @@
     UpdateChange update(ApplianceUpdate const& update) {
         assert(update.id == id());
         bool const changed = set_status(update.status);
         // change shunt connection will not change topology, but will change parameters
         return {false, changed};
     }
 
-   private:
+  private:
     DoubleComplex y1_, y0_;
 
-    template <bool sym_calc>
-    ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
+    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
         ApplianceMathOutput<sym_calc> appliance_math_output;
         ComplexTensor<sym_calc> const param = calc_param<sym_calc>();
         // return value should be injection direction, therefore a negative sign for i
         appliance_math_output.i = -dot(param, u);
         appliance_math_output.s = u * conj(appliance_math_output.i);
         return appliance_math_output;
     }
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final {
-        return u2si<true>(u);
-    }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final {
-        return u2si<false>(u);
-    }
+    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final { return u2si<true>(u); }
+    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final { return u2si<false>(u); }
 
-    double injection_direction() const final {
-        return -1.0;
-    }
+    double injection_direction() const final { return -1.0; }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,45 @@
 #include "../calculation_parameters.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Source : public Appliance {
-   public:
+  public:
     using InputType = SourceInput;
     using UpdateType = SourceUpdate;
     static constexpr char const* name = "source";
-    ComponentType math_model_type() const final {
-        return ComponentType::source;
-    }
+    ComponentType math_model_type() const final { return ComponentType::source; }
 
     explicit Source(SourceInput const& source_input, double u)
         : Appliance{source_input, u},
           u_ref_{source_input.u_ref},
           u_ref_angle_{is_nan(source_input.u_ref_angle) ? 0.0 : source_input.u_ref_angle} {
         double const sk{is_nan(source_input.sk) ? default_source_sk : source_input.sk};
         double const rx_ratio{is_nan(source_input.rx_ratio) ? default_source_rx_ratio : source_input.rx_ratio};
         double const z01_ratio{is_nan(source_input.z01_ratio) ? default_source_z01_ratio : source_input.z01_ratio};
         calculate_y_ref(sk, rx_ratio, z01_ratio);
     }
 
     // calculate y1 y0 ref
     void calculate_y_ref(double sk, double rx_ratio, double z01_ratio) {
-        double const z_abs = base_power_3p / sk;  // s_pu = s/base_s, z = u^2/s = 1/s = base_s/s_pu
+        double const z_abs = base_power_3p / sk; // s_pu = s/base_s, z = u^2/s = 1/s = base_s/s_pu
         double const x1 = z_abs / sqrt(rx_ratio * rx_ratio + 1.0);
         double const r1 = x1 * rx_ratio;
         y1_ref_ = 1.0 / DoubleComplex{r1, x1};
         y0_ref_ = y1_ref_ / z01_ratio;
     }
 
     // getter for calculation param, y_ref
-    template <bool sym>
-    ComplexTensor<sym> math_param() const {
+    template <bool sym> ComplexTensor<sym> math_param() const {
         // internal element_admittance
         if constexpr (sym) {
             return y1_ref_;
-        }
-        else {
+        } else {
             ComplexTensor<false> const sym_matrix = get_sym_matrix();
             ComplexTensor<false> const sym_matrix_inv = get_sym_matrix_inv();
             ComplexTensor<false> y012;
             y012 << y1_ref_, 0.0, 0.0, 0.0, y1_ref_, 0.0, 0.0, 0.0, y0_ref_;
             ComplexTensor<false> yabc = dot(sym_matrix, y012, sym_matrix_inv);
             return yabc;
         }
@@ -73,54 +69,44 @@
         if (!is_nan(new_u_ref_angle)) {
             u_ref_angle_ = new_u_ref_angle;
             changed = true;
         }
         return changed;
     }
     // getter for u_ref for calc_param
-    template <bool sym>
-    DoubleComplex calc_param() const {
-        return u_ref_ * std::exp(1.0i * u_ref_angle_);
-    }
+    template <bool sym> DoubleComplex calc_param() const { return u_ref_ * std::exp(1.0i * u_ref_angle_); }
 
     // update for source
     UpdateChange update(SourceUpdate const& update) {
         assert(update.id == id());
         bool const topo_changed = set_status(update.status);
         bool const param_changed = set_u_ref(update.u_ref, update.u_ref_angle);
         // change source connection will change both topo and param
         // change u ref will change param
         return {topo_changed, param_changed || topo_changed};
     }
 
-   private:
+  private:
     double u_ref_;
     double u_ref_angle_;
     // positive and zero sequence ref
     DoubleComplex y1_ref_{};
     DoubleComplex y0_ref_{};
 
-    template <bool sym_calc>
-    ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
+    template <bool sym_calc> ApplianceMathOutput<sym_calc> u2si(ComplexValue<sym_calc> const& u) const {
         ApplianceMathOutput<sym_calc> appliance_math_output;
         ComplexValue<sym_calc> const u_ref{u_ref_};
         ComplexTensor<sym_calc> const y_ref = math_param<sym_calc>();
         appliance_math_output.i = dot(y_ref, u_ref - u);
         appliance_math_output.s = u * conj(appliance_math_output.i);
         return appliance_math_output;
     }
 
-    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final {
-        return u2si<true>(u);
-    }
-    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final {
-        return u2si<false>(u);
-    }
+    ApplianceMathOutput<true> sym_u2si(ComplexValue<true> const& u) const final { return u2si<true>(u); }
+    ApplianceMathOutput<false> asym_u2si(ComplexValue<false> const& u) const final { return u2si<false>(u); }
 
-    double injection_direction() const final {
-        return 1.0;
-    }
+    double injection_direction() const final { return 1.0; }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #include "branch3.hpp"
 #include "transformer.hpp"
 #include "transformer_utils.hpp"
 
 namespace power_grid_model {
 
 class ThreeWindingTransformer : public Branch3 {
-   public:
+  public:
     using InputType = ThreeWindingTransformerInput;
     using UpdateType = ThreeWindingTransformerUpdate;
     static constexpr char const* name = "three_winding_transformer";
 
     explicit ThreeWindingTransformer(ThreeWindingTransformerInput const& three_winding_transformer_input,
                                      double u1_rated, double u2_rated, double u3_rated)
         : Branch3{three_winding_transformer_input},
@@ -92,33 +92,25 @@
         clock_12_ = static_cast<IntS>(clock_12_ % 12);
         clock_13_ = static_cast<IntS>(clock_13_ % 12);
         // check tap bounds
         tap_pos_ = tap_limit(tap_pos_);
     }
 
     // override getter
-    double base_i_1() const final {
-        return base_i_1_;
-    }
-    double base_i_2() const final {
-        return base_i_2_;
-    }
-    double base_i_3() const final {
-        return base_i_3_;
-    }
+    double base_i_1() const final { return base_i_1_; }
+    double base_i_2() const final { return base_i_2_; }
+    double base_i_3() const final { return base_i_3_; }
     double loading(double s_1, double s_2, double s_3) const final {
         return std::max(std::max(s_1 / sn_1_, s_2 / sn_2_), s_3 / sn_3_);
     }
     // 3-way branch, phase shift = phase_node_x - phase_internal_node
     // the clock_12 and clock_13 is reverted
     // because clock_12 is the phase shift node_1 - node_2
     // and the phase shift in the math model is node_x - node_internal
-    std::array<double, 3> phase_shift() const final {
-        return {0.0, -clock_12_ * deg_30, -clock_13_ * deg_30};
-    }
+    std::array<double, 3> phase_shift() const final { return {0.0, -clock_12_ * deg_30, -clock_13_ * deg_30}; }
 
     // setter
     bool set_tap(IntS new_tap) {
         if (new_tap == na_IntS || new_tap == tap_pos_) {
             return false;
         }
         tap_pos_ = tap_limit(new_tap);
@@ -128,15 +120,15 @@
     UpdateChange update(ThreeWindingTransformerUpdate const& update) {
         assert(update.id == id());
         bool const topo_changed = set_status(update.status_1, update.status_2, update.status_3);
         bool const param_changed = set_tap(update.tap_pos) || topo_changed;
         return {topo_changed, param_changed};
     }
 
-   private:
+  private:
     // three winding transformer parameters
     double u1_;
     double u2_;
     double u3_;
     double u1_rated_;
     double u2_rated_;
     double u3_rated_;
@@ -274,107 +266,105 @@
         // off nominal tap ratio
         auto const [u1, u2, u3] = [this]() {
             double result_u1 = u1_;
             double result_u2 = u2_;
             double result_u3 = u3_;
             if (tap_side_ == Branch3Side::side_1) {
                 result_u1 += tap_direction_ * (tap_pos_ - tap_nom_) * tap_size_;
-            }
-            else if (tap_side_ == Branch3Side::side_2) {
+            } else if (tap_side_ == Branch3Side::side_2) {
                 result_u2 += tap_direction_ * (tap_pos_ - tap_nom_) * tap_size_;
-            }
-            else {
+            } else {
                 result_u3 += tap_direction_ * (tap_pos_ - tap_nom_) * tap_size_;
             }
             return std::make_tuple(result_u1, result_u2, result_u3);
         }();
 
         auto const [uk_T1, uk_T2, uk_T3] = calculate_uk();
         auto const [pk_T1, pk_T2, pk_T3] = calculate_pk();
 
         TransformerInput const transformer_input_T1{
-            {{2}, 0, 1, static_cast<IntS>(status_1()), true},  // {{id}, from_node, to_node, from_status, to_status}
-            u1,                                                // u1
-            u1,                                                // u2
-            sn_1_,                                             // sn
-            uk_T1,                                             // uk
-            pk_T1,                                             // pk
-            i0_,                                               // i0
-            p0_,                                               // p0
-            WindingType::wye_n,                                // winding_from
-            WindingType::wye_n,                                // winding_to
-            0,                                                 // clock
-            BranchSide::from,                                  // tap_side
-            0,                                                 // tap_pos
-            0,                                                 // tap_min
-            0,                                                 // tap_max
-            0,                                                 // tap_nom
-            0.0,                                               // tap_size
-            nan,                                               // uk_min
-            nan,                                               // uk_max
-            nan,                                               // pk_min
-            nan,                                               // pk_max
-            z_grounding_1_.real(),                             // r_grounding_from
-            z_grounding_1_.imag(),                             // x_grounding_from
-            0,                                                 // r_grounding_to
-            0                                                  // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_1()), true}, // {{id}, from_node, to_node, from_status, to_status}
+            u1,                                               // u1
+            u1,                                               // u2
+            sn_1_,                                            // sn
+            uk_T1,                                            // uk
+            pk_T1,                                            // pk
+            i0_,                                              // i0
+            p0_,                                              // p0
+            WindingType::wye_n,                               // winding_from
+            WindingType::wye_n,                               // winding_to
+            0,                                                // clock
+            BranchSide::from,                                 // tap_side
+            0,                                                // tap_pos
+            0,                                                // tap_min
+            0,                                                // tap_max
+            0,                                                // tap_nom
+            0.0,                                              // tap_size
+            nan,                                              // uk_min
+            nan,                                              // uk_max
+            nan,                                              // pk_min
+            nan,                                              // pk_max
+            z_grounding_1_.real(),                            // r_grounding_from
+            z_grounding_1_.imag(),                            // x_grounding_from
+            0,                                                // r_grounding_to
+            0                                                 // x_grounding_to
         };
         TransformerInput const transformer_input_T2{
-            {{2}, 0, 1, static_cast<IntS>(status_2()), true},  // {{id}, from_node, to_node, from_status, to_status}
-            u2,                                                // u1
-            u1,                                                // u2
-            sn_2_,                                             // sn
-            uk_T2,                                             // uk
-            pk_T2,                                             // pk
-            0.0,                                               // i0
-            0.0,                                               // p0
-            winding_2_,                                        // winding_from
-            winding_1_,                                        // winding_to
-            static_cast<IntS>(12 - clock_12_),                 // clock, reversed
-            BranchSide::from,                                  // tap_side
-            0,                                                 // tap_pos
-            0,                                                 // tap_min
-            0,                                                 // tap_max
-            0,                                                 // tap_nom
-            0.0,                                               // tap_size
-            nan,                                               // uk_min
-            nan,                                               // uk_max
-            nan,                                               // pk_min
-            nan,                                               // pk_max
-            z_grounding_2_.real(),                             // r_grounding_from
-            z_grounding_2_.imag(),                             // x_grounding_from
-            0,                                                 // r_grounding_to
-            0                                                  // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_2()), true}, // {{id}, from_node, to_node, from_status, to_status}
+            u2,                                               // u1
+            u1,                                               // u2
+            sn_2_,                                            // sn
+            uk_T2,                                            // uk
+            pk_T2,                                            // pk
+            0.0,                                              // i0
+            0.0,                                              // p0
+            winding_2_,                                       // winding_from
+            winding_1_,                                       // winding_to
+            static_cast<IntS>(12 - clock_12_),                // clock, reversed
+            BranchSide::from,                                 // tap_side
+            0,                                                // tap_pos
+            0,                                                // tap_min
+            0,                                                // tap_max
+            0,                                                // tap_nom
+            0.0,                                              // tap_size
+            nan,                                              // uk_min
+            nan,                                              // uk_max
+            nan,                                              // pk_min
+            nan,                                              // pk_max
+            z_grounding_2_.real(),                            // r_grounding_from
+            z_grounding_2_.imag(),                            // x_grounding_from
+            0,                                                // r_grounding_to
+            0                                                 // x_grounding_to
         };
         TransformerInput const transformer_input_T3{
-            {{2}, 0, 1, static_cast<IntS>(status_3()), true},  // {{id}, from_node, to_node, from_status, to_status}
-            u3,                                                // u1
-            u1,                                                // u2
-            sn_3_,                                             // sn
-            uk_T3,                                             // uk
-            pk_T3,                                             // pk
-            0.0,                                               // i0
-            0.0,                                               // p0
-            winding_3_,                                        // winding_from
-            winding_1_,                                        // winding_to
-            static_cast<IntS>(12 - clock_13_),                 // clock, reversed
-            BranchSide::from,                                  // tap_side
-            0,                                                 // tap_pos
-            0,                                                 // tap_min
-            0,                                                 // tap_max
-            0,                                                 // tap_nom
-            0.0,                                               // tap_size
-            nan,                                               // uk_min
-            nan,                                               // uk_max
-            nan,                                               // pk_min
-            nan,                                               // pk_max
-            z_grounding_3_.real(),                             // r_grounding_from
-            z_grounding_3_.imag(),                             // x_grounding_from
-            0,                                                 // r_grounding_to
-            0                                                  // x_grounding_to
+            {{2}, 0, 1, static_cast<IntS>(status_3()), true}, // {{id}, from_node, to_node, from_status, to_status}
+            u3,                                               // u1
+            u1,                                               // u2
+            sn_3_,                                            // sn
+            uk_T3,                                            // uk
+            pk_T3,                                            // pk
+            0.0,                                              // i0
+            0.0,                                              // p0
+            winding_3_,                                       // winding_from
+            winding_1_,                                       // winding_to
+            static_cast<IntS>(12 - clock_13_),                // clock, reversed
+            BranchSide::from,                                 // tap_side
+            0,                                                // tap_pos
+            0,                                                // tap_min
+            0,                                                // tap_max
+            0,                                                // tap_nom
+            0.0,                                              // tap_size
+            nan,                                              // uk_min
+            nan,                                              // uk_max
+            nan,                                              // pk_min
+            nan,                                              // pk_max
+            z_grounding_3_.real(),                            // r_grounding_from
+            z_grounding_3_.imag(),                            // x_grounding_from
+            0,                                                // r_grounding_to
+            0                                                 // x_grounding_to
         };
 
         Transformer const T1{transformer_input_T1, u1_rated_, u1_rated_};
         Transformer const T2{transformer_input_T2, u2_rated_, u1_rated_};
         Transformer const T3{transformer_input_T3, u3_rated_, u1_rated_};
 
         return {T1, T2, T3};
@@ -395,10 +385,10 @@
         for (size_t i = 0; i < transformer_array.size(); i++) {
             transformer_params[i] = transformer_array[i].calc_param<false>();
         }
         return transformer_params;
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 class Transformer : public Branch {
-   public:
+  public:
     using InputType = TransformerInput;
     using UpdateType = TransformerUpdate;
     static constexpr char const* name = "transformer";
 
     explicit Transformer(TransformerInput const& transformer_input, double u1_rated, double u2_rated)
         : Branch{transformer_input},
           u1_{transformer_input.u1},
@@ -62,34 +62,22 @@
         // set clock to zero if it is 12
         clock_ = static_cast<IntS>(clock_ % 12);
         // check tap bounds
         tap_pos_ = tap_limit(tap_pos_);
     }
 
     // override getter
-    double base_i_from() const final {
-        return base_i_from_;
-    }
-    double base_i_to() const final {
-        return base_i_to_;
-    }
-    double loading(double max_s, double) const final {
-        return max_s / sn_;
-    };
+    double base_i_from() const final { return base_i_from_; }
+    double base_i_to() const final { return base_i_to_; }
+    double loading(double max_s, double) const final { return max_s / sn_; };
     // phase shift is theta_from - theta_to
-    double phase_shift() const final {
-        return clock_ * deg_30;
-    }
-    bool is_param_mutable() const final {
-        return true;
-    }
+    double phase_shift() const final { return clock_ * deg_30; }
+    bool is_param_mutable() const final { return true; }
     // get tap
-    IntS tap_pos() const {
-        return tap_pos_;
-    }
+    IntS tap_pos() const { return tap_pos_; }
     // setter
     bool set_tap(IntS new_tap) {
         if (new_tap == na_IntS || new_tap == tap_pos_) {
             return false;
         }
         tap_pos_ = tap_limit(new_tap);
         return true;
@@ -99,15 +87,15 @@
     UpdateChange update(TransformerUpdate const& update) {
         assert(update.id == id());
         bool const topo_changed = set_status(update.from_status, update.to_status);
         bool const param_changed = set_tap(update.tap_pos) || topo_changed;
         return {topo_changed, param_changed};
     }
 
-   private:
+  private:
     // transformer parameter
     double u1_;
     double u2_;
     double sn_;
     double tap_size_;
     double uk_;
     double pk_;
@@ -153,16 +141,15 @@
         double const base_y_to = base_i_to_ * base_i_to_ / base_power_1p;
         // off nominal tap ratio
         auto const [u1, u2] = [this]() {
             double result_u1 = u1_;
             double result_u2 = u2_;
             if (tap_side_ == BranchSide::from) {
                 result_u1 += tap_direction_ * (tap_pos_ - tap_nom_) * tap_size_;
-            }
-            else {
+            } else {
                 result_u2 += tap_direction_ * (tap_pos_ - tap_nom_) * tap_size_;
             }
             return std::pair{result_u1, result_u2};
         }();
         double const k = (u1 / u2) / nominal_ratio_;
         // pk and uk
         double const uk = tap_adjust_impedance(tap_pos_, tap_min_, tap_max_, tap_nom_, uk_, uk_min_, uk_max_);
@@ -189,16 +176,15 @@
         DoubleComplex y_shunt;
         // Y = I0_2 / (U2/sqrt(3)) = i0 * (S / sqrt(3) / U2) / (U2/sqrt(3)) = i0 * S * / U2 / U2
         double const y_shunt_abs = i0_ * sn_ / u2 / u2;
         // G = P0 / (U2^2)
         y_shunt.real(p0_ / u2 / u2);
         if (y_shunt.real() > y_shunt_abs) {
             y_shunt.imag(0.0);
-        }
-        else {
+        } else {
             y_shunt.imag(-std::sqrt(y_shunt_abs * y_shunt_abs - y_shunt.real() * y_shunt.real()));
         }
         // y shunt
         y_shunt = y_shunt / base_y_to;
         // return
         return std::make_tuple(y_series, y_shunt, k);
     }
@@ -263,10 +249,10 @@
             y012 << param0.value[i], 0.0, 0.0, 0.0, param1.value[i], 0.0, 0.0, 0.0, param2.value[i];
             param.value[i] = dot(sym_matrix, y012, sym_matrix_inv);
         }
         return param;
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     bool const correct_clock_winding = (clock_is_even == (is_from_wye == is_to_wye));
 
     return clock_in_range && correct_clock_winding;
 }
 
 // add tap
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,62 +14,53 @@
 #include "../three_phase_tensor.hpp"
 
 #include <limits>
 
 namespace power_grid_model {
 
 class GenericVoltageSensor : public Sensor {
-   public:
+  public:
     static constexpr char const* name = "generic_voltage_sensor";
 
     explicit GenericVoltageSensor(GenericVoltageSensorInput const& generic_voltage_sensor_input)
         : Sensor{generic_voltage_sensor_input} {};
 
-    template <bool sym>
-    VoltageSensorOutput<sym> get_output(ComplexValue<sym> const& u) const {
+    template <bool sym> VoltageSensorOutput<sym> get_output(ComplexValue<sym> const& u) const {
         if constexpr (sym) {
             assert(u != 0.0 + 0.0i);
             return get_sym_output(u);
-        }
-        else {
+        } else {
             assert(u[0] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(u[1] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(u[2] != 0.0 + 0.0i && "Voltage should not be 0.0 + 0.0i V");
             assert(abs(arg(u[0]) - arg(u[1])) > std::numeric_limits<double>::epsilon() &&
                    "Voltage angles should not be equal");
             assert(abs(arg(u[1]) - arg(u[2])) > std::numeric_limits<double>::epsilon() &&
                    "Voltage angles should not be equal");
             assert(abs(arg(u[2]) - arg(u[0])) > std::numeric_limits<double>::epsilon() &&
                    "Voltage angles should not be equal");
             return get_asym_output(u);
         }
     }
 
-    template <bool sym>
-    VoltageSensorOutput<sym> get_null_output() const {
-        return {{id(), false}, {}, {}};
-    }
+    template <bool sym> VoltageSensorOutput<sym> get_null_output() const { return {{id(), false}, {}, {}}; }
 
-    SensorShortCircuitOutput get_null_sc_output() const {
-        return {{id(), false}};
-    }
+    SensorShortCircuitOutput get_null_sc_output() const { return {{id(), false}}; }
 
-   private:
+  private:
     virtual VoltageSensorOutput<true> get_sym_output(ComplexValue<true> const& u) const = 0;
     virtual VoltageSensorOutput<false> get_asym_output(ComplexValue<false> const& u) const = 0;
 };
 
-template <bool sym>
-class VoltageSensor : public GenericVoltageSensor {
-   public:
+template <bool sym> class VoltageSensor : public GenericVoltageSensor {
+  public:
     static constexpr char const* name = sym ? "sym_voltage_sensor" : "asym_voltage_sensor";
     using InputType = VoltageSensorInput<sym>;
     using UpdateType = VoltageSensorUpdate<sym>;
-    template <bool sym_calc>
-    using OutputType = VoltageSensorOutput<sym_calc>;
+    template <bool sym_calc> using OutputType = VoltageSensorOutput<sym_calc>;
 
     explicit VoltageSensor(VoltageSensorInput<sym> const& voltage_sensor_input, double u_rated)
         : GenericVoltageSensor{voltage_sensor_input},
           u_rated_{u_rated},
           u_sigma_{voltage_sensor_input.u_sigma / (u_rated_ * u_scale<sym>)},
           u_measured_{voltage_sensor_input.u_measured / (u_rated_ * u_scale<sym>)},
           u_angle_measured_{voltage_sensor_input.u_angle_measured} {};
@@ -82,25 +73,24 @@
         if (!is_nan(voltage_sensor_update.u_sigma)) {
             u_sigma_ = voltage_sensor_update.u_sigma / (u_rated_ * u_scale<sym>);
         }
 
         return {false, false};
     }
 
-   private:
+  private:
     double u_rated_;
     double u_sigma_;
     RealValue<sym> u_measured_;
     RealValue<sym> u_angle_measured_;
 
     bool has_angle() const {
         if constexpr (sym) {
             return !is_nan(u_angle_measured_);
-        }
-        else {
+        } else {
             return !u_angle_measured_.isNaN().any();
         }
     }
 
     SensorCalcParam<true> sym_calc_param() const final {
         double const u_variance = u_sigma_ * u_sigma_;
         if (has_angle()) {
@@ -126,16 +116,15 @@
         value.id = id();
         value.energized = 1;
 
         DoubleComplex const u1_measured = sym_calc_param().value;
         bool const has_angle = !is_nan(imag(u1_measured));
         if (has_angle) {
             value.u_residual = (cabs(u1_measured) - cabs(u)) * u_rated_;
-        }
-        else {
+        } else {
             value.u_residual = (real(u1_measured) - cabs(u)) * u_rated_;
         }
         value.u_angle_residual = arg(u1_measured) - arg(u);
         return value;
     }
 
     VoltageSensorOutput<false> get_asym_output(ComplexValue<false> const& u) const final {
@@ -147,9 +136,9 @@
         return value;
     }
 };
 
 using SymVoltageSensor = VoltageSensor<true>;
 using AsymVoltageSensor = VoltageSensor<false>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -18,69 +18,62 @@
 #include <unordered_map>
 
 namespace power_grid_model {
 
 namespace container_impl {
 
 // get index of the first true in bool array
-template <size_t N>
-inline constexpr size_t get_index_bool_array(std::array<bool, N> arr, size_t idx = 0) {
+template <size_t N> inline constexpr size_t get_index_bool_array(std::array<bool, N> arr, size_t idx = 0) {
     if (idx == N) {
         return N;
     }
     if (arr[idx]) {
         return idx;
     }
     return get_index_bool_array(arr, idx + 1);
 }
 
-template <typename U, typename First, typename... Rest>
-constexpr size_t get_type_index() {
+template <typename U, typename First, typename... Rest> constexpr size_t get_type_index() {
     if constexpr (std::is_same_v<U, First>) {
         return 0;
-    }
-    else {
+    } else {
         return 1 + get_type_index<U, Rest...>();
     }
 }
 
 // get index of class in classes, with exact match
 template <class T, class... Ts>
 constexpr size_t get_cls_pos_v = get_index_bool_array(std::array{std::is_same_v<T, Ts>...});
 // get index of first (sub)-class in classes
 // the first match with sub class
 template <class T, class... Ts>
 constexpr size_t get_sub_cls_pos_v = get_index_bool_array(std::array{std::is_base_of_v<T, Ts>...});
 
 // define what types are retrievable using sequence number
-template <class... T>
-struct RetrievableTypes;
+template <class... T> struct RetrievableTypes;
 
 // container default declaration
-template <class... T>
-class Container;
+template <class... T> class Container;
 // real definition with retrievable types
 template <class... GettableTypes, class... StorageableTypes>
 class Container<RetrievableTypes<GettableTypes...>, StorageableTypes...> {
-   public:
+  public:
     static constexpr size_t num_storageable = sizeof...(StorageableTypes);
     static constexpr size_t num_gettable = sizeof...(GettableTypes);
 
     // default constructor, operator
 
     // reserve space
-    template <class Storageable>
-    void reserve(size_t size) {
+    template <class Storageable> void reserve(size_t size) {
         std::vector<Storageable>& vec = std::get<std::vector<Storageable>>(vectors_);
         vec.reserve(size);
     }
 
     // emplace component
-    template <class Storageable, class... Args>
-    void emplace(ID id, Args&&... args) {
+    template <class Storageable, class... Args> void emplace(ID id, Args&&... args) {
         // template<class... Args> Args&&... args perfect forwarding
         assert(!construction_complete_);
         // throw if id already exists
         if (map_.contains(id)) {
             throw ConflictID{id};
         }
         // find group and position
@@ -90,87 +83,77 @@
         // create object
         vec.emplace_back(std::forward<Args>(args)...);
         // insert idx to map
         map_[id] = Idx2D{group, pos};
     }
 
     // get item based on Idx2D
-    template <class Gettable>
-    Gettable& get_item(Idx2D idx_2d) {
+    template <class Gettable> Gettable& get_item(Idx2D idx_2d) {
         constexpr std::array<GetItemFuncPtr<Gettable>, num_storageable> func_arr{
             select_get_item_func_ptr<Gettable, StorageableTypes>::ptr...};
         // selected group should be de derived class of Gettable
         assert(is_base<Gettable>[idx_2d.group]);
         return (this->*(func_arr[idx_2d.group]))(idx_2d.pos);
     }
-    template <class Gettable>
-    Gettable const& get_item(Idx2D idx_2d) const {
+    template <class Gettable> Gettable const& get_item(Idx2D idx_2d) const {
         constexpr std::array<GetItemFuncPtrConst<Gettable>, num_storageable> func_arr{
             select_get_item_func_ptr<Gettable, StorageableTypes>::ptr_const...};
         // selected group should be de derived class of Gettable
         assert(is_base<Gettable>[idx_2d.group]);
         return (this->*(func_arr[idx_2d.group]))(idx_2d.pos);
     }
     // get idx by id
-    template <class Gettable = void>
-    Idx2D get_idx_by_id(ID id) const {
+    template <class Gettable = void> Idx2D get_idx_by_id(ID id) const {
         auto const found = map_.find(id);
         if (found == map_.end()) {
             throw IDNotFound{id};
         }
         if constexpr (!std::is_void_v<Gettable>) {
             if (!is_base<Gettable>[found->second.group]) {
                 throw IDWrongType{id};
             }
         }
         return found->second;
     }
     // get item based on ID
-    template <class Gettable>
-    Gettable& get_item(ID id) {
+    template <class Gettable> Gettable& get_item(ID id) {
         Idx2D const idx = get_idx_by_id<Gettable>(id);
         return get_item<Gettable>(idx);
     }
-    template <class Gettable>
-    Gettable const& get_item(ID id) const {
+    template <class Gettable> Gettable const& get_item(ID id) const {
         Idx2D const idx = get_idx_by_id<Gettable>(id);
         return get_item<Gettable>(idx);
     }
     // get item based on sequence
-    template <class Gettable>
-    Gettable& get_item_by_seq(Idx seq) {
+    template <class Gettable> Gettable& get_item_by_seq(Idx seq) {
         assert(construction_complete_);
         return get_item<Gettable>(get_idx_2d_by_seq<Gettable>(seq));
     }
-    template <class Gettable>
-    Gettable const& get_item_by_seq(Idx seq) const {
+    template <class Gettable> Gettable const& get_item_by_seq(Idx seq) const {
         assert(construction_complete_);
         return get_item<Gettable>(get_idx_2d_by_seq<Gettable>(seq));
     }
 
     // get size
-    template <class Gettable>
-    Idx size() const {
+    template <class Gettable> Idx size() const {
         assert(construction_complete_);
         return size_[get_cls_pos_v<Gettable, GettableTypes...>];
     }
 
     // get sequence idx based on id
-    template <class Gettable>
-    Idx get_seq(ID id) const {
+    template <class Gettable> Idx get_seq(ID id) const {
         assert(construction_complete_);
         std::array<Idx, num_storageable + 1> const& cum_size = cum_size_[get_cls_pos_v<Gettable, GettableTypes...>];
         auto const found = map_.find(id);
         assert(found != map_.end());
         return cum_size[found->second.group] + found->second.pos;
     }
 
     // get idx_2d based on sequence
-    template <class Gettable>
-    Idx2D get_idx_2d_by_seq(Idx seq) const {
+    template <class Gettable> Idx2D get_idx_2d_by_seq(Idx seq) const {
         assert(construction_complete_);
         assert(seq >= 0);
         std::array<Idx, num_storageable + 1> const& cum_size = cum_size_[get_cls_pos_v<Gettable, GettableTypes...>];
         auto const found = std::upper_bound(cum_size.begin(), cum_size.end(), seq);
         assert(found != cum_size.end());
         Idx2D res;
         res.group = static_cast<Idx>(std::distance(cum_size.cbegin(), found) - 1);
@@ -179,232 +162,194 @@
     }
 
     // get start idx based on two classes
     // the GettableBaseType specifies the iterator range of all components whish is subclass of GettableBaseType
     // the StorageableSubType specifies a subset of iterator range of GettableBaseType
     // the function returns the start index of the first StorageableSubType (or its subclass)
     //      in the iterator range of U
-    template <class GettableBaseType, class StorageableSubType>
-    Idx get_start_idx() const {
+    template <class GettableBaseType, class StorageableSubType> Idx get_start_idx() const {
         std::array<Idx, num_storageable + 1> const& cum_size =
             cum_size_[get_cls_pos_v<GettableBaseType, GettableTypes...>];
         return cum_size[get_sub_cls_pos_v<StorageableSubType, StorageableTypes...>];
     }
 
-    template <class Storageable>
-    Idx get_type_idx() const {
+    template <class Storageable> Idx get_type_idx() const {
         return static_cast<Idx>(get_type_index<Storageable, StorageableTypes...>());
     }
 
     void set_construction_complete() {
 #ifndef NDEBUG
         // set construction complete for debug assertions
         construction_complete_ = true;
-#endif  // !NDEBUG
+#endif // !NDEBUG
         size_ = {size_per_type<GettableTypes>()...};
         cum_size_ = {accumulate_size_per_vector<GettableTypes>()...};
     };
 
     // cache a Storagable item with index pos to restore to when restore_values() is called
-    template <class Storageable>
-    void cache_item(Idx pos) {
+    template <class Storageable> void cache_item(Idx pos) {
         const auto& value = get_raw<Storageable, Storageable>(pos);
         auto& cached_vec = std::get<std::vector<std::pair<Idx, Storageable>>>(cached_reset_values_);
 
         cached_vec.emplace_back(pos, value);
     }
 
-    void restore_values() {
-        (restore_values_impl<StorageableTypes>(), ...);
-    }
+    void restore_values() { (restore_values_impl<StorageableTypes>(), ...); }
 
-   private:
+  private:
     std::tuple<std::vector<StorageableTypes>...> vectors_;
     std::unordered_map<ID, Idx2D> map_;
     std::array<Idx, num_gettable> size_;
     std::array<std::array<Idx, num_storageable + 1>, num_gettable> cum_size_;
 
-    std::tuple<std::vector<std::pair<Idx, StorageableTypes>>...> cached_reset_values_;  // indices + reset values
+    std::tuple<std::vector<std::pair<Idx, StorageableTypes>>...> cached_reset_values_; // indices + reset values
 
 #ifndef NDEBUG
     // set construction_complete is used for debug assertions only
     bool construction_complete_{false};
-#endif  // !NDEBUG
+#endif // !NDEBUG
 
     // get item per type
     template <class GettableBaseType, class StorageableSubType>
-    requires std::derived_from<StorageableSubType, GettableBaseType> GettableBaseType& get_raw(Idx pos) {
+        requires std::derived_from<StorageableSubType, GettableBaseType>
+    GettableBaseType& get_raw(Idx pos) {
         return std::get<std::vector<StorageableSubType>>(vectors_)[pos];
     }
     template <class GettableBaseType, class StorageableSubType>
-    requires std::derived_from<StorageableSubType, GettableBaseType> GettableBaseType const& get_raw(Idx pos) const {
+        requires std::derived_from<StorageableSubType, GettableBaseType>
+    GettableBaseType const& get_raw(Idx pos) const {
         return std::get<std::vector<StorageableSubType>>(vectors_)[pos];
     }
 
     // templates to select function pointer
-    template <class Storageable>
-    using GetItemFuncPtr = Storageable& (Container::*)(Idx pos);
-    template <class Storageable>
-    using GetItemFuncPtrConst = Storageable const& (Container::*)(Idx pos) const;
-    template <class GettableBaseType, class StorageableSubType, class = void>
-    struct select_get_item_func_ptr {
+    template <class Storageable> using GetItemFuncPtr = Storageable& (Container::*)(Idx pos);
+    template <class Storageable> using GetItemFuncPtrConst = Storageable const& (Container::*)(Idx pos) const;
+    template <class GettableBaseType, class StorageableSubType, class = void> struct select_get_item_func_ptr {
         static constexpr GetItemFuncPtr<GettableBaseType> ptr = nullptr;
         static constexpr GetItemFuncPtrConst<GettableBaseType> ptr_const = nullptr;
     };
     template <class GettableBaseType, class StorageableSubType>
-    requires std::derived_from<StorageableSubType, GettableBaseType>
+        requires std::derived_from<StorageableSubType, GettableBaseType>
     struct select_get_item_func_ptr<GettableBaseType, StorageableSubType> {
         static constexpr GetItemFuncPtr<GettableBaseType> ptr =
             &Container::get_raw<GettableBaseType, StorageableSubType>;
         static constexpr GetItemFuncPtrConst<GettableBaseType> ptr_const =
             &Container::get_raw<GettableBaseType, StorageableSubType>;
     };
 
     // array of base judge
     template <class Gettable>
     static constexpr std::array<bool, num_storageable> is_base{std::is_base_of_v<Gettable, StorageableTypes>...};
     // array of relevant vector size, for a non-derived class, the size is zero
-    template <class Gettable>
-    std::array<Idx, num_storageable> size_per_vector() const {
+    template <class Gettable> std::array<Idx, num_storageable> size_per_vector() const {
         assert(construction_complete_);
         return std::array<Idx, num_storageable>{
             std::is_base_of_v<Gettable, StorageableTypes>
                 ? static_cast<Idx>(std::get<std::vector<StorageableTypes>>(vectors_).size())
                 : 0 ...};
     }
     // total size of a type
-    template <class Gettable>
-    Idx size_per_type() const {
+    template <class Gettable> Idx size_per_type() const {
         assert(construction_complete_);
         std::array<Idx, num_storageable> const size_vec = size_per_vector<Gettable>();
         return std::reduce(size_vec.begin(), size_vec.end(), Idx{});
     }
-    template <class Gettable>
-    std::array<Idx, num_storageable + 1> accumulate_size_per_vector() const {
+    template <class Gettable> std::array<Idx, num_storageable + 1> accumulate_size_per_vector() const {
         assert(construction_complete_);
         std::array<Idx, num_storageable> const size_vec = size_per_vector<Gettable>();
         std::array<Idx, num_storageable + 1> res{};
         std::inclusive_scan(size_vec.begin(), size_vec.end(), res.begin() + 1);
         return res;
     }
 
-    template <class Storageable>
-    void restore_values_impl() {
+    template <class Storageable> void restore_values_impl() {
         auto& cached_vec = std::get<std::vector<std::pair<Idx, Storageable>>>(cached_reset_values_);
         for (auto it = cached_vec.crbegin(); it != cached_vec.crend(); ++it) {
             auto const& cache = *it;
             get_raw<Storageable, Storageable>(cache.first) = cache.second;
         }
         cached_vec.clear();
     }
 
     // define iterator
     template <class Gettable>
     class Iterator : public boost::iterator_facade<Iterator<Gettable>, Gettable, boost::random_access_traversal_tag,
                                                    Gettable&, Idx> {
-       public:
+      public:
         static constexpr bool is_const = std::is_const_v<Gettable>;
         using base_type = std::remove_cv_t<Gettable>;
         using container_type = std::conditional_t<is_const, Container const, Container>;
         // constructor including default
         explicit Iterator(container_type* container_ptr = nullptr, Idx idx = 0)
-            : container_ptr_{container_ptr}, idx_{idx} {
-        }
+            : container_ptr_{container_ptr}, idx_{idx} {}
         // conversion to const iterator
         template <class ConstGettable = Gettable>
-        requires(!is_const) explicit operator Iterator<ConstGettable const>() const {
+            requires(!is_const)
+        explicit operator Iterator<ConstGettable const>() const {
             return Iterator<ConstGettable const>{container_ptr_, idx_};
         }
 
-       private:
+      private:
         friend class boost::iterator_core_access;
 
-        Gettable& dereference() const {
-            return container_ptr_->template get_item_by_seq<base_type>(idx_);
-        }
+        Gettable& dereference() const { return container_ptr_->template get_item_by_seq<base_type>(idx_); }
         bool equal(Iterator const& other) const {
             assert(container_ptr_ == other.container_ptr_);
             return idx_ == other.idx_;
         }
-        void increment() {
-            ++idx_;
-        }
-        void decrement() {
-            --idx_;
-        }
-        void advance(Idx n) {
-            idx_ += n;
-        }
+        void increment() { ++idx_; }
+        void decrement() { --idx_; }
+        void advance(Idx n) { idx_ += n; }
         Idx distance_to(Iterator const& other) const {
             assert(container_ptr_ == other.container_ptr_);
             return other.idx_ - idx_;
         }
         // store container pointer
         // and idx
         container_type* container_ptr_;
         Idx idx_;
     };
 
     // define proxy
-    template <class Gettable>
-    class Proxy {
-       private:
+    template <class Gettable> class Proxy {
+      private:
         static constexpr bool is_const = std::is_const_v<Gettable>;
         using base_type = std::remove_cv_t<Gettable>;
         using container_type = std::conditional_t<is_const, Container const, Container>;
 
-       public:
+      public:
         explicit Proxy(container_type& container)
-            : begin_{&container, 0}, end_{&container, container.template size<base_type>()} {
-        }
-        Iterator<Gettable> begin() {
-            return begin_;
-        }
-        Iterator<Gettable> end() {
-            return end_;
-        }
+            : begin_{&container, 0}, end_{&container, container.template size<base_type>()} {}
+        Iterator<Gettable> begin() { return begin_; }
+        Iterator<Gettable> end() { return end_; }
 
-       private:
+      private:
         Iterator<Gettable> const begin_;
         Iterator<Gettable> const end_;
     };
 
-   public:
-    template <class Gettable>
-    Proxy<Gettable> iter() {
-        return Proxy<Gettable>{*this};
-    }
-    template <class Gettable>
-    Proxy<Gettable const> iter() const {
-        return Proxy<Gettable const>{*this};
-    }
-    template <class Gettable>
-    Proxy<Gettable const> citer() const {
-        return iter<Gettable>();
-    }
+  public:
+    template <class Gettable> Proxy<Gettable> iter() { return Proxy<Gettable>{*this}; }
+    template <class Gettable> Proxy<Gettable const> iter() const { return Proxy<Gettable const>{*this}; }
+    template <class Gettable> Proxy<Gettable const> citer() const { return iter<Gettable>(); }
 };
 
 // type traits to instantiate container
-template <class... T>
-struct ExtraRetrievableTypes;
+template <class... T> struct ExtraRetrievableTypes;
 // with no extra types, default all vector value types
-template <class... T>
-struct container_trait {
+template <class... T> struct container_trait {
     using type = Container<RetrievableTypes<T...>, T...>;
 };
 // if extra types are provided, also add to the retrievable types
-template <class... TR, class... T>
-struct container_trait<ExtraRetrievableTypes<TR...>, T...> {
+template <class... TR, class... T> struct container_trait<ExtraRetrievableTypes<TR...>, T...> {
     using type = Container<RetrievableTypes<T..., TR...>, T...>;
 };
 
-}  // namespace container_impl
+} // namespace container_impl
 
-template <class... T>
-using ExtraRetrievableTypes = container_impl::ExtraRetrievableTypes<T...>;
+template <class... T> using ExtraRetrievableTypes = container_impl::ExtraRetrievableTypes<T...>;
 
-template <class... T>
-using Container = typename container_impl::container_trait<T...>::type;
+template <class... T> using Container = typename container_impl::container_trait<T...>::type;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #define POWER_GRID_MODEL_ENUM_HPP
 
 #include "power_grid_model.hpp"
 
 namespace power_grid_model {
 
 enum class LoadGenType : IntS {
-    const_pq = 0,  // constant power
-    const_y = 1,   // constant element_admittance (impedance)
-    const_i = 2,   // constant current
+    const_pq = 0, // constant power
+    const_y = 1,  // constant element_admittance (impedance)
+    const_i = 2,  // constant current
 };
 
 enum class WindingType : IntS { wye = 0, wye_n = 1, delta = 2, zigzag = 3, zigzag_n = 4 };
 
 enum class BranchSide : IntS { from = 0, to = 1 };
 
 enum class Branch3Side : IntS { side_1 = 0, side_2 = 1, side_3 = 2 };
@@ -92,10 +92,10 @@
     bc = 6,
     default_value = -1,
     nan = na_IntS
 };
 
 enum class CType : IntS { c_int32 = 0, c_int8 = 1, c_double = 2, c_double3 = 3 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -11,70 +11,65 @@
 
 #include <exception>
 #include <string>
 
 namespace power_grid_model {
 
 class PowerGridError : public std::exception {
-   public:
-    void append_msg(std::string const &msg) {
-        msg_ += msg;
-    }
-    char const *what() const noexcept final {
-        return msg_.c_str();
-    }
+  public:
+    void append_msg(std::string const& msg) { msg_ += msg; }
+    char const* what() const noexcept final { return msg_.c_str(); }
 
-   private:
+  private:
     std::string msg_;
 };
 
-template <typename T>
-class MissingCaseForEnumError : public PowerGridError {
-   public:
-    MissingCaseForEnumError(const std::string &method, const T &value) {
+template <typename T> class MissingCaseForEnumError : public PowerGridError {
+  public:
+    MissingCaseForEnumError(const std::string& method, const T& value) {
         append_msg(method + " is not implemented for " + typeid(T).name() + " #" + std::to_string(IntS(value)) + "!\n");
     }
 };
 
 class ConflictVoltage : public PowerGridError {
-   public:
+  public:
     ConflictVoltage(ID id, ID id1, ID id2, double u1, double u2) {
         append_msg("Conflicting voltage for line " + std::to_string(id) + "\n voltage at from node " +
                    std::to_string(id1) + " is " + std::to_string(u1) + "\n voltage at to node " + std::to_string(id2) +
                    " is " + std::to_string(u2) + '\n');
     }
 };
 
 class InvalidBranch : public PowerGridError {
-   public:
+  public:
     InvalidBranch(ID branch_id, ID node_id) {
         append_msg("Branch " + std::to_string(branch_id) + " has the same from- and to-node " +
                    std::to_string(node_id) + ",\n This is not allowed!\n");
     }
 };
 
 class InvalidBranch3 : public PowerGridError {
-   public:
+  public:
     InvalidBranch3(ID branch3_id, ID node_1_id, ID node_2_id, ID node_3_id) {
         append_msg("Branch3 " + std::to_string(branch3_id) +
                    " is connected to the same node at least twice. Node 1/2/3: " + std::to_string(node_1_id) + "/" +
                    std::to_string(node_2_id) + "/" + std::to_string(node_3_id) + ",\n This is not allowed!\n");
     }
 };
 
 class InvalidTransformerClock : public PowerGridError {
-   public:
+  public:
     InvalidTransformerClock(ID id, IntS clock) {
         append_msg("Invalid clock for transformer " + std::to_string(id) + ", clock  " + std::to_string(clock) + '\n');
     }
 };
 
 class SparseMatrixError : public PowerGridError {
-   public:
-    SparseMatrixError(Idx err, std::string const &msg = "") {
+  public:
+    SparseMatrixError(Idx err, std::string const& msg = "") {
         append_msg("Sparse matrix error with error code #" + std::to_string(err) + " (possibly singular)\n");
         if (!msg.empty()) {
             append_msg(msg + "\n");
         }
         append_msg("If you get this error from state estimation, ");
         append_msg("it usually means the system is not fully observable, i.e. not enough measurements.");
     }
@@ -82,113 +77,99 @@
         append_msg("Sparse matrix error, possibly singular matrix!\n" +
                    std::string("If you get this error from state estimation, ") +
                    "it usually means the system is not fully observable, i.e. not enough measurements.");
     }
 };
 
 class IterationDiverge : public PowerGridError {
-   public:
+  public:
     IterationDiverge(Idx num_iter, double max_dev, double err_tol) {
         append_msg("Iteration failed to converge after " + std::to_string(num_iter) + " iterations! Max deviation: " +
                    std::to_string(max_dev) + ", error tolerance: " + std::to_string(err_tol) + ".\n");
     }
 };
 
 class ConflictID : public PowerGridError {
-   public:
-    explicit ConflictID(ID id) {
-        append_msg("Conflicting id detected: " + std::to_string(id) + '\n');
-    }
+  public:
+    explicit ConflictID(ID id) { append_msg("Conflicting id detected: " + std::to_string(id) + '\n'); }
 };
 
 class IDNotFound : public PowerGridError {
-   public:
-    explicit IDNotFound(ID id) {
-        append_msg("The id cannot be found: " + std::to_string(id) + '\n');
-    }
+  public:
+    explicit IDNotFound(ID id) { append_msg("The id cannot be found: " + std::to_string(id) + '\n'); }
 };
 
 class InvalidMeasuredObject : public PowerGridError {
-   public:
-    InvalidMeasuredObject(const std::string &object, const std::string &sensor) {
+  public:
+    InvalidMeasuredObject(const std::string& object, const std::string& sensor) {
         append_msg(sensor + " is not supported for " + object);
     }
 };
 
 class IDWrongType : public PowerGridError {
-   public:
-    explicit IDWrongType(ID id) {
-        append_msg("Wrong type for object with id " + std::to_string(id) + '\n');
-    }
+  public:
+    explicit IDWrongType(ID id) { append_msg("Wrong type for object with id " + std::to_string(id) + '\n'); }
 };
 
 class CalculationError : public PowerGridError {
-   public:
-    explicit CalculationError(std::string const &msg) {
-        append_msg(msg);
-    }
+  public:
+    explicit CalculationError(std::string const& msg) { append_msg(msg); }
 };
 
 class BatchCalculationError : public CalculationError {
-   public:
-    BatchCalculationError(std::string const &msg, IdxVector const &failed_scenarios,
-                          std::vector<std::string> const &err_msgs)
-        : CalculationError(msg), failed_scenarios_{failed_scenarios}, err_msgs_(err_msgs) {
-    }
+  public:
+    BatchCalculationError(std::string const& msg, IdxVector const& failed_scenarios,
+                          std::vector<std::string> const& err_msgs)
+        : CalculationError(msg), failed_scenarios_{failed_scenarios}, err_msgs_(err_msgs) {}
 
-    IdxVector const &failed_scenarios() const {
-        return failed_scenarios_;
-    }
+    IdxVector const& failed_scenarios() const { return failed_scenarios_; }
 
-    std::vector<std::string> const &err_msgs() const {
-        return err_msgs_;
-    }
+    std::vector<std::string> const& err_msgs() const { return err_msgs_; }
 
-   private:
+  private:
     IdxVector failed_scenarios_;
     std::vector<std::string> err_msgs_;
 };
 
 class InvalidCalculationMethod : public CalculationError {
-   public:
-    InvalidCalculationMethod() : CalculationError("The calculation method is invalid for this calculation!") {
-    }
+  public:
+    InvalidCalculationMethod() : CalculationError("The calculation method is invalid for this calculation!") {}
 };
 
 class UnknownAttributeName : public PowerGridError {
-   public:
-    explicit UnknownAttributeName(std::string const &attr_name) {
+  public:
+    explicit UnknownAttributeName(std::string const& attr_name) {
         append_msg("Unknown attribute name!" + attr_name + "\n");
     }
 };
 
 class InvalidShortCircuitType : public PowerGridError {
-   public:
+  public:
     explicit InvalidShortCircuitType(FaultType short_circuit_type) {
         append_msg("The short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
                    ") is invalid!\n");
     }
     InvalidShortCircuitType(bool sym, FaultType short_circuit_type) {
         append_msg("The short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
                    ") does not match the calculation type (symmetric=" + std::to_string(sym) + ")\n");
     }
 };
 
 class InvalidShortCircuitPhases : public PowerGridError {
-   public:
+  public:
     InvalidShortCircuitPhases(FaultType short_circuit_type, FaultPhase short_circuit_phases) {
         append_msg("The short circuit phases (" + std::to_string(static_cast<IntS>(short_circuit_phases)) +
                    ") do not match the short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
                    ")\n");
     }
 };
 
 class InvalidShortCircuitPhaseOrType : public PowerGridError {
-   public:
+  public:
     InvalidShortCircuitPhaseOrType() {
         append_msg("During one calculation the short circuit types phases should be similar for all faults \n");
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,98 +12,91 @@
 
 namespace power_grid_model::main_core {
 
 // template to construct components
 // using forward interators
 // different selection based on component type
 template <std::derived_from<Base> Component, class ComponentContainer, std::forward_iterator ForwardIterator>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 void add_component(MainModelState<ComponentContainer>& state, ForwardIterator begin, ForwardIterator end,
                    double system_frequency) {
     size_t const size = std::distance(begin, end);
     state.components.template reserve<Component>(size);
     // loop to add component
     for (auto it = begin; it != end; ++it) {
         auto const& input = *it;
         ID const id = input.id;
         // construct based on type of component
         if constexpr (std::derived_from<Component, Node>) {
             state.components.template emplace<Component>(id, input);
-        }
-        else if constexpr (std::derived_from<Component, Branch>) {
+        } else if constexpr (std::derived_from<Component, Branch>) {
             double const u1 = state.components.template get_item<Node>(input.from_node).u_rated();
             double const u2 = state.components.template get_item<Node>(input.to_node).u_rated();
             // set system frequency for line
             if constexpr (std::same_as<Component, Line>) {
                 state.components.template emplace<Component>(id, input, system_frequency, u1, u2);
-            }
-            else {
+            } else {
                 state.components.template emplace<Component>(id, input, u1, u2);
             }
-        }
-        else if constexpr (std::derived_from<Component, Branch3>) {
+        } else if constexpr (std::derived_from<Component, Branch3>) {
             double const u1 = state.components.template get_item<Node>(input.node_1).u_rated();
             double const u2 = state.components.template get_item<Node>(input.node_2).u_rated();
             double const u3 = state.components.template get_item<Node>(input.node_3).u_rated();
             state.components.template emplace<Component>(id, input, u1, u2, u3);
-        }
-        else if constexpr (std::derived_from<Component, Appliance>) {
+        } else if constexpr (std::derived_from<Component, Appliance>) {
             double const u = state.components.template get_item<Node>(input.node).u_rated();
             state.components.template emplace<Component>(id, input, u);
-        }
-        else if constexpr (std::derived_from<Component, GenericVoltageSensor>) {
+        } else if constexpr (std::derived_from<Component, GenericVoltageSensor>) {
             double const u = state.components.template get_item<Node>(input.measured_object).u_rated();
             state.components.template emplace<Component>(id, input, u);
-        }
-        else if constexpr (std::derived_from<Component, GenericPowerSensor>) {
+        } else if constexpr (std::derived_from<Component, GenericPowerSensor>) {
             // it is not allowed to place a sensor at a link
             if (state.components.get_idx_by_id(input.measured_object).group ==
                 state.components.template get_type_idx<Link>()) {
                 throw InvalidMeasuredObject("Link", "PowerSensor");
             }
             ID const measured_object = input.measured_object;
             // check correctness of measured component type based on measured terminal type
             switch (input.measured_terminal_type) {
                 using enum MeasuredTerminalType;
 
-                case branch_from:
-                case branch_to:
-                    state.components.template get_item<Branch>(measured_object);
-                    break;
-                case branch3_1:
-                case branch3_2:
-                case branch3_3:
-                    state.components.template get_item<Branch3>(measured_object);
-                    break;
-                case shunt:
-                    state.components.template get_item<Shunt>(measured_object);
-                    break;
-                case source:
-                    state.components.template get_item<Source>(measured_object);
-                    break;
-                case load:
-                    state.components.template get_item<GenericLoad>(measured_object);
-                    break;
-                case generator:
-                    state.components.template get_item<GenericGenerator>(measured_object);
-                    break;
-                case node:
-                    state.components.template get_item<Node>(measured_object);
-                    break;
-                default:
-                    throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " item retrieval",
-                                                  input.measured_terminal_type);
+            case branch_from:
+            case branch_to:
+                state.components.template get_item<Branch>(measured_object);
+                break;
+            case branch3_1:
+            case branch3_2:
+            case branch3_3:
+                state.components.template get_item<Branch3>(measured_object);
+                break;
+            case shunt:
+                state.components.template get_item<Shunt>(measured_object);
+                break;
+            case source:
+                state.components.template get_item<Source>(measured_object);
+                break;
+            case load:
+                state.components.template get_item<GenericLoad>(measured_object);
+                break;
+            case generator:
+                state.components.template get_item<GenericGenerator>(measured_object);
+                break;
+            case node:
+                state.components.template get_item<Node>(measured_object);
+                break;
+            default:
+                throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " item retrieval",
+                                              input.measured_terminal_type);
             }
 
             state.components.template emplace<Component>(id, input);
-        }
-        else if constexpr (std::derived_from<Component, Fault>) {
+        } else if constexpr (std::derived_from<Component, Fault>) {
             // check that fault object exists (currently, only faults at nodes are supported)
             state.components.template get_item<Node>(input.fault_object);
             state.components.template emplace<Component>(id, input);
         }
     }
 }
 
-}  // namespace power_grid_model::main_core
+} // namespace power_grid_model::main_core
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -11,152 +11,153 @@
 #include "../all_components.hpp"
 
 namespace power_grid_model::main_core {
 
 namespace detail {
 
 template <std::derived_from<Base> BaseComponent, std::derived_from<Base> Component, class ComponentContainer>
-requires std::derived_from<Component, BaseComponent> &&
-    model_component_state<MainModelState, ComponentContainer, Component>
+    requires std::derived_from<Component, BaseComponent> &&
+             model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_sequence_offset(MainModelState<ComponentContainer> const& state) {
     return state.components.template get_start_idx<BaseComponent, Component>();
 }
 
 template <std::same_as<Node> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->node.cbegin();
 }
 
 template <std::derived_from<Branch> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->branch.cbegin() + comp_sequence_offset<Branch, Component>(state);
 }
 
 template <std::derived_from<Branch3> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->branch3.cbegin() + comp_sequence_offset<Branch3, Component>(state);
 }
 
 template <std::same_as<Source> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->source.cbegin();
 }
 
 template <std::derived_from<GenericLoadGen> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->load_gen.cbegin() + comp_sequence_offset<GenericLoadGen, Component>(state);
 }
 
 template <std::same_as<Shunt> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.topo_comp_coup->shunt.cbegin();
 }
 
 template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.comp_topo->voltage_sensor_node_idx.cbegin() +
            comp_sequence_offset<GenericVoltageSensor, Component>(state);
 }
 
 template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.comp_topo->power_sensor_object_idx.cbegin() +
            comp_sequence_offset<GenericPowerSensor, Component>(state);
 }
 
 template <std::same_as<Fault> Component, class ComponentContainer>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr auto comp_base_sequence_cbegin(MainModelState<ComponentContainer> const& state) {
     return state.comp_coup.fault.cbegin();
 }
 
 template <typename Component, typename IndexType, class ComponentContainer, std::forward_iterator ResIt,
           typename ResFunc>
-requires model_component_state<MainModelState, ComponentContainer, Component> &&
-    std::invocable<std::remove_cvref_t<ResFunc>, Component const&, IndexType>&&
-        std::convertible_to<std::invoke_result_t<ResFunc, Component const&, IndexType>, std::iter_value_t<ResIt>>&&
-            std::convertible_to<IndexType, decltype(*comp_base_sequence_cbegin<Component>(
-                                               MainModelState<ComponentContainer>{}))> constexpr ResIt
-            produce_output(MainModelState<ComponentContainer> const& state, ResIt res_it, ResFunc&& func) {
+    requires model_component_state<MainModelState, ComponentContainer, Component> &&
+             std::invocable<std::remove_cvref_t<ResFunc>, Component const&, IndexType> &&
+             std::convertible_to<std::invoke_result_t<ResFunc, Component const&, IndexType>,
+                                 std::iter_value_t<ResIt>> &&
+             std::convertible_to<IndexType,
+                                 decltype(*comp_base_sequence_cbegin<Component>(MainModelState<ComponentContainer>{}))>
+constexpr ResIt produce_output(MainModelState<ComponentContainer> const& state, ResIt res_it, ResFunc&& func) {
     return std::transform(state.components.template citer<Component>().begin(),
                           state.components.template citer<Component>().end(),
                           comp_base_sequence_cbegin<Component>(state), res_it, func);
 }
 
-}  // namespace detail
+} // namespace detail
 
 // output node
 template <std::same_as<Node> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Node, Idx2D>(state, res_it, [&math_output](Node const& node, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return node.get_null_output<sym>();
         }
         return node.get_output<sym>(math_output[math_id.group].u[math_id.pos],
                                     math_output[math_id.group].bus_injection[math_id.pos]);
     });
 }
 template <std::same_as<Node> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Node, Idx2D>(state, res_it, [&math_output](Node const& node, Idx2D math_id) {
         if (math_id.group == -1) {
             return node.get_null_sc_output();
         }
         return node.get_sc_output(math_output[math_id.group].u_bus[math_id.pos]);
     });
 }
 
 // output branch
 template <std::derived_from<Branch> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Branch const& branch, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return branch.get_null_output<sym>();
         }
         return branch.get_output<sym>(math_output[math_id.group].branch[math_id.pos]);
     });
 }
 template <std::derived_from<Branch> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Branch const& branch, Idx2D math_id) {
         if (math_id.group == -1) {
             return branch.get_null_sc_output();
         }
         return branch.get_sc_output(math_output[math_id.group].branch[math_id.pos]);
     });
 }
 
 // output branch3
 template <std::derived_from<Branch3> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2DBranch3>(
         state, res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             if (math_id.group == -1) {
@@ -166,15 +167,15 @@
             auto const& branches = math_output[math_id.group].branch;
             return branch3.get_output<sym>(branches[math_id.pos[0]], branches[math_id.pos[1]],
                                            branches[math_id.pos[2]]);
         });
 }
 template <std::derived_from<Branch3> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2DBranch3>(
         state, res_it, [&math_output](Branch3 const& branch3, Idx2DBranch3 math_id) {
             if (math_id.group == -1) {
                 return branch3.get_null_sc_output();
             }
@@ -183,110 +184,109 @@
             return branch3.get_sc_output(branches[math_id.pos[0]], branches[math_id.pos[1]], branches[math_id.pos[2]]);
         });
 }
 
 // output source, load_gen, shunt individually
 template <std::same_as<Appliance> Component, class ComponentContainer, math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     res_it = output_result<Source>(state, math_output, res_it);
     res_it = output_result<GenericLoadGen>(state, math_output, res_it);
     res_it = output_result<Shunt>(state, math_output, res_it);
     return res_it;
 }
 
 // output source
 template <std::same_as<Source> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Source const& source, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return source.get_null_output<sym>();
         }
         return source.get_output<sym>(math_output[math_id.group].source[math_id.pos]);
     });
 }
 template <std::same_as<Source> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Source const& source, Idx2D math_id) {
         if (math_id.group == -1) {
             return source.get_null_sc_output();
         }
         return source.get_sc_output(math_output[math_id.group].source[math_id.pos]);
     });
 }
 
 // output load gen
 template <std::derived_from<GenericLoadGen> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(
         state, res_it, [&math_output](GenericLoadGen const& load_gen, Idx2D math_id) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             if (math_id.group == -1) {
                 return load_gen.get_null_output<sym>();
             }
             return load_gen.get_output<sym>(math_output[math_id.group].load_gen[math_id.pos]);
         });
 }
 template <std::derived_from<GenericLoadGen> Component, class ComponentContainer,
           short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
-    return detail::produce_output<Component, Idx2D>(state, res_it,
-                                                    [](GenericLoadGen const& load_gen, Idx2D /* math_id */) {
-                                                        return load_gen.get_null_sc_output();
-                                                    });
+    return detail::produce_output<Component, Idx2D>(
+        state, res_it,
+        [](GenericLoadGen const& load_gen, Idx2D /* math_id */) { return load_gen.get_null_sc_output(); });
 }
 
 // output shunt
 template <std::same_as<Shunt> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Shunt const& shunt, Idx2D math_id) {
         constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
         if (math_id.group == -1) {
             return shunt.get_null_output<sym>();
         }
         return shunt.get_output<sym>(math_output[math_id.group].shunt[math_id.pos]);
     });
 }
 template <std::same_as<Shunt> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(state, res_it, [&math_output](Shunt const& shunt, Idx2D math_id) {
         if (math_id.group == -1) {
             return shunt.get_null_sc_output();
         }
         return shunt.get_sc_output(math_output[math_id.group].shunt[math_id.pos]);
     });
 }
 
 // output voltage sensor
 template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericVoltageSensor const& voltage_sensor, Idx const node_seq) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             Idx2D const node_math_id = state.topo_comp_coup->node[node_seq];
@@ -294,130 +294,129 @@
                 return voltage_sensor.get_null_output<sym>();
             }
             return voltage_sensor.get_output<sym>(math_output[node_math_id.group].u[node_math_id.pos]);
         });
 }
 template <std::derived_from<GenericVoltageSensor> Component, class ComponentContainer,
           short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [](GenericVoltageSensor const& voltage_sensor, Idx const /* node_seq */) {
             return voltage_sensor.get_null_sc_output();
         });
 }
 
 // output power sensor
 template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer,
           steady_state_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx>(
         state, res_it, [&state, &math_output](GenericPowerSensor const& power_sensor, Idx const obj_seq) {
             constexpr auto sym = symmetric_math_output_type<MathOutputType>;
 
             auto const terminal_type = power_sensor.get_terminal_type();
             Idx2D const obj_math_id = [&]() {
                 switch (terminal_type) {
                     using enum MeasuredTerminalType;
 
-                    case branch_from:
-                    case branch_to:
-                        return state.topo_comp_coup->branch[obj_seq];
-                    case source:
-                        return state.topo_comp_coup->source[obj_seq];
-                    case shunt:
-                        return state.topo_comp_coup->shunt[obj_seq];
-                    case load:
-                    case generator:
-                        return state.topo_comp_coup->load_gen[obj_seq];
-                    // from branch3, get relevant math object branch based on the measured side
-                    case branch3_1:
-                        return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
-                                     state.topo_comp_coup->branch3[obj_seq].pos[0]};
-                    case branch3_2:
-                        return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
-                                     state.topo_comp_coup->branch3[obj_seq].pos[1]};
-                    case branch3_3:
-                        return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
-                                     state.topo_comp_coup->branch3[obj_seq].pos[2]};
-                    case node:
-                        return state.topo_comp_coup->node[obj_seq];
-                    default:
-                        throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
-                                                      terminal_type);
-                }
-            }();
-
-            if (obj_math_id.group == -1) {
-                return power_sensor.get_null_output<sym>();
-            }
-
-            switch (terminal_type) {
-                using enum MeasuredTerminalType;
-
                 case branch_from:
-                // all power sensors in branch3 are at from side in the mathematical model
-                case branch3_1:
-                case branch3_2:
-                case branch3_3:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_f);
                 case branch_to:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_t);
+                    return state.topo_comp_coup->branch[obj_seq];
                 case source:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].source[obj_math_id.pos].s);
+                    return state.topo_comp_coup->source[obj_seq];
                 case shunt:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].shunt[obj_math_id.pos].s);
+                    return state.topo_comp_coup->shunt[obj_seq];
                 case load:
                 case generator:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].load_gen[obj_math_id.pos].s);
+                    return state.topo_comp_coup->load_gen[obj_seq];
+                // from branch3, get relevant math object branch based on the measured side
+                case branch3_1:
+                    return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
+                                 state.topo_comp_coup->branch3[obj_seq].pos[0]};
+                case branch3_2:
+                    return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
+                                 state.topo_comp_coup->branch3[obj_seq].pos[1]};
+                case branch3_3:
+                    return Idx2D{state.topo_comp_coup->branch3[obj_seq].group,
+                                 state.topo_comp_coup->branch3[obj_seq].pos[2]};
                 case node:
-                    return power_sensor.get_output<sym>(math_output[obj_math_id.group].bus_injection[obj_math_id.pos]);
+                    return state.topo_comp_coup->node[obj_seq];
                 default:
                     throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
                                                   terminal_type);
+                }
+            }();
+
+            if (obj_math_id.group == -1) {
+                return power_sensor.get_null_output<sym>();
+            }
+
+            switch (terminal_type) {
+                using enum MeasuredTerminalType;
+
+            case branch_from:
+            // all power sensors in branch3 are at from side in the mathematical model
+            case branch3_1:
+            case branch3_2:
+            case branch3_3:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_f);
+            case branch_to:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_t);
+            case source:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].source[obj_math_id.pos].s);
+            case shunt:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].shunt[obj_math_id.pos].s);
+            case load:
+            case generator:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].load_gen[obj_math_id.pos].s);
+            case node:
+                return power_sensor.get_output<sym>(math_output[obj_math_id.group].bus_injection[obj_math_id.pos]);
+            default:
+                throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
+                                              terminal_type);
             }
         });
 }
 template <std::derived_from<GenericPowerSensor> Component, class ComponentContainer,
           short_circuit_math_output_type MathOutputType, std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
     return detail::produce_output<Component, Idx>(state, res_it,
                                                   [](GenericPowerSensor const& power_sensor, Idx const /* node_seq */) {
                                                       return power_sensor.get_null_sc_output();
                                                   });
 }
 
 // output fault
 template <std::same_as<Fault> Component, class ComponentContainer, steady_state_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component>
+    requires model_component_state<MainModelState, ComponentContainer, Component>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& /* math_output */, ResIt res_it) {
-    return detail::produce_output<Component, Idx2D>(state, res_it, [](Fault const& fault, Idx2D /* math_id */) {
-        return fault.get_output();
-    });
+    return detail::produce_output<Component, Idx2D>(
+        state, res_it, [](Fault const& fault, Idx2D /* math_id */) { return fault.get_output(); });
 }
 template <std::same_as<Fault> Component, class ComponentContainer, short_circuit_math_output_type MathOutputType,
           std::forward_iterator ResIt>
-requires model_component_state<MainModelState, ComponentContainer, Component> &&
-    model_component_state<MainModelState, ComponentContainer, Node>
+    requires model_component_state<MainModelState, ComponentContainer, Component> &&
+             model_component_state<MainModelState, ComponentContainer, Node>
 constexpr ResIt output_result(MainModelState<ComponentContainer> const& state,
                               std::vector<MathOutputType> const& math_output, ResIt res_it) {
     return detail::produce_output<Component, Idx2D>(
         state, res_it, [&state, &math_output](Fault const& fault, Idx2D math_id) {
             if (math_id.group == -1) {
                 return fault.get_null_sc_output();
             }
 
             auto const u_rated = state.components.template get_item<Node>(fault.get_fault_object()).u_rated();
             return fault.get_sc_output(math_output[math_id.group].fault[math_id.pos], u_rated);
         });
 }
 
-}  // namespace power_grid_model::main_core
+} // namespace power_grid_model::main_core
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 #include "../calculation_parameters.hpp"
 #include "../container.hpp"
 
 #include <concepts>
 
 namespace power_grid_model::main_core {
 
-template <class CompContainer>
-struct MainModelState {
+template <class CompContainer> struct MainModelState {
     using ComponentContainer = CompContainer;
 
     ComponentContainer components;
 
     // calculation parameters
     std::shared_ptr<ComponentTopology const> comp_topo;
 
@@ -26,22 +25,26 @@
     std::shared_ptr<TopologicalComponentToMathCoupling const> topo_comp_coup;
 
     ComponentToMathCoupling comp_coup;
 };
 
 template <typename ContainerType, typename ComponentType>
 concept component_container = requires(ContainerType const& c, ID id) {
-    { c.template citer<ComponentType>().begin() } -> std::forward_iterator;
-    { c.template citer<ComponentType>().end() } -> std::forward_iterator;
-    { *(c.template citer<ComponentType>().begin()) } -> std::same_as<ComponentType const&>;
-    { *(c.template citer<ComponentType>().end()) } -> std::same_as<ComponentType const&>;
-    { c.template get_item<ComponentType>(id) } -> std::convertible_to<ComponentType const&>;
-};
+                                  { c.template citer<ComponentType>().begin() } -> std::forward_iterator;
+                                  { c.template citer<ComponentType>().end() } -> std::forward_iterator;
+                                  {
+                                      *(c.template citer<ComponentType>().begin())
+                                      } -> std::same_as<ComponentType const&>;
+                                  { *(c.template citer<ComponentType>().end()) } -> std::same_as<ComponentType const&>;
+                                  {
+                                      c.template get_item<ComponentType>(id)
+                                      } -> std::convertible_to<ComponentType const&>;
+                              };
 
 template <template <typename T> class StateType, typename ContainerType, typename ComponentType>
 concept model_component_state =
     component_container<typename StateType<ContainerType>::ComponentContainer, ComponentType> &&
     std::same_as<StateType<ContainerType>, MainModelState<ContainerType>>;
 
-}  // namespace power_grid_model::main_core
+} // namespace power_grid_model::main_core
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 // template to update components
 // using forward interators
 // different selection based on component type
 // if sequence_idx is given, it will be used to load the object instead of using IDs via hash map.
 template <std::derived_from<Base> Component, class CacheType, class ComponentContainer,
           std::forward_iterator ForwardIterator>
-requires model_component_state<MainModelState, ComponentContainer, Component> UpdateChange
-update_component(MainModelState<ComponentContainer>& state, ForwardIterator begin, ForwardIterator end,
-                 std::vector<Idx2D> const& sequence_idx = {}) {
+    requires model_component_state<MainModelState, ComponentContainer, Component>
+UpdateChange update_component(MainModelState<ComponentContainer>& state, ForwardIterator begin, ForwardIterator end,
+                              std::vector<Idx2D> const& sequence_idx = {}) {
     bool const has_sequence_id = !sequence_idx.empty();
     Idx seq = 0;
 
     UpdateChange changed;
 
     // loop to to update component
     for (auto it = begin; it != end; ++it, ++seq) {
@@ -42,10 +42,10 @@
 
         changed = changed || comp.update(*it);
     }
 
     return changed;
 }
 
-}  // namespace power_grid_model::main_core
+} // namespace power_grid_model::main_core
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -32,45 +32,42 @@
 
 // threading
 #include <thread>
 
 namespace power_grid_model {
 
 // main model implementation template
-template <class T, class U>
-class MainModelImpl;
+template <class T, class U> class MainModelImpl;
 
 template <class... ExtraRetrievableType, class... ComponentType>
 class MainModelImpl<ExtraRetrievableTypes<ExtraRetrievableType...>, ComponentList<ComponentType...>> {
-   private:
+  private:
     // internal type traits
     // container class
     using ComponentContainer = Container<ExtraRetrievableTypes<ExtraRetrievableType...>, ComponentType...>;
     using MainModelState = main_core::MainModelState<ComponentContainer>;
 
     // trait on type list
     // struct of entry
     // name of the component, and the index in the list
     struct ComponentEntry {
         char const* name;
         size_t index;
     };
 
-    template <class T, class U>
-    struct component_list_generator_impl;
+    template <class T, class U> struct component_list_generator_impl;
     template <class... C, size_t... index>
     struct component_list_generator_impl<ComponentList<C...>, std::index_sequence<index...>> {
         using AllTypes = ComponentList<C...>;
         static constexpr std::array component_index_map{ComponentEntry{C::name, index}...};
         static constexpr size_t n_types = sizeof...(C);
 
         static size_t find_index(std::string const& name) {
-            auto const found = std::find_if(component_index_map.cbegin(), component_index_map.cend(), [&name](auto x) {
-                return x == name;
-            });
+            auto const found = std::find_if(component_index_map.cbegin(), component_index_map.cend(),
+                                            [&name](auto x) { return x == name; });
             assert(found != component_index_map.cend());
             return found->index;
         }
     };
     using AllComponents = component_list_generator_impl<ComponentList<ComponentType...>,
                                                         std::make_index_sequence<sizeof...(ComponentType)>>;
     static constexpr size_t n_types = AllComponents::n_types;
@@ -84,15 +81,15 @@
                                 DataPointer<false> const& data_ptr, Idx position);
     using CheckUpdateFunc = bool (*)(ConstDataPointer const& component_update);
     using GetSeqIdxFunc = std::vector<Idx2D> (*)(MainModelImpl const& x, ConstDataPointer const& component_update);
     using GetIndexerFunc = void (*)(MainModelImpl const& x, ID const* id_begin, Idx size, Idx* indexer_begin);
 
     static constexpr Idx ignore_output{-1};
 
-   public:
+  public:
     struct cached_update_t : std::true_type {};
 
     struct permanent_update_t : std::false_type {};
 
     // constructor with data
     explicit MainModelImpl(double system_frequency, ConstDataset const& input_data, Idx pos = 0)
         : system_frequency_{system_frequency} {
@@ -110,20 +107,18 @@
             // add
             add[entry.index](*this, found->second, pos);
         }
         set_construction_complete();
     }
 
     // constructor with only frequency
-    explicit MainModelImpl(double system_frequency) : system_frequency_{system_frequency} {
-    }
+    explicit MainModelImpl(double system_frequency) : system_frequency_{system_frequency} {}
 
     // get number
-    template <class CompType>
-    Idx component_count() const {
+    template <class CompType> Idx component_count() const {
         assert(construction_complete_);
         return state_.components.template size<CompType>();
     }
 
     // all component count
     std::map<std::string, Idx> all_component_count() const {
         std::map<std::string, Idx> map;
@@ -134,16 +129,15 @@
                 map[entry.name] = size;
             }
         }
         return map;
     }
 
     // helper function to add vectors of components
-    template <class CompType>
-    void add_component(std::vector<typename CompType::InputType> const& components) {
+    template <class CompType> void add_component(std::vector<typename CompType::InputType> const& components) {
         add_component<CompType>(components.cbegin(), components.cend());
     }
 
     // template to construct components
     // using forward interators
     // different selection based on component type
     template <std::derived_from<Base> CompType, std::forward_iterator ForwardIterator>
@@ -192,16 +186,15 @@
                 continue;
             }
             // try to find sequence idx
             auto const found_seq = sequence_idx_map.find(entry.name);
             if (found_seq == sequence_idx_map.cend()) {
                 // if not found sequence, update using IDs
                 update[entry.index](*this, found->second, pos, {});
-            }
-            else {
+            } else {
                 // else update using pre-cached sequence number
                 update[entry.index](*this, found->second, pos, found_seq->second);
             }
         }
     }
 
     // restore the initial values of all components
@@ -215,15 +208,15 @@
     // set complete construction
     // initialize internal arrays
     void set_construction_complete() {
         assert(!construction_complete_);
 #ifndef NDEBUG
         // set construction_complete for debug assertions
         construction_complete_ = true;
-#endif  // !NDEBUG
+#endif // !NDEBUG
         state_.components.set_construction_complete();
         // set component topo
         ComponentTopology comp_topo;
         comp_topo.n_node = state_.components.template size<Node>();
         // fill topology data
         comp_topo.branch_node_idx.resize(state_.components.template size<Branch>());
         std::transform(state_.components.template citer<Branch>().begin(),
@@ -237,78 +230,72 @@
                        state_.components.template citer<Branch3>().end(), comp_topo.branch3_node_idx.begin(),
                        [this](Branch3 const& branch3) {
                            return Branch3Idx{state_.components.template get_seq<Node>(branch3.node_1()),
                                              state_.components.template get_seq<Node>(branch3.node_2()),
                                              state_.components.template get_seq<Node>(branch3.node_3())};
                        });
         comp_topo.source_node_idx.resize(state_.components.template size<Source>());
-        std::transform(state_.components.template citer<Source>().begin(),
-                       state_.components.template citer<Source>().end(), comp_topo.source_node_idx.begin(),
-                       [this](Source const& source) {
-                           return state_.components.template get_seq<Node>(source.node());
-                       });
+        std::transform(
+            state_.components.template citer<Source>().begin(), state_.components.template citer<Source>().end(),
+            comp_topo.source_node_idx.begin(),
+            [this](Source const& source) { return state_.components.template get_seq<Node>(source.node()); });
         comp_topo.shunt_node_idx.resize(state_.components.template size<Shunt>());
         std::transform(state_.components.template citer<Shunt>().begin(),
                        state_.components.template citer<Shunt>().end(), comp_topo.shunt_node_idx.begin(),
-                       [this](Shunt const& shunt) {
-                           return state_.components.template get_seq<Node>(shunt.node());
-                       });
+                       [this](Shunt const& shunt) { return state_.components.template get_seq<Node>(shunt.node()); });
         comp_topo.load_gen_node_idx.resize(state_.components.template size<GenericLoadGen>());
         std::transform(state_.components.template citer<GenericLoadGen>().begin(),
                        state_.components.template citer<GenericLoadGen>().end(), comp_topo.load_gen_node_idx.begin(),
                        [this](GenericLoadGen const& load_gen) {
                            return state_.components.template get_seq<Node>(load_gen.node());
                        });
         comp_topo.load_gen_type.resize(state_.components.template size<GenericLoadGen>());
         std::transform(state_.components.template citer<GenericLoadGen>().begin(),
                        state_.components.template citer<GenericLoadGen>().end(), comp_topo.load_gen_type.begin(),
-                       [](GenericLoadGen const& load_gen) {
-                           return load_gen.type();
-                       });
+                       [](GenericLoadGen const& load_gen) { return load_gen.type(); });
         comp_topo.voltage_sensor_node_idx.resize(state_.components.template size<GenericVoltageSensor>());
         std::transform(state_.components.template citer<GenericVoltageSensor>().begin(),
                        state_.components.template citer<GenericVoltageSensor>().end(),
                        comp_topo.voltage_sensor_node_idx.begin(), [this](GenericVoltageSensor const& voltage_sensor) {
                            return state_.components.template get_seq<Node>(voltage_sensor.measured_object());
                        });
         comp_topo.power_sensor_object_idx.resize(state_.components.template size<GenericPowerSensor>());
-        std::transform(
-            state_.components.template citer<GenericPowerSensor>().begin(),
-            state_.components.template citer<GenericPowerSensor>().end(), comp_topo.power_sensor_object_idx.begin(),
-            [this](GenericPowerSensor const& power_sensor) {
-                switch (power_sensor.get_terminal_type()) {
-                    using enum MeasuredTerminalType;
-
-                    case branch_from:
-                    case branch_to:
-                        return state_.components.template get_seq<Branch>(power_sensor.measured_object());
-                    case source:
-                        return state_.components.template get_seq<Source>(power_sensor.measured_object());
-                    case shunt:
-                        return state_.components.template get_seq<Shunt>(power_sensor.measured_object());
-                    case load:
-                    case generator:
-                        return state_.components.template get_seq<GenericLoadGen>(power_sensor.measured_object());
-                    case branch3_1:
-                    case branch3_2:
-                    case branch3_3:
-                        return state_.components.template get_seq<Branch3>(power_sensor.measured_object());
-                    case node:
-                        return state_.components.template get_seq<Node>(power_sensor.measured_object());
-                    default:
-                        throw MissingCaseForEnumError("Power sensor idx to seq transformation",
-                                                      power_sensor.get_terminal_type());
-                }
-            });
-        comp_topo.power_sensor_terminal_type.resize(state_.components.template size<GenericPowerSensor>());
         std::transform(state_.components.template citer<GenericPowerSensor>().begin(),
                        state_.components.template citer<GenericPowerSensor>().end(),
-                       comp_topo.power_sensor_terminal_type.begin(), [](GenericPowerSensor const& power_sensor) {
-                           return power_sensor.get_terminal_type();
+                       comp_topo.power_sensor_object_idx.begin(), [this](GenericPowerSensor const& power_sensor) {
+                           switch (power_sensor.get_terminal_type()) {
+                               using enum MeasuredTerminalType;
+
+                           case branch_from:
+                           case branch_to:
+                               return state_.components.template get_seq<Branch>(power_sensor.measured_object());
+                           case source:
+                               return state_.components.template get_seq<Source>(power_sensor.measured_object());
+                           case shunt:
+                               return state_.components.template get_seq<Shunt>(power_sensor.measured_object());
+                           case load:
+                           case generator:
+                               return state_.components.template get_seq<GenericLoadGen>(
+                                   power_sensor.measured_object());
+                           case branch3_1:
+                           case branch3_2:
+                           case branch3_3:
+                               return state_.components.template get_seq<Branch3>(power_sensor.measured_object());
+                           case node:
+                               return state_.components.template get_seq<Node>(power_sensor.measured_object());
+                           default:
+                               throw MissingCaseForEnumError("Power sensor idx to seq transformation",
+                                                             power_sensor.get_terminal_type());
+                           }
                        });
+        comp_topo.power_sensor_terminal_type.resize(state_.components.template size<GenericPowerSensor>());
+        std::transform(state_.components.template citer<GenericPowerSensor>().begin(),
+                       state_.components.template citer<GenericPowerSensor>().end(),
+                       comp_topo.power_sensor_terminal_type.begin(),
+                       [](GenericPowerSensor const& power_sensor) { return power_sensor.get_terminal_type(); });
         state_.comp_topo = std::make_shared<ComponentTopology const>(std::move(comp_topo));
     }
 
     void reset_solvers() {
         assert(construction_complete_);
         is_topology_up_to_date_ = false;
         is_sym_parameter_up_to_date_ = false;
@@ -336,30 +323,30 @@
         for (ComponentEntry const& entry : AllComponents::component_index_map) {
             if (entry.name == component_type) {
                 return get_indexer_func[entry.index](*this, id_begin, size, indexer_begin);
             }
         }
     }
 
-   private:
+  private:
     void update_state(const UpdateChange& changes) {
         // if topology changed, everything is not up to date
         // if only param changed, set param to not up to date
         is_topology_up_to_date_ = is_topology_up_to_date_ && !changes.topo;
         is_sym_parameter_up_to_date_ = is_sym_parameter_up_to_date_ && !changes.topo && !changes.param;
         is_asym_parameter_up_to_date_ = is_asym_parameter_up_to_date_ && !changes.topo && !changes.param;
     }
 
     template <math_output_type MathOutputType, typename MathSolverType, typename InputType, typename PrepareInputFn,
               typename SolveFn>
-    requires std::invocable<std::remove_cvref_t<PrepareInputFn>> &&
-        std::invocable<std::remove_cvref_t<SolveFn>, MathSolverType&, InputType const&>&&
-            std::same_as<std::invoke_result_t<PrepareInputFn>, std::vector<InputType>>&&
-                std::same_as<std::invoke_result_t<SolveFn, MathSolverType&, InputType const&>, MathOutputType>
-                    std::vector<MathOutputType> calculate_(PrepareInputFn&& prepare_input, SolveFn&& solve) {
+        requires std::invocable<std::remove_cvref_t<PrepareInputFn>> &&
+                 std::invocable<std::remove_cvref_t<SolveFn>, MathSolverType&, InputType const&> &&
+                 std::same_as<std::invoke_result_t<PrepareInputFn>, std::vector<InputType>> &&
+                 std::same_as<std::invoke_result_t<SolveFn, MathSolverType&, InputType const&>, MathOutputType>
+    std::vector<MathOutputType> calculate_(PrepareInputFn&& prepare_input, SolveFn&& solve) {
         constexpr bool sym = symmetric_math_output_type<MathOutputType>;
 
         assert(construction_complete_);
         calculation_info_ = CalculationInfo{};
         // prepare
         Timer timer(calculation_info_, 2100, "Prepare");
         prepare_solvers<sym>();
@@ -372,41 +359,35 @@
         return math_output;
     }
 
     template <bool sym>
     std::vector<MathOutput<sym>> calculate_power_flow_(double err_tol, Idx max_iter,
                                                        CalculationMethod calculation_method) {
         return calculate_<MathOutput<sym>, MathSolver<sym>, PowerFlowInput<sym>>(
-            [this] {
-                return prepare_power_flow_input<sym>();
-            },
+            [this] { return prepare_power_flow_input<sym>(); },
             [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, PowerFlowInput<sym> const& y) {
                 return solver.run_power_flow(y, err_tol, max_iter, calculation_info_, calculation_method);
             });
     }
 
     template <bool sym>
     std::vector<MathOutput<sym>> calculate_state_estimation_(double err_tol, Idx max_iter,
                                                              CalculationMethod calculation_method) {
         return calculate_<MathOutput<sym>, MathSolver<sym>, StateEstimationInput<sym>>(
-            [this] {
-                return prepare_state_estimation_input<sym>();
-            },
+            [this] { return prepare_state_estimation_input<sym>(); },
             [this, err_tol, max_iter, calculation_method](MathSolver<sym>& solver, StateEstimationInput<sym> const& y) {
                 return solver.run_state_estimation(y, err_tol, max_iter, calculation_info_, calculation_method);
             });
     }
 
     template <bool sym>
     std::vector<ShortCircuitMathOutput<sym>> calculate_short_circuit_(double voltage_scaling_factor_c,
                                                                       CalculationMethod calculation_method) {
         return calculate_<ShortCircuitMathOutput<sym>, MathSolver<sym>, ShortCircuitInput>(
-            [this] {
-                return prepare_short_circuit_input<sym>();
-            },
+            [this] { return prepare_short_circuit_input<sym>(); },
             [this, voltage_scaling_factor_c, calculation_method](MathSolver<sym>& solver, ShortCircuitInput const& y) {
                 return solver.run_short_circuit(y, voltage_scaling_factor_c, calculation_info_, calculation_method);
             });
     }
 
     // get sequence idx map for fast caching of component sequences
     // only applicable for independent update dataset
@@ -452,45 +433,43 @@
     threading
         < 0 sequential
         = 0 parallel, use number of hardware threads
         > 0 specify number of parallel threads
     raise a BatchCalculationError if any of the calculations in the batch raised an exception
     */
     template <typename Calculate>
-    requires std::invocable<std::remove_cvref_t<Calculate>, MainModelImpl&, Dataset const&, Idx> BatchParameter
-    batch_calculation_(Calculate&& calculation_fn, Dataset const& result_data, ConstDataset const& update_data,
-                       Idx threading = -1) {
+        requires std::invocable<std::remove_cvref_t<Calculate>, MainModelImpl&, Dataset const&, Idx>
+    BatchParameter batch_calculation_(Calculate&& calculation_fn, Dataset const& result_data,
+                                      ConstDataset const& update_data, Idx threading = -1) {
         // if the update batch is one empty map without any component
         // execute one power flow in the current instance, no batch calculation is needed
         // NOTE: if the map is not empty but the datasets inside are empty
         //     that will be considered as a zero batch_size
         bool const all_empty = update_data.empty();
         if (all_empty) {
             calculation_fn(*this, result_data, 0);
             return BatchParameter{};
         }
 
         // get number of batches (can't be empty, because then all_empty would have been true)
         Idx const n_batch = update_data.cbegin()->second.batch_size();
         // assert if all component types have the same number of batches
-        assert(std::all_of(update_data.cbegin(), update_data.cend(), [n_batch](auto const& x) {
-            return x.second.batch_size() == n_batch;
-        }));
+        assert(std::all_of(update_data.cbegin(), update_data.cend(),
+                           [n_batch](auto const& x) { return x.second.batch_size() == n_batch; }));
 
         // if the batch_size is zero, it is a special case without doing any calculations at all
         // we consider in this case the batch set is independent and but not topology cachable
         if (n_batch == 0) {
             return BatchParameter{};
         }
 
         // calculate once to cache topology, ignore results, all math solvers are initialized
         try {
             calculation_fn(*this, {}, ignore_output);
-        }
-        catch (const SparseMatrixError&) {
+        } catch (const SparseMatrixError&) {
             // missing entries are provided in the update data
         }
 
         // const ref of current instance
         MainModelImpl const& base_model = *this;
 
         // cache component update order if possible
@@ -508,35 +487,32 @@
             MainModelImpl model{base_model};
             for (Idx batch_number = start; batch_number < n_batch; batch_number += stride) {
                 // try to update model and run calculation
                 try {
                     model.update_component<cached_update_t>(update_data, batch_number, sequence_idx_map);
                     calculation_fn(model, result_data, batch_number);
                     model.restore_components();
-                }
-                catch (std::exception const& ex) {
+                } catch (std::exception const& ex) {
                     exceptions[batch_number] = ex.what();
-                }
-                catch (...) {
+                } catch (...) {
                     exceptions[batch_number] = "unknown exception";
                 }
             }
         };
 
         // run batches sequential or parallel
         Idx const hardware_thread = (Idx)std::thread::hardware_concurrency();
         // run sequential if
         //    specified threading < 0
         //    use hardware threads, but it is either unknown (0) or only has one thread (1)
         //    specified threading = 1
         if (threading < 0 || threading == 1 || (threading == 0 && hardware_thread < 2)) {
             // run all in sequential
             sub_batch(0, 1);
-        }
-        else {
+        } else {
             // create parallel threads
             Idx const n_thread = threading == 0 ? hardware_thread : threading;
             std::vector<std::thread> threads;
             threads.reserve(n_thread);
             for (Idx thread_number = 0; thread_number != n_thread; ++thread_number) {
                 // compute each sub batch with stride
                 threads.emplace_back(sub_batch, thread_number, n_thread);
@@ -561,17 +537,16 @@
         if (!combined_error_message.empty()) {
             throw BatchCalculationError(combined_error_message, failed_scenarios, err_msgs);
         }
 
         return BatchParameter{};
     }
 
-   public:
-    template <class Component>
-    using UpdateType = typename Component::UpdateType;
+  public:
+    template <class Component> using UpdateType = typename Component::UpdateType;
 
     static bool is_update_independent(ConstDataset const& update_data) {
         // check all components
         return std::all_of(AllComponents::component_index_map.cbegin(), AllComponents::component_index_map.cend(),
                            [&update_data](ComponentEntry const& entry) {
                                static constexpr std::array check_component_update_independent{
                                    &is_component_update_independent<ComponentType>...};
@@ -581,16 +556,15 @@
                                    return true;
                                }
                                // check for this component update
                                return check_component_update_independent[entry.index](found->second);
                            });
     }
 
-    template <class Component>
-    static bool is_component_update_independent(ConstDataPointer const& component_update) {
+    template <class Component> static bool is_component_update_independent(ConstDataPointer const& component_update) {
         // If the batch size is (0 or) 1, then the update data for this component is 'independent'
         if (component_update.batch_size() <= 1) {
             return true;
         }
 
         // Remember the first batch size, then loop over the remaining batches and check if they are of the same length
         Idx const elements_per_scenario = component_update.elements_per_scenario(0);
@@ -687,21 +661,19 @@
     }
 
     // Single short circuit calculation, propagating the results to result_data
     void calculate_short_circuit(double voltage_scaling_factor_c, CalculationMethod calculation_method,
                                  Dataset const& result_data, Idx pos = 0) {
         assert(construction_complete_);
         if (std::all_of(state_.components.template citer<Fault>().begin(),
-                        state_.components.template citer<Fault>().end(), [](Fault const& fault) {
-                            return fault.get_fault_type() == FaultType::three_phase;
-                        })) {
+                        state_.components.template citer<Fault>().end(),
+                        [](Fault const& fault) { return fault.get_fault_type() == FaultType::three_phase; })) {
             auto const math_output = calculate_short_circuit_<true>(voltage_scaling_factor_c, calculation_method);
             output_result(math_output, result_data, pos);
-        }
-        else {
+        } else {
             auto const math_output = calculate_short_circuit_<false>(voltage_scaling_factor_c, calculation_method);
             output_result(math_output, result_data, pos);
         }
     }
 
     // Batch short circuit calculation, propagating the results to result_data
     BatchParameter calculate_short_circuit(double voltage_scaling_factor_c, CalculationMethod calculation_method,
@@ -755,19 +727,17 @@
 
     // TODO(mgovers): remove this functionality
     template <bool sym>
     void output_result(std::vector<MathOutput<sym>> const& math_output, Dataset const& result_data, Idx pos = 0) {
         return output_result<MathOutput<sym>>(math_output, result_data, pos);
     }
 
-    CalculationInfo calculation_info() {
-        return calculation_info_;
-    }
+    CalculationInfo calculation_info() { return calculation_info_; }
 
-   private:
+  private:
     double system_frequency_;
 
     MainModelState state_;
     // math model
     std::vector<MathSolver<true>> sym_solvers_;
     std::vector<MathSolver<false>> asym_solvers_;
     Idx n_math_solvers_{0};
@@ -775,32 +745,28 @@
     bool is_sym_parameter_up_to_date_{false};
     bool is_asym_parameter_up_to_date_{false};
     UpdateChange cached_state_changes_{};
     CalculationInfo calculation_info_;
 #ifndef NDEBUG
     // construction_complete is used for debug assertions only
     bool construction_complete_{false};
-#endif  // !NDEBUG
+#endif // !NDEBUG
 
-    template <bool sym>
-    bool& is_parameter_up_to_date() {
+    template <bool sym> bool& is_parameter_up_to_date() {
         if constexpr (sym) {
             return is_sym_parameter_up_to_date_;
-        }
-        else {
+        } else {
             return is_asym_parameter_up_to_date_;
         }
     }
 
-    template <bool sym>
-    std::vector<MathSolver<sym>>& get_solvers() {
+    template <bool sym> std::vector<MathSolver<sym>>& get_solvers() {
         if constexpr (sym) {
             return sym_solvers_;
-        }
-        else {
+        } else {
             return asym_solvers_;
         }
     }
 
     void rebuild_topology() {
         assert(construction_complete_);
         // clear old solvers
@@ -815,44 +781,37 @@
         std::transform(
             state_.components.template citer<Branch>().begin(), state_.components.template citer<Branch>().end(),
             comp_conn.branch_connected.begin(), [](Branch const& branch) {
                 return BranchConnected{static_cast<IntS>(branch.from_status()), static_cast<IntS>(branch.to_status())};
             });
         std::transform(state_.components.template citer<Branch>().begin(),
                        state_.components.template citer<Branch>().end(), comp_conn.branch_phase_shift.begin(),
-                       [](Branch const& branch) {
-                           return branch.phase_shift();
-                       });
+                       [](Branch const& branch) { return branch.phase_shift(); });
         std::transform(
             state_.components.template citer<Branch3>().begin(), state_.components.template citer<Branch3>().end(),
             comp_conn.branch3_connected.begin(), [](Branch3 const& branch3) {
                 return Branch3Connected{static_cast<IntS>(branch3.status_1()), static_cast<IntS>(branch3.status_2()),
                                         static_cast<IntS>(branch3.status_3())};
             });
         std::transform(state_.components.template citer<Branch3>().begin(),
                        state_.components.template citer<Branch3>().end(), comp_conn.branch3_phase_shift.begin(),
-                       [](Branch3 const& branch3) {
-                           return branch3.phase_shift();
-                       });
+                       [](Branch3 const& branch3) { return branch3.phase_shift(); });
         std::transform(state_.components.template citer<Source>().begin(),
                        state_.components.template citer<Source>().end(), comp_conn.source_connected.begin(),
-                       [](Source const& source) {
-                           return source.status();
-                       });
+                       [](Source const& source) { return source.status(); });
         // re build
         Topology topology{*state_.comp_topo, comp_conn};
         std::tie(state_.math_topology, state_.topo_comp_coup) = topology.build_topology();
         n_math_solvers_ = static_cast<Idx>(state_.math_topology.size());
         is_topology_up_to_date_ = true;
         is_sym_parameter_up_to_date_ = false;
         is_asym_parameter_up_to_date_ = false;
     }
 
-    template <bool sym>
-    std::vector<MathModelParam<sym>> get_math_param() {
+    template <bool sym> std::vector<MathModelParam<sym>> get_math_param() {
         std::vector<MathModelParam<sym>> math_param(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             math_param[i].branch_param.resize(state_.math_topology[i]->n_branch());
             math_param[i].shunt_param.resize(state_.math_topology[i]->n_shunt());
             math_param[i].source_param.resize(state_.math_topology[i]->n_source());
         }
         // loop all branch
@@ -897,17 +856,15 @@
             // assign parameters
             math_param[math_idx.group].source_param[math_idx.pos] =
                 state_.components.template get_item_by_seq<Source>(i).template math_param<sym>();
         }
         return math_param;
     }
 
-    static constexpr auto include_all = [](Idx) {
-        return true;
-    };
+    static constexpr auto include_all = [](Idx) { return true; };
 
     /** This is a heavily templated member function because it operates on many different variables of many different
      * types, but the essence is ever the same: filling one member (vector) of the calculation calc_input struct
      * (soa) with the right calculation symmetric or asymmetric calculation parameters, in the same order as the
      * corresponding component are stored in the component topology. There is one such struct for each sub graph / math
      * model and all of them are filled within the same function call (i.e. Notice that calc_input is a vector).
      *
@@ -955,17 +912,17 @@
      * @param include
      *      A lambda function (Idx i -> bool) which returns true if the component at Idx i should be included.
      * 	    The default lambda `include_all` always returns `true`.
      */
     template <bool sym, class CalcStructOut, typename CalcParamOut,
               std::vector<CalcParamOut>(CalcStructOut::*comp_vect), class ComponentIn,
               std::invocable<Idx> PredicateIn = decltype(include_all)>
-    requires std::convertible_to < std::invoke_result_t<PredicateIn, Idx>,
-    bool > void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
-                              PredicateIn include = include_all) {
+        requires std::convertible_to<std::invoke_result_t<PredicateIn, Idx>, bool>
+    void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
+                       PredicateIn include = include_all) {
         for (Idx i = 0, n = (Idx)components.size(); i != n; ++i) {
             if (include(i)) {
                 Idx2D const math_idx = components[i];
                 if (math_idx.group != -1) {
                     auto const& component = state_.components.template get_item_by_seq<ComponentIn>(i);
                     CalcParamOut const calc_param = calculate_param<sym>(component);
                     CalcStructOut& math_model_input = calc_input[math_idx.group];
@@ -975,40 +932,41 @@
             }
         }
     }
 
     template <bool sym, class CalcStructOut, typename CalcParamOut,
               std::vector<CalcParamOut>(CalcStructOut::*comp_vect), class ComponentIn,
               std::invocable<Idx> PredicateIn = decltype(include_all)>
-    requires std::convertible_to < std::invoke_result_t<PredicateIn, Idx>,
-    bool > void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
-                              std::invocable<ComponentIn const&> auto extra_args, PredicateIn include = include_all) {
+        requires std::convertible_to<std::invoke_result_t<PredicateIn, Idx>, bool>
+    void prepare_input(std::vector<Idx2D> const& components, std::vector<CalcStructOut>& calc_input,
+                       std::invocable<ComponentIn const&> auto extra_args, PredicateIn include = include_all) {
         for (Idx i = 0, n = (Idx)components.size(); i != n; ++i) {
             if (include(i)) {
                 Idx2D const math_idx = components[i];
                 if (math_idx.group != -1) {
                     auto const& component = state_.components.template get_item_by_seq<ComponentIn>(i);
                     CalcParamOut const calc_param = calculate_param<sym>(component, extra_args(component));
                     CalcStructOut& math_model_input = calc_input[math_idx.group];
                     std::vector<CalcParamOut>& math_model_input_vect = math_model_input.*comp_vect;
                     math_model_input_vect[math_idx.pos] = calc_param;
                 }
             }
         }
     }
 
-    template <bool sym>
-    auto calculate_param(auto const& c, auto const&... extra_args) {
-        if constexpr (requires { {c.calc_param(extra_args...)}; }) {
+    template <bool sym> auto calculate_param(auto const& c, auto const&... extra_args) {
+        if constexpr (requires {
+                          { c.calc_param(extra_args...) };
+                      }) {
             return c.calc_param(extra_args...);
-        }
-        else if constexpr (requires { {c.template calc_param<sym>(extra_args...)}; }) {
+        } else if constexpr (requires {
+                                 { c.template calc_param<sym>(extra_args...) };
+                             }) {
             return c.template calc_param<sym>(extra_args...);
-        }
-        else {
+        } else {
             return;
         }
     }
 
     template <bool sym, IntSVector(StateEstimationInput<sym>::*component), class Component>
     void prepare_input_status(std::vector<Idx2D> const& objects, std::vector<StateEstimationInput<sym>>& input) {
         for (Idx i = 0, n = (Idx)objects.size(); i != n; ++i) {
@@ -1017,16 +975,15 @@
                 continue;
             }
             (input[math_idx.group].*component)[math_idx.pos] =
                 state_.components.template get_item_by_seq<Component>(i).status();
         }
     }
 
-    template <bool sym>
-    std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
+    template <bool sym> std::vector<PowerFlowInput<sym>> prepare_power_flow_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
         std::vector<PowerFlowInput<sym>> pf_input(n_math_solvers_);
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             pf_input[i].s_injection.resize(state_.math_topology[i]->n_load_gen());
             pf_input[i].source.resize(state_.math_topology[i]->n_source());
         }
         prepare_input<sym, PowerFlowInput<sym>, DoubleComplex, &PowerFlowInput<sym>::source, Source>(
@@ -1034,16 +991,15 @@
 
         prepare_input<sym, PowerFlowInput<sym>, ComplexValue<sym>, &PowerFlowInput<sym>::s_injection, GenericLoadGen>(
             state_.topo_comp_coup->load_gen, pf_input);
 
         return pf_input;
     }
 
-    template <bool sym>
-    std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
+    template <bool sym> std::vector<StateEstimationInput<sym>> prepare_state_estimation_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
 
         std::vector<StateEstimationInput<sym>> se_input(n_math_solvers_);
 
         for (Idx i = 0; i != n_math_solvers_; ++i) {
             se_input[i].shunt_status.resize(state_.math_topology[i]->n_shunt());
             se_input[i].load_gen_status.resize(state_.math_topology[i]->n_load_gen());
@@ -1065,28 +1021,26 @@
                                                                                      se_input);
 
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_voltage, GenericVoltageSensor>(
             state_.topo_comp_coup->voltage_sensor, se_input);
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_source_power, GenericPowerSensor>(
-            state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
-                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::source;
-            });
+            state_.topo_comp_coup->power_sensor, se_input,
+            [this](Idx i) { return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::source; });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_load_gen_power, GenericPowerSensor>(
             state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
                 return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
                        state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_shunt_power, GenericPowerSensor>(
-            state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
-                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
-            });
+            state_.topo_comp_coup->power_sensor, se_input,
+            [this](Idx i) { return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::shunt; });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_from_power, GenericPowerSensor>(
             state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
                 return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_from ||
                        // all branch3 sensors are at from side in the mathematical model
                        state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_1 ||
                        state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_2 ||
@@ -1095,35 +1049,33 @@
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_to_power, GenericPowerSensor>(
             state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
                 return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_bus_injection, GenericPowerSensor>(
-            state_.topo_comp_coup->power_sensor, se_input, [this](Idx i) {
-                return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::node;
-            });
+            state_.topo_comp_coup->power_sensor, se_input,
+            [this](Idx i) { return state_.comp_topo->power_sensor_terminal_type[i] == MeasuredTerminalType::node; });
 
         return se_input;
     }
 
-    template <bool sym>
-    std::vector<ShortCircuitInput> prepare_short_circuit_input() {
+    template <bool sym> std::vector<ShortCircuitInput> prepare_short_circuit_input() {
         assert(is_topology_up_to_date_ && is_parameter_up_to_date<sym>());
 
         std::vector<IdxVector> topo_fault_indices(state_.math_topology.size());
         std::vector<IdxVector> topo_bus_indices(state_.math_topology.size());
 
         for (Idx fault_idx{0}; fault_idx < state_.components.template size<Fault>(); ++fault_idx) {
             auto const& fault = state_.components.template get_item_by_seq<Fault>(fault_idx);
             if (fault.status()) {
                 auto const node_idx = state_.components.template get_seq<Node>(fault.get_fault_object());
                 auto const topo_bus_idx = state_.topo_comp_coup->node[node_idx];
 
-                if (topo_bus_idx.group >= 0) {  // Consider non-isolated objects only
+                if (topo_bus_idx.group >= 0) { // Consider non-isolated objects only
                     topo_fault_indices[topo_bus_idx.group].push_back(fault_idx);
                     topo_bus_indices[topo_bus_idx.group].push_back(topo_bus_idx.pos);
                 }
             }
         }
 
         auto fault_coup = std::vector<Idx2D>(state_.components.template size<Fault>(), Idx2D{-1, -1});
@@ -1149,16 +1101,15 @@
             });
         prepare_input<sym, ShortCircuitInput, DoubleComplex, &ShortCircuitInput::source, Source>(
             state_.topo_comp_coup->source, sc_input);
 
         return sc_input;
     }
 
-    template <bool sym>
-    void prepare_solvers() {
+    template <bool sym> void prepare_solvers() {
         std::vector<MathSolver<sym>>& solvers = get_solvers<sym>();
         // also get the vector of other solvers (sym -> asym, or asym -> sym)
         std::vector<MathSolver<!sym>>& other_solvers = get_solvers<!sym>();
         // rebuild topology if needed
         if (!is_topology_up_to_date_) {
             rebuild_topology();
         }
@@ -1200,10 +1151,10 @@
 };
 
 using MainModel =
     MainModelImpl<ExtraRetrievableTypes<Base, Node, Branch, Branch3, Appliance, GenericLoadGen, GenericLoad,
                                         GenericGenerator, GenericPowerSensor, GenericVoltageSensor>,
                   AllComponents>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -13,66 +13,55 @@
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
-template <scalar_value T, bool sym, bool is_tensor, int n_sub_block>
-struct block_trait {
+template <scalar_value T, bool sym, bool is_tensor, int n_sub_block> struct block_trait {
     static constexpr int n_row = sym ? n_sub_block : n_sub_block * 3;
     static constexpr int n_col = is_tensor ? (sym ? n_sub_block : n_sub_block * 3) : 1;
     using ArrayType = Eigen::Array<T, n_row, n_col, Eigen::ColMajor>;
 };
 
 template <class T, bool sym, bool is_tensor, int n_sub_block>
 class Block : public block_trait<T, sym, is_tensor, n_sub_block>::ArrayType {
-   public:
+  public:
     using ArrayType = typename block_trait<T, sym, is_tensor, n_sub_block>::ArrayType;
     using ArrayType::operator();
 
     // default zero
     Block() : ArrayType{ArrayType::Zero()} {};
     // eigen expression
-    template <typename OtherDerived>
-    explicit Block(Eigen::ArrayBase<OtherDerived> const& other) : ArrayType{other} {
-    }
-    template <typename OtherDerived>
-    Block& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
+    template <typename OtherDerived> explicit Block(Eigen::ArrayBase<OtherDerived> const& other) : ArrayType{other} {}
+    template <typename OtherDerived> Block& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
         this->ArrayType::operator=(other);
         return *this;
     }
 
-    template <int r>
-    static auto get_asym_row_idx() {
-        return Eigen::seqN(Eigen::fix<r * 3>, Eigen::fix<3>);
-    }
-    template <int c>
-    static auto get_asym_col_idx() {
+    template <int r> static auto get_asym_row_idx() { return Eigen::seqN(Eigen::fix<r * 3>, Eigen::fix<3>); }
+    template <int c> static auto get_asym_col_idx() {
         if constexpr (is_tensor) {
             return Eigen::seqN(Eigen::fix<c * 3>, Eigen::fix<3>);
-        }
-        else {
+        } else {
             return Eigen::seqN(Eigen::fix<0>, Eigen::fix<1>);
         }
     }
 
     template <int r, int c>
     using GetterType =
         std::conditional_t<sym, T&, decltype(std::declval<ArrayType>()(get_asym_row_idx<r>(), get_asym_col_idx<c>()))>;
 
-    template <int r, int c>
-    GetterType<r, c> get_val() {
+    template <int r, int c> GetterType<r, c> get_val() {
         if constexpr (sym) {
             return (*this)(r, c);
-        }
-        else {
+        } else {
             return (*this)(get_asym_row_idx<r>(), get_asym_col_idx<c>());
         }
     }
 };
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,24 @@
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
 // solver
-template <bool sym>
-class IterativeCurrentPFSolver : public IterativePFSolver<sym, IterativeCurrentPFSolver<sym>> {
-   public:
+template <bool sym> class IterativeCurrentPFSolver : public IterativePFSolver<sym, IterativeCurrentPFSolver<sym>> {
+  public:
     using BlockPermArray =
         typename SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>>::BlockPermArray;
 
     IterativeCurrentPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : IterativePFSolver<sym, IterativeCurrentPFSolver>{y_bus, topo_ptr},
           rhs_u_(y_bus.size()),
           y_data_ptr_(nullptr),
-          sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()} {
-    }
+          sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()} {}
 
     // Add source admittance to Y bus and set variable for prepared y bus to true
     void initialize_derived_solver(YBus<sym> const& y_bus, MathOutput<sym> const&) {
         IdxVector const& source_bus_indptr = *this->source_bus_indptr_;
         ComplexTensorVector<sym> const& ydata = y_bus.admittance();
         IdxVector const& bus_entry = y_bus.lu_diag();
         // if Y bus is not up to date
@@ -138,46 +136,43 @@
             for (Idx load_number = load_gen_bus_indptr[bus_number]; load_number != load_gen_bus_indptr[bus_number + 1];
                  ++load_number) {
                 // load type
                 LoadGenType const type = load_gen_type[load_number];
                 switch (type) {
                     using enum LoadGenType;
 
-                    case const_pq:
-                        // I_inj_i = conj(S_inj_j/U_i) for constant PQ type
-                        rhs_u_[bus_number] += conj(input.s_injection[load_number] / u[bus_number]);
-                        break;
-                    case const_y:
-                        // I_inj_i = conj((S_inj_j * abs(U_i)^2) / U_i) = conj((S_inj_j) * U_i for const impedance type
-                        rhs_u_[bus_number] += conj(input.s_injection[load_number]) * u[bus_number];
-                        break;
-                    case const_i:
-                        // I_inj_i = conj(S_inj_j*abs(U_i)/U_i) for const current type
-                        rhs_u_[bus_number] +=
-                            conj(input.s_injection[load_number] * cabs(u[bus_number]) / u[bus_number]);
-                        break;
-                    default:
-                        throw MissingCaseForEnumError("Injection current calculation", type);
+                case const_pq:
+                    // I_inj_i = conj(S_inj_j/U_i) for constant PQ type
+                    rhs_u_[bus_number] += conj(input.s_injection[load_number] / u[bus_number]);
+                    break;
+                case const_y:
+                    // I_inj_i = conj((S_inj_j * abs(U_i)^2) / U_i) = conj((S_inj_j) * U_i for const impedance type
+                    rhs_u_[bus_number] += conj(input.s_injection[load_number]) * u[bus_number];
+                    break;
+                case const_i:
+                    // I_inj_i = conj(S_inj_j*abs(U_i)/U_i) for const current type
+                    rhs_u_[bus_number] += conj(input.s_injection[load_number] * cabs(u[bus_number]) / u[bus_number]);
+                    break;
+                default:
+                    throw MissingCaseForEnumError("Injection current calculation", type);
                 }
             }
             // loop sources: j
             for (Idx source_number = source_bus_indptr[bus_number]; source_number != source_bus_indptr[bus_number + 1];
                  ++source_number) {
                 // I_inj_i += Y_source_j * U_ref_j
                 rhs_u_[bus_number] += dot(y_bus.math_model_param().source_param[source_number],
                                           ComplexValue<sym>{input.source[source_number]});
             }
         }
     }
 
     // Solve the linear equations I_inj = YU
     // inplace
-    void solve_matrix() {
-        sparse_solver_.solve_with_prefactorized_matrix(*mat_data_, *perm_, rhs_u_, rhs_u_);
-    }
+    void solve_matrix() { sparse_solver_.solve_with_prefactorized_matrix(*mat_data_, *perm_, rhs_u_, rhs_u_); }
 
     // Find maximum deviation in voltage among all buses
     double iterate_unknown(ComplexValueVector<sym>& u) {
         double max_dev = 0.0;
         // loop all buses
         for (Idx bus_number = 0; bus_number != this->n_bus_; ++bus_number) {
             // Get maximum iteration for a bus
@@ -186,27 +181,26 @@
             max_dev = std::max(dev, max_dev);
             // assign updated values
             u[bus_number] = rhs_u_[bus_number];
         }
         return max_dev;
     }
 
-   private:
+  private:
     ComplexValueVector<sym> rhs_u_;
     std::shared_ptr<ComplexTensorVector<sym> const> mat_data_;
     ComplexTensorVector<sym> const* y_data_ptr_;
     // sparse solver
     SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>> sparse_solver_;
     std::shared_ptr<BlockPermArray const> perm_;
 };
 
 template class IterativeCurrentPFSolver<true>;
 template class IterativeCurrentPFSolver<false>;
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-template <bool sym>
-using IterativeCurrentPFSolver = math_model_impl::IterativeCurrentPFSolver<sym>;
+template <bool sym> using IterativeCurrentPFSolver = math_model_impl::IterativeCurrentPFSolver<sym>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -20,93 +20,71 @@
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
 // block class for the unknown vector and/or right-hand side in state estimation equation
-template <bool sym>
-struct SEUnknown : public Block<DoubleComplex, sym, false, 2> {
-    template <int r, int c>
-    using GetterType = typename Block<DoubleComplex, sym, false, 2>::template GetterType<r, c>;
+template <bool sym> struct SEUnknown : public Block<DoubleComplex, sym, false, 2> {
+    template <int r, int c> using GetterType = typename Block<DoubleComplex, sym, false, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<DoubleComplex, sym, false, 2>::Block;
     using Block<DoubleComplex, sym, false, 2>::operator=;
 
-    GetterType<0, 0> u() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<1, 0> phi() {
-        return this->template get_val<1, 0>();
-    }
+    GetterType<0, 0> u() { return this->template get_val<0, 0>(); }
+    GetterType<1, 0> phi() { return this->template get_val<1, 0>(); }
 
-    GetterType<0, 0> eta() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<1, 0> tau() {
-        return this->template get_val<1, 0>();
-    }
+    GetterType<0, 0> eta() { return this->template get_val<0, 0>(); }
+    GetterType<1, 0> tau() { return this->template get_val<1, 0>(); }
 };
 
 // block class for the right hand side in state estimation equation
-template <bool sym>
-using SERhs = SEUnknown<sym>;
+template <bool sym> using SERhs = SEUnknown<sym>;
 
 // class of 2*2 (6*6) se gain block
 /*
 [
    [G, QH]
    [Q, R ]
 ]
 */
-template <bool sym>
-class SEGainBlock : public Block<DoubleComplex, sym, true, 2> {
-   public:
-    template <int r, int c>
-    using GetterType = typename Block<DoubleComplex, sym, true, 2>::template GetterType<r, c>;
+template <bool sym> class SEGainBlock : public Block<DoubleComplex, sym, true, 2> {
+  public:
+    template <int r, int c> using GetterType = typename Block<DoubleComplex, sym, true, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<DoubleComplex, sym, true, 2>::Block;
     using Block<DoubleComplex, sym, true, 2>::operator=;
 
-    GetterType<0, 0> g() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<0, 1> qh() {
-        return this->template get_val<0, 1>();
-    }
-    GetterType<1, 0> q() {
-        return this->template get_val<1, 0>();
-    }
-    GetterType<1, 1> r() {
-        return this->template get_val<1, 1>();
-    }
+    GetterType<0, 0> g() { return this->template get_val<0, 0>(); }
+    GetterType<0, 1> qh() { return this->template get_val<0, 1>(); }
+    GetterType<1, 0> q() { return this->template get_val<1, 0>(); }
+    GetterType<1, 1> r() { return this->template get_val<1, 1>(); }
 };
 
 // processed measurement struct
 // combined all measurement of the same quantity
 // accumulate for bus injection measurement
-template <bool sym>
-class MeasuredValues {
+template <bool sym> class MeasuredValues {
     static constexpr Idx disconnected = -1;
     static constexpr Idx unmeasured = -2;
     static constexpr Idx undefined = -3;
 
     // struct to store bus injection information
     struct BusInjection {
         // The index in main_value_ where the total measured bus injection is stored.
         // This includes node injection measurements, source power measurements and load/gen power measurements.
         Idx idx_bus_injection{undefined};
 
         // The number of unmeasured appliances
         Idx n_unmeasured_appliances = 0;
     };
 
-   public:
+  public:
     // construct
     MeasuredValues(YBus<sym> const& y_bus, StateEstimationInput<sym> const& input)
         : math_topology_{y_bus.shared_topology()},
           bus_appliance_injection_(math_topology().n_bus()),
           idx_voltage_(math_topology().n_bus()),
           bus_injection_(math_topology().n_bus()),
           idx_branch_from_power_(math_topology().n_branch()),
@@ -124,62 +102,44 @@
         // loop branch
         process_branch_measurements(input);
         // normalize
         normalize_variance();
     }
 
     // checker of measured data, return true if measurement is available
-    bool has_voltage(Idx bus) const {
-        return idx_voltage_[bus] >= 0;
-    }
-    bool has_bus_injection(Idx bus) const {
-        return bus_injection_[bus].idx_bus_injection >= 0;
-    }
-    bool has_branch_from(Idx branch) const {
-        return idx_branch_from_power_[branch] >= 0;
-    }
-    bool has_branch_to(Idx branch) const {
-        return idx_branch_to_power_[branch] >= 0;
-    }
-    bool has_shunt(Idx shunt) const {
-        return idx_shunt_power_[shunt] >= 0;
-    }
-    bool has_load_gen(Idx load_gen) const {
-        return idx_load_gen_power_[load_gen] >= 0;
-    }
-    bool has_source(Idx source) const {
-        return idx_source_power_[source] >= 0;
-    }
-    bool has_angle() const {
-        return n_angle_ > 0;
-    }
+    bool has_voltage(Idx bus) const { return idx_voltage_[bus] >= 0; }
+    bool has_bus_injection(Idx bus) const { return bus_injection_[bus].idx_bus_injection >= 0; }
+    bool has_branch_from(Idx branch) const { return idx_branch_from_power_[branch] >= 0; }
+    bool has_branch_to(Idx branch) const { return idx_branch_to_power_[branch] >= 0; }
+    bool has_shunt(Idx shunt) const { return idx_shunt_power_[shunt] >= 0; }
+    bool has_load_gen(Idx load_gen) const { return idx_load_gen_power_[load_gen] >= 0; }
+    bool has_source(Idx source) const { return idx_source_power_[source] >= 0; }
+    bool has_angle() const { return n_angle_ > 0; }
 
     // getter of measurement and variance
     // if the obj is not measured, it is undefined behaviour to call this function
     // use checker first
 
     // getter of voltage variance
-    double voltage_var(Idx bus) const {
-        return main_value_[idx_voltage_[bus]].variance;
-    }
+    double voltage_var(Idx bus) const { return main_value_[idx_voltage_[bus]].variance; }
     // getter of voltage value for all buses
     // for no measurement, the voltage phasor is used from the current iteration
     // for magnitude only measurement, angle is added from the current iteration
     // for magnitude and angle measurement, the measured phasor is returned
     ComplexValueVector<sym> voltage(ComplexValueVector<sym> const& current_u) const {
         ComplexValueVector<sym> u(current_u.size());
         for (Idx bus = 0; bus != (Idx)current_u.size(); ++bus) {
             // no measurement
             if (idx_voltage_[bus] == unmeasured) {
                 u[bus] = current_u[bus];
             }
             // no angle measurement
             else if (is_nan(imag(main_value_[idx_voltage_[bus]].value))) {
                 u[bus] = real(main_value_[idx_voltage_[bus]].value) * current_u[bus] /
-                         cabs(current_u[bus]);  // U / |U| to get angle shift
+                         cabs(current_u[bus]); // U / |U| to get angle shift
             }
             // full measurement
             else {
                 u[bus] = main_value_[idx_voltage_[bus]].value;
             }
         }
         return u;
@@ -188,34 +148,24 @@
     // power measurement
     SensorCalcParam<sym> const& bus_injection(Idx bus) const {
         return main_value_[bus_injection_[bus].idx_bus_injection];
     }
     SensorCalcParam<sym> const& branch_from_power(Idx branch) const {
         return main_value_[idx_branch_from_power_[branch]];
     }
-    SensorCalcParam<sym> const& branch_to_power(Idx branch) const {
-        return main_value_[idx_branch_to_power_[branch]];
-    }
-    SensorCalcParam<sym> const& shunt_power(Idx shunt) const {
-        return main_value_[idx_shunt_power_[shunt]];
-    }
+    SensorCalcParam<sym> const& branch_to_power(Idx branch) const { return main_value_[idx_branch_to_power_[branch]]; }
+    SensorCalcParam<sym> const& shunt_power(Idx shunt) const { return main_value_[idx_shunt_power_[shunt]]; }
     SensorCalcParam<sym> const& load_gen_power(Idx load_gen) const {
         return extra_value_[idx_load_gen_power_[load_gen]];
     }
-    SensorCalcParam<sym> const& source_power(Idx source) const {
-        return extra_value_[idx_source_power_[source]];
-    }
+    SensorCalcParam<sym> const& source_power(Idx source) const { return extra_value_[idx_source_power_[source]]; }
 
     // getter mean angle shift
-    RealValue<sym> mean_angle_shift() const {
-        return mean_angle_shift_;
-    }
-    bool has_angle_measurement() const {
-        return n_angle_ > 0;
-    }
+    RealValue<sym> mean_angle_shift() const { return mean_angle_shift_; }
+    bool has_angle_measurement() const { return n_angle_ > 0; }
 
     // calculate load_gen and source flow
     // with given bus voltage and bus current injection
     using FlowVector = std::vector<ApplianceMathOutput<sym>>;
     using LoadGenSourceFlow = std::pair<FlowVector, FlowVector>;
 
     LoadGenSourceFlow calculate_load_gen_source(ComplexValueVector<sym> const& u,
@@ -248,15 +198,15 @@
                 source_flow[source].i = conj(source_flow[source].s / u[bus]);
             }
         }
 
         return std::make_pair(load_gen_flow, source_flow);
     }
 
-   private:
+  private:
     // cache topology
     std::shared_ptr<MathModelTopology const> math_topology_;
 
     // flat array of all the relevant measurement for the main calculation
     // branch/shunt flow, bus voltage, injection flow
     std::vector<SensorCalcParam<sym>> main_value_;
     // flat array of all the load_gen/source measurement
@@ -280,17 +230,15 @@
     IdxVector idx_source_power_;
     // number of angle measurement
     Idx n_angle_;
     // average angle shift of voltages with angle measurement
     // default is zero is no voltage has angle measurement
     RealValue<sym> mean_angle_shift_;
 
-    MathModelTopology const& math_topology() const {
-        return *math_topology_;
-    }
+    MathModelTopology const& math_topology() const { return *math_topology_; }
 
     void process_bus_related_measurements(StateEstimationInput<sym> const& input) {
         /*
         The main purpose of this function is to aggregate all voltage and power sensor values to
             one voltage sensor value per bus.
             one injection power sensor value per bus.
             one power sensor value per shunt (in injection reference direction, note shunt itself is not considered as
@@ -314,34 +262,30 @@
         which is considered as a measurement in the main_value_ with zero variance.
 
         The voltage values in main_value_ can be found using idx_voltage.
         The power values in main_value_ can be found using bus_injection_ (for combined load_gen and source)
         and idx_shunt_power_ (for shunt).
         */
         MathModelTopology const& topo = math_topology();
-        RealValue<sym> angle_cum{};  // cumulative angle
+        RealValue<sym> angle_cum{}; // cumulative angle
         for (Idx bus = 0; bus != topo.n_bus(); ++bus) {
             // voltage
             {
                 Idx const begin = topo.voltage_sensor_indptr[bus];
                 Idx const end = topo.voltage_sensor_indptr[bus + 1];
                 if (begin == end) {
                     idx_voltage_[bus] = unmeasured;
-                }
-                else {
+                } else {
                     idx_voltage_[bus] = (Idx)main_value_.size();
                     // check if there is nan
                     if (std::any_of(input.measured_voltage.cbegin() + begin, input.measured_voltage.cbegin() + end,
-                                    [](auto const& x) {
-                                        return is_nan(imag(x.value));
-                                    })) {
+                                    [](auto const& x) { return is_nan(imag(x.value)); })) {
                         // only keep magnitude
                         main_value_.push_back(combine_measurements<true>(input.measured_voltage, begin, end));
-                    }
-                    else {
+                    } else {
                         // keep complex number
                         main_value_.push_back(combine_measurements(input.measured_voltage, begin, end));
                         ++n_angle_;
                         // accumulate angle, offset by intrinsic phase shift
                         angle_cum += arg(main_value_.back().value * std::exp(-1.0i * topo.phase_shift[bus]));
                     }
                 }
@@ -400,29 +344,26 @@
                 // combine valid appliance_injection_measurement and direct_injection_measurement
                 // three scenarios, check if we have valid injection measurement
                 if (n_unmeasured == 0 || !std::isinf(direct_injection_measurement.variance)) {
                     bus_injection_[bus].idx_bus_injection = (Idx)main_value_.size();
                     if (n_unmeasured > 0) {
                         // only direct injection
                         main_value_.push_back(direct_injection_measurement);
-                    }
-                    else if (std::isinf(direct_injection_measurement.variance) ||
-                             appliance_injection_measurement.variance == 0.0) {
+                    } else if (std::isinf(direct_injection_measurement.variance) ||
+                               appliance_injection_measurement.variance == 0.0) {
                         // only appliance injection if
                         //    there is no direct injection measurement,
                         //    or we have zero injection
                         main_value_.push_back(appliance_injection_measurement);
-                    }
-                    else {
+                    } else {
                         // both valid, we combine again
                         main_value_.push_back(combine_measurements(
                             {direct_injection_measurement, appliance_injection_measurement}, 0, 2));
                     }
-                }
-                else {
+                } else {
                     bus_injection_[bus].idx_bus_injection = unmeasured;
                 }
             }
         }
         // assign a meaningful mean angle shift, if at least one voltage has angle measurement
         if (n_angle_ > 0) {
             mean_angle_shift_ = angle_cum / n_angle_;
@@ -444,20 +385,16 @@
         idx_branch_to_power_/idx_branch_from_power_ is set to disconnected.
         Else, idx_branch_to_power_/idx_branch_from_power_ is set to the index of the aggregated data in main_value_.
 
         All measurement values for a single side of a branch are combined in a weighted average, which is appended to
         main_value_. The power values in main_value_ can be found using idx_branch_to_power_/idx_branch_from_power_.
         */
         MathModelTopology const& topo = math_topology();
-        static constexpr auto branch_from_checker = [](BranchIdx x) -> bool {
-            return x[0] != -1;
-        };
-        static constexpr auto branch_to_checker = [](BranchIdx x) -> bool {
-            return x[1] != -1;
-        };
+        static constexpr auto branch_from_checker = [](BranchIdx x) -> bool { return x[0] != -1; };
+        static constexpr auto branch_to_checker = [](BranchIdx x) -> bool { return x[1] != -1; };
         for (Idx branch = 0; branch != topo.n_branch(); ++branch) {
             // from side
             idx_branch_from_power_[branch] =
                 process_one_object(branch, topo.branch_from_power_sensor_indptr, topo.branch_bus_idx,
                                    input.measured_branch_from_power, main_value_, branch_from_checker);
             // to side
             idx_branch_to_power_[branch] =
@@ -476,22 +413,20 @@
         double accumulated_inverse_variance = 0.0;
         ComplexValue<sym> accumulated_value{};
         for (Idx pos = begin; pos != end; ++pos) {
             accumulated_inverse_variance += 1.0 / data[pos].variance;
             if constexpr (only_magnitude) {
                 ComplexValue<sym> abs_value = piecewise_complex_value<sym>(DoubleComplex{0.0, nan});
                 if (is_nan(imag(data[pos].value))) {
-                    abs_value += real(data[pos].value);  // only keep real part
-                }
-                else {
-                    abs_value += cabs(data[pos].value);  // get abs of the value
+                    abs_value += real(data[pos].value); // only keep real part
+                } else {
+                    abs_value += cabs(data[pos].value); // get abs of the value
                 }
                 accumulated_value += abs_value / data[pos].variance;
-            }
-            else {
+            } else {
                 // accumulate value
                 accumulated_value += data[pos].value / data[pos].variance;
             }
         }
         return SensorCalcParam<sym>{accumulated_value / accumulated_inverse_variance,
                                     1.0 / accumulated_inverse_variance};
     }
@@ -503,17 +438,15 @@
                                     std::vector<SensorCalcParam<sym>>& result_data, IdxVector& result_idx) {
         for (Idx obj = obj_indptr[bus]; obj != obj_indptr[bus + 1]; ++obj) {
             result_idx[obj] = process_one_object(obj, sensor_indptr, obj_status, input_data, result_data);
         }
     }
 
     // process one object
-    static constexpr auto default_status_checker = [](auto x) -> bool {
-        return x;
-    };
+    static constexpr auto default_status_checker = [](auto x) -> bool { return x; };
     template <class TS, class StatusChecker = decltype(default_status_checker)>
     static Idx process_one_object(Idx const obj, IdxVector const& sensor_indptr, std::vector<TS> const& obj_status,
                                   std::vector<SensorCalcParam<sym>> const& input_data,
                                   std::vector<SensorCalcParam<sym>>& result_data,
                                   StatusChecker status_checker = default_status_checker) {
         Idx const begin = sensor_indptr[obj];
         Idx const end = sensor_indptr[obj + 1];
@@ -537,39 +470,35 @@
         for (SensorCalcParam<sym> const& x : main_value_) {
             // only non-zero variance is considered
             if (x.variance != 0.0) {
                 min_var = std::min(min_var, x.variance);
             }
         }
         // scale
-        std::for_each(main_value_.begin(), main_value_.end(), [&](SensorCalcParam<sym>& x) {
-            x.variance /= min_var;
-        });
+        std::for_each(main_value_.begin(), main_value_.end(), [&](SensorCalcParam<sym>& x) { x.variance /= min_var; });
     }
 
     void calculate_non_over_determined_injection(Idx n_unmeasured, Idx load_gen_begin, Idx load_gen_end,
                                                  Idx source_begin, Idx source_end,
                                                  SensorCalcParam<sym> const& bus_appliance_injection,
                                                  ComplexValue<sym> const& s, FlowVector& load_gen_flow,
                                                  FlowVector& source_flow) const {
         // calculate residual, divide, and assign to unmeasured (but connected) appliances
         ComplexValue<sym> const s_residual_per_appliance = (s - bus_appliance_injection.value) / (double)n_unmeasured;
         for (Idx load_gen = load_gen_begin; load_gen != load_gen_end; ++load_gen) {
             if (has_load_gen(load_gen)) {
                 load_gen_flow[load_gen].s = load_gen_power(load_gen).value;
-            }
-            else if (idx_load_gen_power_[load_gen] == unmeasured) {
+            } else if (idx_load_gen_power_[load_gen] == unmeasured) {
                 load_gen_flow[load_gen].s = s_residual_per_appliance;
             }
         }
         for (Idx source = source_begin; source != source_end; ++source) {
             if (has_source(source)) {
                 source_flow[source].s = source_power(source).value;
-            }
-            else if (idx_source_power_[source] == unmeasured) {
+            } else if (idx_source_power_[source] == unmeasured) {
                 source_flow[source].s = s_residual_per_appliance;
             }
         }
     }
 
     void calculate_over_determined_injection(Idx load_gen_begin, Idx load_gen_end, Idx source_begin, Idx source_end,
                                              SensorCalcParam<sym> const& bus_appliance_injection,
@@ -592,28 +521,26 @@
     }
 };
 
 template class MeasuredValues<true>;
 template class MeasuredValues<false>;
 
 // solver
-template <bool sym>
-class IterativeLinearSESolver {
+template <bool sym> class IterativeLinearSESolver {
     // block size 2 for symmetric, 6 for asym
     static constexpr Idx bsr_block_size_ = sym ? 2 : 6;
 
-   public:
+  public:
     IterativeLinearSESolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           math_topo_{topo_ptr},
           data_gain_(y_bus.nnz_lu()),
           x_rhs_(y_bus.size()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
-          perm_(y_bus.size()) {
-    }
+          perm_(y_bus.size()) {}
 
     MathOutput<sym> run_state_estimation(YBus<sym> const& y_bus, StateEstimationInput<sym> const& input, double err_tol,
                                          Idx max_iter, CalculationInfo& calculation_info) {
         // prepare
         Timer main_timer, sub_timer;
         MathOutput<sym> output;
         output.u.resize(n_bus_);
@@ -662,15 +589,15 @@
 
         const auto key = Timer::make_key(2228, "Max number of iterations");
         calculation_info[key] = std::max(calculation_info[key], (double)num_iter);
 
         return output;
     }
 
-   private:
+  private:
     // array selection function pointer
     static constexpr std::array has_branch_{&MeasuredValues<sym>::has_branch_from, &MeasuredValues<sym>::has_branch_to};
     static constexpr std::array branch_power_{&MeasuredValues<sym>::branch_from_power,
                                               &MeasuredValues<sym>::branch_to_power};
 
     Idx n_bus_;
     // shared topo data
@@ -845,16 +772,15 @@
         // if no angle measurement is present
         DoubleComplex const angle_offset = [&]() -> DoubleComplex {
             if (has_angle_measurement) {
                 return 1.0;
             }
             if constexpr (sym) {
                 return cabs(x_rhs_[math_topo_->slack_bus_].u()) / x_rhs_[math_topo_->slack_bus_].u();
-            }
-            else {
+            } else {
                 return cabs(x_rhs_[math_topo_->slack_bus_].u()(0)) / x_rhs_[math_topo_->slack_bus_].u()(0);
             }
         }();
 
         for (Idx bus = 0; bus != n_bus_; ++bus) {
             // phase offset to calculated voltage as normalized
             ComplexValue<sym> const u_normalized = x_rhs_[bus].u() * angle_offset;
@@ -876,15 +802,14 @@
             measured_value.calculate_load_gen_source(output.u, output.bus_injection);
     }
 };
 
 template class IterativeLinearSESolver<true>;
 template class IterativeLinearSESolver<false>;
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-template <bool sym>
-using IterativeLinearSESolver = math_model_impl::IterativeLinearSESolver<sym>;
+template <bool sym> using IterativeLinearSESolver = math_model_impl::IterativeLinearSESolver<sym>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,16 @@
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
 // solver
-template <bool sym, typename DerivedSolver>
-class IterativePFSolver {
-   public:
+template <bool sym, typename DerivedSolver> class IterativePFSolver {
+  public:
     friend DerivedSolver;
     MathOutput<sym> run_power_flow(YBus<sym> const& y_bus, PowerFlowInput<sym> const& input, double err_tol,
                                    Idx max_iter, CalculationInfo& calculation_info) {
         // get derived reference for derived solver class
         DerivedSolver& derived_solver = static_cast<DerivedSolver&>(*this);
         IdxVector const& source_bus_indptr = *source_bus_indptr_;
         std::vector<double> const& phase_shift = *phase_shift_;
@@ -47,15 +46,15 @@
         {
             Timer const sub_timer{calculation_info, 2221, "Initialize calculation"};
             // average u_ref of all sources
             DoubleComplex const u_ref = [&]() {
                 DoubleComplex sum_u_ref = 0.0;
                 for (Idx bus = 0; bus != n_bus_; ++bus) {
                     for (Idx source = source_bus_indptr[bus]; source != source_bus_indptr[bus + 1]; ++source) {
-                        sum_u_ref += input.source[source] * std::exp(1.0i * -phase_shift[bus]);  // offset phase shift
+                        sum_u_ref += input.source[source] * std::exp(1.0i * -phase_shift[bus]); // offset phase shift
                     }
                 }
                 return sum_u_ref / (double)input.source.size();
             }();
 
             // assign u_ref as flat start
             for (Idx i = 0; i != n_bus_; ++i) {
@@ -129,49 +128,48 @@
             // load_gen
             for (Idx load_gen = (*load_gen_bus_indptr_)[bus]; load_gen != (*load_gen_bus_indptr_)[bus + 1];
                  ++load_gen) {
                 LoadGenType const type = (*load_gen_type_)[load_gen];
                 switch (type) {
                     using enum LoadGenType;
 
-                    case const_pq:
-                        // always same power
-                        output.load_gen[load_gen].s = input.s_injection[load_gen];
-                        break;
-                    case const_y:
-                        // power is quadratic relation to voltage
-                        output.load_gen[load_gen].s =
-                            input.s_injection[load_gen] * cabs(output.u[bus]) * cabs(output.u[bus]);
-                        break;
-                    case const_i:
-                        // power is linear relation to voltage
-                        output.load_gen[load_gen].s = input.s_injection[load_gen] * cabs(output.u[bus]);
-                        break;
-                    default:
-                        throw MissingCaseForEnumError("Power injection", type);
+                case const_pq:
+                    // always same power
+                    output.load_gen[load_gen].s = input.s_injection[load_gen];
+                    break;
+                case const_y:
+                    // power is quadratic relation to voltage
+                    output.load_gen[load_gen].s =
+                        input.s_injection[load_gen] * cabs(output.u[bus]) * cabs(output.u[bus]);
+                    break;
+                case const_i:
+                    // power is linear relation to voltage
+                    output.load_gen[load_gen].s = input.s_injection[load_gen] * cabs(output.u[bus]);
+                    break;
+                default:
+                    throw MissingCaseForEnumError("Power injection", type);
                 }
                 output.load_gen[load_gen].i = conj(output.load_gen[load_gen].s / output.u[bus]);
             }
         }
         output.bus_injection = y_bus.calculate_injection(output.u);
     }
 
-   private:
+  private:
     Idx n_bus_;
     std::shared_ptr<DoubleVector const> phase_shift_;
     std::shared_ptr<IdxVector const> load_gen_bus_indptr_;
     std::shared_ptr<IdxVector const> source_bus_indptr_;
     std::shared_ptr<std::vector<LoadGenType> const> load_gen_type_;
     IterativePFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           phase_shift_{topo_ptr, &topo_ptr->phase_shift},
           load_gen_bus_indptr_{topo_ptr, &topo_ptr->load_gen_bus_indptr},
           source_bus_indptr_{topo_ptr, &topo_ptr->source_bus_indptr},
-          load_gen_type_{topo_ptr, &topo_ptr->load_gen_type} {
-    }
+          load_gen_type_{topo_ptr, &topo_ptr->load_gen_type} {}
 };
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,27 @@
 #include "../exception.hpp"
 #include "../power_grid_model.hpp"
 #include "../three_phase_tensor.hpp"
 #include "../timer.hpp"
 
 namespace power_grid_model {
 
-template <bool sym>
-class LinearPFSolver {
-   private:
+template <bool sym> class LinearPFSolver {
+  private:
     // block size 1 for symmetric, 3 for asym
     static constexpr Idx bsr_block_size_ = sym ? 1 : 3;
 
-   public:
+  public:
     LinearPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           load_gen_bus_indptr_{topo_ptr, &topo_ptr->load_gen_bus_indptr},
           source_bus_indptr_{topo_ptr, &topo_ptr->source_bus_indptr},
           mat_data_(y_bus.nnz_lu()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
-          perm_(n_bus_) {
-    }
+          perm_(n_bus_) {}
 
     MathOutput<sym> run_power_flow(YBus<sym> const& y_bus, PowerFlowInput<sym> const& input,
                                    CalculationInfo& calculation_info) {
         // getter
         ComplexTensorVector<sym> const& ydata = y_bus.admittance();
         IdxVector const& bus_entry = y_bus.lu_diag();
         // output
@@ -110,15 +108,15 @@
         sub_timer = Timer(calculation_info, 2223, "Calculate Math Result");
         calculate_result(y_bus, input, output);
 
         // output
         return output;
     }
 
-   private:
+  private:
     Idx n_bus_;
     // shared topo data
     std::shared_ptr<IdxVector const> load_gen_bus_indptr_;
     std::shared_ptr<IdxVector const> source_bus_indptr_;
     // sparse linear equation
     ComplexTensorVector<sym> mat_data_;
     // sparse solver
@@ -156,10 +154,10 @@
         output.bus_injection = y_bus.calculate_injection(output.u);
     }
 };
 
 template class LinearPFSolver<true>;
 template class LinearPFSolver<false>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,47 +19,44 @@
 #include "../three_phase_tensor.hpp"
 #include "../timer.hpp"
 
 #include <optional>
 
 namespace power_grid_model {
 
-template <bool sym>
-class MathSolver {
-   public:
+template <bool sym> class MathSolver {
+  public:
     MathSolver(std::shared_ptr<MathModelTopology const> const& topo_ptr,
                std::shared_ptr<MathModelParam<sym> const> const& param,
                std::shared_ptr<YBusStructure const> const& y_bus_struct = {})
         : topo_ptr_{topo_ptr},
           y_bus_{topo_ptr, param, y_bus_struct},
-          all_const_y_{std::all_of(topo_ptr->load_gen_type.cbegin(), topo_ptr->load_gen_type.cend(), [](LoadGenType x) {
-              return x == LoadGenType::const_y;
-          })} {
-    }
+          all_const_y_{std::all_of(topo_ptr->load_gen_type.cbegin(), topo_ptr->load_gen_type.cend(),
+                                   [](LoadGenType x) { return x == LoadGenType::const_y; })} {}
 
     MathOutput<sym> run_power_flow(PowerFlowInput<sym> const& input, double err_tol, Idx max_iter,
                                    CalculationInfo& calculation_info, CalculationMethod calculation_method) {
         using enum CalculationMethod;
 
         // set method to always linear if all load_gens have const_y
         calculation_method = all_const_y_ ? linear : calculation_method;
 
         switch (calculation_method) {
-            case default_method:
-                [[fallthrough]];  // use Newton-Raphson by default
-            case newton_raphson:
-                return run_power_flow_newton_raphson(input, err_tol, max_iter, calculation_info);
-            case linear:
-                return run_power_flow_linear(input, err_tol, max_iter, calculation_info);
-            case linear_current:
-                return run_power_flow_linear_current(input, err_tol, max_iter, calculation_info);
-            case iterative_current:
-                return run_power_flow_iterative_current(input, err_tol, max_iter, calculation_info);
-            default:
-                throw InvalidCalculationMethod{};
+        case default_method:
+            [[fallthrough]]; // use Newton-Raphson by default
+        case newton_raphson:
+            return run_power_flow_newton_raphson(input, err_tol, max_iter, calculation_info);
+        case linear:
+            return run_power_flow_linear(input, err_tol, max_iter, calculation_info);
+        case linear_current:
+            return run_power_flow_linear_current(input, err_tol, max_iter, calculation_info);
+        case iterative_current:
+            return run_power_flow_iterative_current(input, err_tol, max_iter, calculation_info);
+        default:
+            throw InvalidCalculationMethod{};
         }
     }
 
     MathOutput<sym> run_state_estimation(StateEstimationInput<sym> const& input, double err_tol, Idx max_iter,
                                          CalculationInfo& calculation_info, CalculationMethod calculation_method) {
         if (calculation_method != CalculationMethod::default_method &&
             calculation_method != CalculationMethod::iterative_linear) {
@@ -102,22 +99,20 @@
         iterative_linear_se_solver_.reset();
     }
 
     void update_value(std::shared_ptr<MathModelParam<sym> const> const& math_model_param) {
         y_bus_.update_admittance(math_model_param);
     }
 
-    std::shared_ptr<YBusStructure const> shared_y_bus_struct() const {
-        return y_bus_.shared_y_bus_struct();
-    }
+    std::shared_ptr<YBusStructure const> shared_y_bus_struct() const { return y_bus_.shared_y_bus_struct(); }
 
-   private:
+  private:
     std::shared_ptr<MathModelTopology const> topo_ptr_;
     YBus<sym> y_bus_;
-    bool all_const_y_;  // if all the load_gen is const element_admittance (impedance) type
+    bool all_const_y_; // if all the load_gen is const element_admittance (impedance) type
     std::optional<NewtonRaphsonPFSolver<sym>> newton_pf_solver_;
     std::optional<LinearPFSolver<sym>> linear_pf_solver_;
     std::optional<IterativeLinearSESolver<sym>> iterative_linear_se_solver_;
     std::optional<IterativeCurrentPFSolver<sym>> iterative_current_pf_solver_;
     std::optional<ShortCircuitSolver<sym>> iec60909_sc_solver_;
 
     MathOutput<sym> run_power_flow_newton_raphson(PowerFlowInput<sym> const& input, double err_tol, Idx max_iter,
@@ -152,10 +147,10 @@
         return run_power_flow_iterative_current(input, std::numeric_limits<double>::infinity(), 1, calculation_info);
     }
 };
 
 template class MathSolver<true>;
 template class MathSolver<false>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -159,85 +159,62 @@
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
 // class for phasor in polar coordinate and/or complex power
-template <bool sym>
-struct PolarPhasor : public Block<double, sym, false, 2> {
-    template <int r, int c>
-    using GetterType = typename Block<double, sym, false, 2>::template GetterType<r, c>;
+template <bool sym> struct PolarPhasor : public Block<double, sym, false, 2> {
+    template <int r, int c> using GetterType = typename Block<double, sym, false, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<double, sym, false, 2>::Block;
     using Block<double, sym, false, 2>::operator=;
 
-    GetterType<0, 0> theta() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<1, 0> v() {
-        return this->template get_val<1, 0>();
-    }
+    GetterType<0, 0> theta() { return this->template get_val<0, 0>(); }
+    GetterType<1, 0> v() { return this->template get_val<1, 0>(); }
 
-    GetterType<0, 0> p() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<1, 0> q() {
-        return this->template get_val<1, 0>();
-    }
+    GetterType<0, 0> p() { return this->template get_val<0, 0>(); }
+    GetterType<1, 0> q() { return this->template get_val<1, 0>(); }
 };
 
 // class for complex power
-template <bool sym>
-using ComplexPower = PolarPhasor<sym>;
+template <bool sym> using ComplexPower = PolarPhasor<sym>;
 
 // class of pf block
 // block of incomplete power flow jacobian
 // non-diagonal H, N, M, L
 // [ [H = dP/dTheta, N = V * dP/dV],
 // [M = dQ/dTheta = -N, L = V * dQ/dV = H] ]
 // Hij = Gij .* sij - Bij .* cij = L
 // Nij = Gij .* cij + Bij .* sij = -M
-template <bool sym>
-class PFJacBlock : public Block<double, sym, true, 2> {
-   public:
-    template <int r, int c>
-    using GetterType = typename Block<double, sym, true, 2>::template GetterType<r, c>;
+template <bool sym> class PFJacBlock : public Block<double, sym, true, 2> {
+  public:
+    template <int r, int c> using GetterType = typename Block<double, sym, true, 2>::template GetterType<r, c>;
 
     // eigen expression
     using Block<double, sym, true, 2>::Block;
     using Block<double, sym, true, 2>::operator=;
 
-    GetterType<0, 0> h() {
-        return this->template get_val<0, 0>();
-    }
-    GetterType<0, 1> n() {
-        return this->template get_val<0, 1>();
-    }
-    GetterType<1, 0> m() {
-        return this->template get_val<1, 0>();
-    }
-    GetterType<1, 1> l() {
-        return this->template get_val<1, 1>();
-    }
+    GetterType<0, 0> h() { return this->template get_val<0, 0>(); }
+    GetterType<0, 1> n() { return this->template get_val<0, 1>(); }
+    GetterType<1, 0> m() { return this->template get_val<1, 0>(); }
+    GetterType<1, 1> l() { return this->template get_val<1, 1>(); }
 };
 
 // solver
-template <bool sym>
-class NewtonRaphsonPFSolver : public IterativePFSolver<sym, NewtonRaphsonPFSolver<sym>> {
-   public:
+template <bool sym> class NewtonRaphsonPFSolver : public IterativePFSolver<sym, NewtonRaphsonPFSolver<sym>> {
+  public:
     NewtonRaphsonPFSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : IterativePFSolver<sym, NewtonRaphsonPFSolver>{y_bus, topo_ptr},
           data_jac_(y_bus.nnz_lu()),
           x_(y_bus.size()),
           del_x_pq_(y_bus.size()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
-          perm_(y_bus.size()) {
-    }
+          perm_(y_bus.size()) {}
 
     // Initilize the unknown variable in polar form
     void initialize_derived_solver(YBus<sym> const&, MathOutput<sym> const& output) {
         // get magnitude and angle of start voltage
         for (Idx i = 0; i != this->n_bus_; ++i) {
             x_[i].v() = cabs(output.u[i]);
             x_[i].theta() = arg(output.u[i]);
@@ -301,38 +278,38 @@
 
             // loop load
             for (Idx j = load_gen_bus_indptr[i]; j != load_gen_bus_indptr[i + 1]; ++j) {
                 // load type
                 LoadGenType const type = load_gen_type[j];
                 // modify jacobian and del_pq based on type
                 switch (type) {
-                    case LoadGenType::const_pq:
-                        // PQ_sp = PQ_base
-                        del_x_pq_[i].p() += real(input.s_injection[j]);
-                        del_x_pq_[i].q() += imag(input.s_injection[j]);
-                        // -dPQ_sp/dV * V = 0
-                        break;
-                    case LoadGenType::const_y:
-                        // PQ_sp = PQ_base * V^2
-                        del_x_pq_[i].p() += real(input.s_injection[j]) * x_[i].v() * x_[i].v();
-                        del_x_pq_[i].q() += imag(input.s_injection[j]) * x_[i].v() * x_[i].v();
-                        // -dPQ_sp/dV * V = -PQ_base * 2 * V^2
-                        add_diag(data_jac_[k].n(), -real(input.s_injection[j]) * 2.0 * x_[i].v() * x_[i].v());
-                        add_diag(data_jac_[k].l(), -imag(input.s_injection[j]) * 2.0 * x_[i].v() * x_[i].v());
-                        break;
-                    case LoadGenType::const_i:
-                        // PQ_sp = PQ_base * V
-                        del_x_pq_[i].p() += real(input.s_injection[j]) * x_[i].v();
-                        del_x_pq_[i].q() += imag(input.s_injection[j]) * x_[i].v();
-                        // -dPQ_sp/dV * V = -PQ_base * V
-                        add_diag(data_jac_[k].n(), -real(input.s_injection[j]) * x_[i].v());
-                        add_diag(data_jac_[k].l(), -imag(input.s_injection[j]) * x_[i].v());
-                        break;
-                    default:
-                        throw MissingCaseForEnumError("Jacobian and deviation calculation", type);
+                case LoadGenType::const_pq:
+                    // PQ_sp = PQ_base
+                    del_x_pq_[i].p() += real(input.s_injection[j]);
+                    del_x_pq_[i].q() += imag(input.s_injection[j]);
+                    // -dPQ_sp/dV * V = 0
+                    break;
+                case LoadGenType::const_y:
+                    // PQ_sp = PQ_base * V^2
+                    del_x_pq_[i].p() += real(input.s_injection[j]) * x_[i].v() * x_[i].v();
+                    del_x_pq_[i].q() += imag(input.s_injection[j]) * x_[i].v() * x_[i].v();
+                    // -dPQ_sp/dV * V = -PQ_base * 2 * V^2
+                    add_diag(data_jac_[k].n(), -real(input.s_injection[j]) * 2.0 * x_[i].v() * x_[i].v());
+                    add_diag(data_jac_[k].l(), -imag(input.s_injection[j]) * 2.0 * x_[i].v() * x_[i].v());
+                    break;
+                case LoadGenType::const_i:
+                    // PQ_sp = PQ_base * V
+                    del_x_pq_[i].p() += real(input.s_injection[j]) * x_[i].v();
+                    del_x_pq_[i].q() += imag(input.s_injection[j]) * x_[i].v();
+                    // -dPQ_sp/dV * V = -PQ_base * V
+                    add_diag(data_jac_[k].n(), -real(input.s_injection[j]) * x_[i].v());
+                    add_diag(data_jac_[k].l(), -imag(input.s_injection[j]) * x_[i].v());
+                    break;
+                default:
+                    throw MissingCaseForEnumError("Jacobian and deviation calculation", type);
                 }
             }
 
             // loop source
             for (Idx j = source_bus_indptr[i]; j != source_bus_indptr[i + 1]; ++j) {
                 ComplexTensor<sym> const y_ref = y_bus.math_model_param().source_param[j];
                 ComplexValue<sym> const u_ref{input.source[j]};
@@ -359,17 +336,15 @@
                 data_jac_[k].m() += block_mm.m();
                 data_jac_[k].l() += block_mm.l();
             }
         }
     }
 
     // Solve the linear Equations
-    void solve_matrix() {
-        sparse_solver_.prefactorize_and_solve(data_jac_, perm_, del_x_pq_, del_x_pq_);
-    }
+    void solve_matrix() { sparse_solver_.prefactorize_and_solve(data_jac_, perm_, del_x_pq_, del_x_pq_); }
 
     // Get maximum deviation among all bus voltages
     double iterate_unknown(ComplexValueVector<sym>& u) {
         double max_dev = 0.0;
         // loop each bus as i
         for (Idx i = 0; i != this->n_bus_; ++i) {
             // angle
@@ -384,19 +359,19 @@
             max_dev = std::max(dev, max_dev);
             // assign
             u[i] = u_tmp;
         }
         return max_dev;
     }
 
-   private:
+  private:
     // data for jacobian
     std::vector<PFJacBlock<sym>> data_jac_;
     // calculation data
-    std::vector<PolarPhasor<sym>> x_;  // unknown
+    std::vector<PolarPhasor<sym>> x_; // unknown
     // this stores in different steps
     // 1. negative power injection: - p/q_calculated
     // 2. power unbalance: p/q_specified - p/q_calculated
     // 3. unknown iterative
     std::vector<ComplexPower<sym>> del_x_pq_;
     SparseLUSolver<PFJacBlock<sym>, ComplexPower<sym>, PolarPhasor<sym>> sparse_solver_;
     // permutation array
@@ -432,15 +407,14 @@
         return block;
     }
 };
 
 template class NewtonRaphsonPFSolver<true>;
 template class NewtonRaphsonPFSolver<false>;
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-template <bool sym>
-using NewtonRaphsonPFSolver = math_model_impl::NewtonRaphsonPFSolver<sym>;
+template <bool sym> using NewtonRaphsonPFSolver = math_model_impl::NewtonRaphsonPFSolver<sym>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
 // solver
-template <bool sym>
-class ShortCircuitSolver {
+template <bool sym> class ShortCircuitSolver {
     using BlockPermArray =
         typename SparseLUSolver<ComplexTensor<sym>, ComplexValue<sym>, ComplexValue<sym>>::BlockPermArray;
 
-   public:
+  public:
     ShortCircuitSolver(YBus<sym> const& y_bus, std::shared_ptr<MathModelTopology const> const& topo_ptr)
         : n_bus_{y_bus.size()},
           n_source_{topo_ptr->n_source()},
           source_bus_indptr_{topo_ptr, &topo_ptr->source_bus_indptr},
           mat_data_(y_bus.nnz_lu()),
           sparse_solver_{y_bus.shared_indptr_lu(), y_bus.shared_indices_lu(), y_bus.shared_diag_lu()},
-          perm_{static_cast<BlockPermArray>(n_bus_)} {
-    }
+          perm_{static_cast<BlockPermArray>(n_bus_)} {}
 
     ShortCircuitMathOutput<sym> run_short_circuit(double voltage_scaling_factor_c, YBus<sym> const& y_bus,
                                                   ShortCircuitInput const& input) {
         check_input_valid(input);
 
         auto [fault_type, fault_phase] = extract_fault_type_phase(input.faults);
 
@@ -70,51 +68,50 @@
             auto& diagonal_element = mat_data_[diagonal_position];
             auto& u_bus = output.u_bus[bus_number];
 
             // add all sources
             for (Idx source_number = source_bus_indptr[bus_number]; source_number != source_bus_indptr[bus_number + 1];
                  ++source_number) {
                 ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
-                diagonal_element += y_source;  // add y_source to the diagonal of Ybus
+                diagonal_element += y_source; // add y_source to the diagonal of Ybus
                 u_bus += dot(y_source, ComplexValue<sym>{input.source[source_number] *
-                                                         voltage_scaling_factor_c});  // rhs += Y_source * U_source * c
+                                                         voltage_scaling_factor_c}); // rhs += Y_source * U_source * c
             }
             // skip if no fault
             if (!input.faults.empty()) {
                 // add all faults
                 for (Idx fault_number = fault_bus_indptr[bus_number]; fault_number != fault_bus_indptr[bus_number + 1];
                      ++fault_number) {
                     DoubleComplex const y_fault = input.faults[fault_number].y_fault;
                     if (std::isinf(y_fault.real())) {
                         assert(std::isinf(y_fault.imag()));
                         infinite_admittance_fault_counter[bus_number] += 1;
-                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                        if (fault_type == FaultType::three_phase) { // three phase fault
                             for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                  data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                 Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                                 // mat_data[:,bus] = 0
                                 mat_data_[col_data_index] = ComplexTensor<sym>{0};
                             }
                             // mat_data[bus,bus] = -1
                             diagonal_element = ComplexTensor<sym>{-1};
-                            u_bus = ComplexValue<sym>{0};  // update rhs
+                            u_bus = ComplexValue<sym>{0}; // update rhs
                         }
                         if constexpr (!sym) {
                             if (fault_type == FaultType::single_phase_to_ground) {
                                 for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                      data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                     Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                                     // mat_data[:,bus][:, phase_1] = 0
                                     mat_data_[col_data_index].col(phase_1) = 0;
                                 }
                                 // mat_data[bus,bus][phase_1, phase_1] = -1
                                 diagonal_element(phase_1, phase_1) = -1;
-                                u_bus(phase_1) = 0;  // update rhs
-                            }
-                            else if (fault_type == FaultType::two_phase) {
+                                u_bus(phase_1) = 0; // update rhs
+                            } else if (fault_type == FaultType::two_phase) {
                                 for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                      data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                     Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                                     // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
                                     // mat_data[:,bus][:, phase_2] = 0
                                     mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
                                     mat_data_[col_data_index].col(phase_2) = 0;
@@ -122,16 +119,15 @@
                                 // mat_data[bus,bus][phase_1, phase_2] = -1
                                 // mat_data[bus,bus][phase_2, phase_2] = 1
                                 diagonal_element(phase_1, phase_2) = -1;
                                 diagonal_element(phase_2, phase_2) = 1;
                                 // update rhs
                                 u_bus(phase_2) += u_bus(phase_1);
                                 u_bus(phase_1) = 0;
-                            }
-                            else if (fault_type == FaultType::two_phase_to_ground) {
+                            } else if (fault_type == FaultType::two_phase_to_ground) {
                                 for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                      data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                     Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                                     // mat_data[:,bus][:, phase_1] = 0
                                     // mat_data[:,bus][:, phase_2] = 0
                                     mat_data_[col_data_index].col(phase_1) = 0;
                                     mat_data_[col_data_index].col(phase_2) = 0;
@@ -139,45 +135,42 @@
                                 // mat_data[bus,bus][phase_1, phase_1] = -1
                                 // mat_data[bus,bus][phase_2, phase_2] = -1
                                 diagonal_element(phase_1, phase_1) = -1;
                                 diagonal_element(phase_2, phase_2) = -1;
                                 // update rhs
                                 u_bus(phase_1) = 0;
                                 u_bus(phase_2) = 0;
-                            }
-                            else {
+                            } else {
                                 assert((fault_type == FaultType::three_phase));
                                 continue;
                             }
                         }
                         // If there is a fault with infinite admittance, there is no need to add other faults to that
                         // bus
                         break;
                     }
                     assert(!std::isinf(y_fault.imag()));
-                    if (fault_type == FaultType::three_phase) {  // three phase fault
+                    if (fault_type == FaultType::three_phase) { // three phase fault
                         // mat_data[bus,bus] += y_fault
                         diagonal_element += ComplexTensor<sym>{y_fault};
                     }
                     if constexpr (!sym) {
                         if (fault_type == FaultType::single_phase_to_ground) {
                             // mat_data[bus,bus][phase_1, phase_1] += y_fault
                             diagonal_element(phase_1, phase_1) += y_fault;
-                        }
-                        else if (fault_type == FaultType::two_phase) {
+                        } else if (fault_type == FaultType::two_phase) {
                             // mat_data[bus,bus][phase_1, phase_1] += y_fault
                             // mat_data[bus,bus][phase_2, phase_2] += y_fault
                             // mat_data[bus,bus][phase_1, phase_2] -= y_fault
                             // mat_data[bus,bus][phase_2, phase_1] -= y_fault
                             diagonal_element(phase_1, phase_1) += y_fault;
                             diagonal_element(phase_2, phase_2) += y_fault;
                             diagonal_element(phase_1, phase_2) -= y_fault;
                             diagonal_element(phase_2, phase_1) -= y_fault;
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
+                        } else if (fault_type == FaultType::two_phase_to_ground) {
                             for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                  data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                 Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
                                 // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
                                 // mat_data[:,bus][:, phase_2] = 0
                                 mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
                                 mat_data_[col_data_index].col(phase_2) = 0;
@@ -187,16 +180,15 @@
                             // mat_data[bus,bus][phase_2, phase_2] = 1
                             diagonal_element(phase_1, phase_2) = -1;
                             diagonal_element(phase_2, phase_2) = 1;
                             diagonal_element(phase_2, phase_1) += y_fault;
                             // update rhs
                             u_bus(phase_2) += u_bus(phase_1);
                             u_bus(phase_1) = 0;
-                        }
-                        else {
+                        } else {
                             assert((fault_type == FaultType::three_phase));
                             continue;
                         }
                     }
                 }
             }
         }
@@ -207,15 +199,15 @@
         // post processing
         calculate_result(y_bus, input, output, infinite_admittance_fault_counter, fault_type, phase_1, phase_2,
                          voltage_scaling_factor_c);
 
         return output;
     }
 
-   private:
+  private:
     Idx n_bus_;
     Idx n_fault_;
     Idx n_source_;
     // shared topo data
     std::shared_ptr<IdxVector const> source_bus_indptr_;
     // sparse linear equation
     ComplexTensorVector<sym> mat_data_;
@@ -237,81 +229,74 @@
                      fault_number != input.fault_bus_indptr[bus_number + 1]; ++fault_number) {
                     auto& i_fault = output.fault[fault_number].i_fault;
                     auto& u_bus = output.u_bus[bus_number];
                     DoubleComplex const y_fault = input.faults[fault_number].y_fault;
 
                     if (std::isinf(y_fault.real())) {
                         assert(std::isinf(y_fault.imag()));
-                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                        if (fault_type == FaultType::three_phase) { // three phase fault
                             i_fault = -1.0 * static_cast<ComplexValue<sym>>(x_bus_subtotal) /
-                                      infinite_admittance_fault_counter_bus;  // injection is
-                                                                              // negative to fault
+                                      infinite_admittance_fault_counter_bus; // injection is
+                                                                             // negative to fault
                             u_bus = ComplexValue<sym>{0.0};
                         }
                         if constexpr (!sym) {
                             if (fault_type == FaultType::single_phase_to_ground) {
                                 i_fault(phase_1) =
                                     -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
                                 u_bus(phase_1) = 0.0;
-                            }
-                            else if (fault_type == FaultType::two_phase) {
+                            } else if (fault_type == FaultType::two_phase) {
                                 i_fault(phase_1) =
                                     -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
                                 i_fault(phase_2) = -1.0 * i_fault(phase_1);
                                 u_bus(phase_2) = u_bus(phase_1);
-                            }
-                            else if (fault_type == FaultType::two_phase_to_ground) {
+                            } else if (fault_type == FaultType::two_phase_to_ground) {
                                 i_fault(phase_1) =
                                     -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
                                 i_fault(phase_2) =
                                     -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
                                 u_bus(phase_1) = 0.0;
                                 u_bus(phase_2) = 0.0;
-                            }
-                            else {
+                            } else {
                                 assert((fault_type == FaultType::three_phase));
                                 continue;
                             }
                         }
-                    }
-                    else {
+                    } else {
                         assert(!std::isinf(y_fault.imag()));
                         if (infinite_admittance_fault_counter[bus_number] > 0) {
                             // ignore fault objects with impedance, when there is a fault with infinite admittance on
                             // bus
                             continue;
                         }
-                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                        if (fault_type == FaultType::three_phase) { // three phase fault
                             i_fault = static_cast<ComplexValue<sym>>(y_fault * x_bus_subtotal);
                         }
                         if constexpr (!sym) {
                             if (fault_type == FaultType::single_phase_to_ground) {
                                 i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1];
-                            }
-                            else if (fault_type == FaultType::two_phase) {
+                            } else if (fault_type == FaultType::two_phase) {
                                 i_fault(phase_1) =
                                     y_fault * x_bus_subtotal[phase_1] - y_fault * x_bus_subtotal[phase_2];
                                 i_fault(phase_2) =
                                     y_fault * x_bus_subtotal[phase_2] - y_fault * x_bus_subtotal[phase_1];
-                            }
-                            else if (fault_type == FaultType::two_phase_to_ground) {
+                            } else if (fault_type == FaultType::two_phase_to_ground) {
                                 i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2];
                                 i_fault(phase_2) = -1.0 * i_fault(phase_1) + y_fault * x_bus_subtotal[phase_1];
                                 u_bus(phase_2) = u_bus(phase_1);
-                            }
-                            else {
+                            } else {
                                 assert((fault_type == FaultType::three_phase));
                                 continue;
                             }
                         }
                     }
                 }
 
-                ComplexValue<sym> i_source_bus{};     // total source current in to the bus
-                ComplexValue<sym> i_source_inject{};  // total raw source current as a Norton equivalent
+                ComplexValue<sym> i_source_bus{};    // total source current in to the bus
+                ComplexValue<sym> i_source_inject{}; // total raw source current as a Norton equivalent
                 for (Idx source_number = (*source_bus_indptr_)[bus_number];
                      source_number != (*source_bus_indptr_)[bus_number + 1]; ++source_number) {
                     ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
                     ComplexValue<sym> const i_source_inject_single =
                         dot(y_source, ComplexValue<sym>{input.source[source_number] * voltage_scaling_factor_c});
                     output.source[source_number].i = i_source_inject_single - dot(y_source, output.u_bus[bus_number]);
                     i_source_bus += output.source[source_number].i;
@@ -330,36 +315,32 @@
                         if (fault_type == FaultType::three_phase) {
                             i_fault +=
                                 static_cast<ComplexValue<sym>>(i_source_bus / infinite_admittance_fault_counter_bus);
                         }
                         if constexpr (!sym) {
                             if (fault_type == FaultType::single_phase_to_ground) {
                                 i_fault(phase_1) += i_source_bus[phase_1] / infinite_admittance_fault_counter_bus;
-                            }
-                            else if (fault_type == FaultType::two_phase) {
+                            } else if (fault_type == FaultType::two_phase) {
                                 i_fault(phase_1) += i_source_inject[phase_1] / infinite_admittance_fault_counter_bus;
                                 // i_inj_1 + i_inj_2 = i_ref_1 + i_ref_2
                                 // i_fault_2_p = i_inj_1
                                 //      i_fault_2_p is the i_fault_2 status quo after the first fault loop
                                 // i_inj_2 = - i_inj_1 + i_ref_1 + i_ref_2
                                 // i_fault_2 = i_ref_2 - i_inj_2 = i_ref_2 + i_inj_1 - i_ref_1 - i_ref_2
                                 //           = i_inj_1 - i_ref_1 = i_fault_2_p - i_ref_1
                                 i_fault(phase_2) -= i_source_inject[phase_1] / infinite_admittance_fault_counter_bus;
-                            }
-                            else if (fault_type == FaultType::two_phase_to_ground) {
+                            } else if (fault_type == FaultType::two_phase_to_ground) {
                                 i_fault(phase_1) += i_source_bus[phase_1];
                                 i_fault(phase_2) += i_source_bus[phase_2];
-                            }
-                            else {
+                            } else {
                                 assert((fault_type == FaultType::three_phase));
                                 continue;
                             }
                         }
-                    }
-                    else {
+                    } else {
                         // compensate for 2 phase to ground fault with impedance
                         assert(!std::isinf(y_fault.imag()));
                         if constexpr (!sym) {
                             if ((fault_type == FaultType::two_phase_to_ground) &&
                                 (infinite_admittance_fault_counter_bus == 0.0)) {
                                 double const finite_admittance_fault_counter_bus = static_cast<double>(
                                     input.fault_bus_indptr[bus_number + 1] - input.fault_bus_indptr[bus_number]);
@@ -388,43 +369,43 @@
         IntS phase_2{-1};
 
         // This function updates the phase index for single and two phase faults
 
         using enum FaultPhase;
 
         switch (fault_phase) {
-            case a: {
-                phase_1 = 0;
-                break;
-            }
-            case b: {
-                phase_1 = 1;
-                break;
-            }
-            case c: {
-                phase_1 = 2;
-                break;
-            }
-            case ab: {
-                phase_1 = 0;
-                phase_2 = 1;
-                break;
-            }
-            case ac: {
-                phase_1 = 0;
-                phase_2 = 2;
-                break;
-            }
-            case bc: {
-                phase_1 = 1;
-                phase_2 = 2;
-                break;
-            }
-            default:
-                break;
+        case a: {
+            phase_1 = 0;
+            break;
+        }
+        case b: {
+            phase_1 = 1;
+            break;
+        }
+        case c: {
+            phase_1 = 2;
+            break;
+        }
+        case ab: {
+            phase_1 = 0;
+            phase_2 = 1;
+            break;
+        }
+        case ac: {
+            phase_1 = 0;
+            phase_2 = 2;
+            break;
+        }
+        case bc: {
+            phase_1 = 1;
+            phase_2 = 2;
+            break;
+        }
+        default:
+            break;
         }
 
         return std::make_pair(phase_1, phase_2);
     }
 
     static constexpr auto extract_fault_type_phase(std::vector<FaultCalcParam> const& faults) {
         if (faults.empty()) {
@@ -460,15 +441,14 @@
         });
     }
 };
 
 template class ShortCircuitSolver<true>;
 template class ShortCircuitSolver<false>;
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-template <bool sym>
-using ShortCircuitSolver = math_model_impl::ShortCircuitSolver<sym>;
+template <bool sym> using ShortCircuitSolver = math_model_impl::ShortCircuitSolver<sym>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,115 +13,110 @@
 #include <memory>
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
-template <class Tensor, class RHSVector, class XVector, class = void>
-struct sparse_lu_entry_trait;
+template <class Tensor, class RHSVector, class XVector, class = void> struct sparse_lu_entry_trait;
 
 template <class Tensor, class RHSVector, class XVector>
 concept scalar_value_lu = scalar_value<Tensor> && std::same_as<Tensor, RHSVector> && std::same_as<Tensor, XVector>;
 
 // TODO(mgovers) improve this concept
-template <class Derived>
-int check_array_base(Eigen::ArrayBase<Derived> const&) {
-    return 0;
-}
+template <class Derived> int check_array_base(Eigen::ArrayBase<Derived> const&) { return 0; }
 template <class ArrayLike>
-concept eigen_array = std::same_as<decltype(check_array_base(ArrayLike{})), int>;  // should be an eigen array
+concept eigen_array = std::same_as<decltype(check_array_base(ArrayLike{})), int>; // should be an eigen array
 
 template <class LHSArrayLike, class RHSArrayLike>
 concept matrix_multiplicable = eigen_array<LHSArrayLike> && eigen_array<RHSArrayLike> &&
-    (static_cast<Idx>(LHSArrayLike::ColsAtCompileTime) == static_cast<Idx>(RHSArrayLike::RowsAtCompileTime));
+                               (static_cast<Idx>(LHSArrayLike::ColsAtCompileTime) ==
+                                static_cast<Idx>(RHSArrayLike::RowsAtCompileTime));
 
 template <class Tensor, class RHSVector, class XVector>
-concept tensor_lu = rk2_tensor<Tensor> && column_vector<RHSVector> && column_vector<XVector> &&
+concept tensor_lu =
+    rk2_tensor<Tensor> && column_vector<RHSVector> && column_vector<XVector> &&
     matrix_multiplicable<Tensor, RHSVector> && matrix_multiplicable<Tensor, XVector> &&
-    std::same_as<typename Tensor::Scalar, typename RHSVector::Scalar> &&  // all entries should have same scalar type
-    std::same_as<typename Tensor::Scalar, typename XVector::Scalar> &&    // all entries should have same scalar type
-    scalar_value<typename Tensor::Scalar>;                                // scalar can only be double or complex double
+    std::same_as<typename Tensor::Scalar, typename RHSVector::Scalar> && // all entries should have same scalar type
+    std::same_as<typename Tensor::Scalar, typename XVector::Scalar> &&   // all entries should have same scalar type
+    scalar_value<typename Tensor::Scalar>;                               // scalar can only be double or complex double
 
 template <class Tensor, class RHSVector, class XVector>
-requires scalar_value_lu<Tensor, RHSVector, XVector>
+    requires scalar_value_lu<Tensor, RHSVector, XVector>
 struct sparse_lu_entry_trait<Tensor, RHSVector, XVector> {
     static constexpr bool is_block = false;
     static constexpr Idx block_size = 1;
     using Scalar = Tensor;
     using Matrix = Tensor;
     using LUFactor = void;
     struct BlockPerm {};
     using BlockPermArray = Idx;
 };
 
 template <class Tensor, class RHSVector, class XVector>
-requires tensor_lu<Tensor, RHSVector, XVector>
+    requires tensor_lu<Tensor, RHSVector, XVector>
 struct sparse_lu_entry_trait<Tensor, RHSVector, XVector> {
     static constexpr bool is_block = true;
     static constexpr Idx block_size = Tensor::RowsAtCompileTime;
     using Scalar = typename Tensor::Scalar;
     using Matrix = Eigen::Matrix<Scalar, block_size, block_size, Tensor::Options>;
-    using LUFactor = Eigen::FullPivLU<Eigen::Ref<Matrix>>;  // LU decomposition with full pivoting in place
+    using LUFactor = Eigen::FullPivLU<Eigen::Ref<Matrix>>; // LU decomposition with full pivoting in place
     struct BlockPerm {
         typename LUFactor::PermutationPType p;
         typename LUFactor::PermutationQType q;
-    };  // Extract permutation matrices p and q from LUFactor
+    }; // Extract permutation matrices p and q from LUFactor
     using BlockPermArray = std::vector<BlockPerm>;
 };
 
-template <class Tensor, class RHSVector, class XVector>
-class SparseLUSolver {
-   public:
+template <class Tensor, class RHSVector, class XVector> class SparseLUSolver {
+  public:
     using entry_trait = sparse_lu_entry_trait<Tensor, RHSVector, XVector>;
     static constexpr bool is_block = entry_trait::is_block;
     static constexpr Idx block_size = entry_trait::block_size;
     using Scalar = typename entry_trait::Scalar;
     using LUFactor = typename entry_trait::LUFactor;
     using BlockPerm = typename entry_trait::BlockPerm;
     using BlockPermArray = typename entry_trait::BlockPermArray;
 
-    SparseLUSolver(std::shared_ptr<IdxVector const> const& row_indptr,   // indptr including fill-ins
-                   std::shared_ptr<IdxVector const> const& col_indices,  // indices including fill-ins
+    SparseLUSolver(std::shared_ptr<IdxVector const> const& row_indptr,  // indptr including fill-ins
+                   std::shared_ptr<IdxVector const> const& col_indices, // indices including fill-ins
                    std::shared_ptr<IdxVector const> const& diag_lu)
         : size_{(Idx)row_indptr->size() - 1},
           nnz_{row_indptr->back()},
           row_indptr_{row_indptr},
           col_indices_{col_indices},
-          diag_lu_{diag_lu} {
-    }
+          diag_lu_{diag_lu} {}
 
     // solve with new matrix data, need to factorize first
-    void prefactorize_and_solve(
-        std::vector<Tensor>& data,         // matrix data, factorize in-place
-        BlockPermArray& block_perm_array,  // pre-allocated permutation array, will be overwritten
-        std::vector<RHSVector> const& rhs, std::vector<XVector>& x) {
+    void
+    prefactorize_and_solve(std::vector<Tensor>& data,        // matrix data, factorize in-place
+                           BlockPermArray& block_perm_array, // pre-allocated permutation array, will be overwritten
+                           std::vector<RHSVector> const& rhs, std::vector<XVector>& x) {
         prefactorize(data, block_perm_array);
         // call solve with const method
         solve_with_prefactorized_matrix((std::vector<Tensor> const&)data, block_perm_array, rhs, x);
     }
 
     // solve with existing pre-factorization
-    void solve_with_prefactorized_matrix(
-        std::vector<Tensor> const& data,         // pre-factoirzed data, const ref
-        BlockPermArray const& block_perm_array,  // pre-calculated permutation, const ref
-        std::vector<RHSVector> const& rhs, std::vector<XVector>& x) {
+    void
+    solve_with_prefactorized_matrix(std::vector<Tensor> const& data,        // pre-factoirzed data, const ref
+                                    BlockPermArray const& block_perm_array, // pre-calculated permutation, const ref
+                                    std::vector<RHSVector> const& rhs, std::vector<XVector>& x) {
         // local reference
         auto const& row_indptr = *row_indptr_;
         auto const& col_indices = *col_indices_;
         auto const& diag_lu = *diag_lu_;
         auto const& lu_matrix = data;
 
         // forward substitution with L
         for (Idx row = 0; row != size_; ++row) {
             // permutation if needed
             if constexpr (is_block) {
                 x[row] = (block_perm_array[row].p * rhs[row].matrix()).array();
-            }
-            else {
+            } else {
                 x[row] = rhs[row];
             }
 
             // loop all columns until diagonal
             for (Idx l_idx = row_indptr[row]; l_idx < diag_lu[row]; ++l_idx) {
                 Idx const col = col_indices[l_idx];
                 // never overshoot
@@ -158,16 +153,15 @@
                 Tensor const& pivot = lu_matrix[diag_lu[row]];
                 for (Idx br = block_size - 1; br != -1; --br) {
                     for (Idx bc = block_size - 1; bc > br; --bc) {
                         xb(br) -= pivot(br, bc) * xb(bc);
                     }
                     xb(br) = xb(br) / pivot(br, br);
                 }
-            }
-            else {
+            } else {
                 x[row] = x[row] / lu_matrix[diag_lu[row]];
             }
         }
         // restore permutation for block matrix
         if constexpr (is_block) {
             for (Idx row = 0; row != size_; ++row) {
                 x[row] = (block_perm_array[row].q * x[row].matrix()).array();
@@ -206,16 +200,15 @@
                     lu_factor.setThreshold(1e-100);
                     if (lu_factor.rank() < block_size) {
                         throw SparseMatrixError{};
                     }
                     // record block permutation
                     block_perm_array[pivot_row_col] = {lu_factor.permutationP(), lu_factor.permutationQ()};
                     return block_perm_array[pivot_row_col];
-                }
-                else {
+                } else {
                     if (lu_matrix[pivot_idx] == 0.0) {
                         throw SparseMatrixError{};
                     }
                     return {};
                 }
             }();
             // reference to pivot
@@ -293,16 +286,15 @@
                     for (Idx block_col = 0; block_col < block_size; ++block_col) {
                         for (Idx block_row = 0; block_row < block_col; ++block_row) {
                             l.col(block_col) -= pivot(block_row, block_col) * l.col(block_row);
                         }
                         // divide diagonal
                         l.col(block_col) = l.col(block_col) / pivot(block_col, block_col);
                     }
-                }
-                else {
+                } else {
                     // for scalar matrix, just divide
                     // L_k,pivot = A_k,pivot / U_pivot    k > pivot
                     lu_matrix[l_idx] = lu_matrix[l_idx] / pivot;
                 }
                 Tensor const& l = lu_matrix[l_idx];
 
                 // for all entries in the right of (l_row, u_col)
@@ -330,23 +322,23 @@
                 ++col_position_idx[l_row];
             }
             // iterate column position for the pivot
             ++col_position_idx[pivot_row_col];
         }
     }
 
-   private:
+  private:
     Idx size_;
-    Idx nnz_;  // number of non zeroes (in block)
+    Idx nnz_; // number of non zeroes (in block)
     std::shared_ptr<IdxVector const> row_indptr_;
     std::shared_ptr<IdxVector const> col_indices_;
     std::shared_ptr<IdxVector const> diag_lu_;
 };
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
 template <class Tensor, class RHSVector, class XVector>
 using SparseLUSolver = math_model_impl::SparseLUSolver<Tensor, RHSVector, XVector>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #include "../three_phase_tensor.hpp"
 
 namespace power_grid_model {
 
 // hide implementation in inside namespace
 namespace math_model_impl {
 
-using OffDiagIdxMap = std::array<Idx, 2>;  // map of ft and tf for branch
+using OffDiagIdxMap = std::array<Idx, 2>; // map of ft and tf for branch
 
 using MatrixPos = std::pair<Idx, Idx>;
 
 struct YBusElementMap {
     MatrixPos pos;
     YBusElement element;
 };
@@ -106,16 +106,16 @@
         // add element
         // off diagonal element list
         std::vector<OffDiagIdxMap> off_diag_map(n_branch + n_fill_in);
         // loop branch
         for (Idx branch = 0; branch != n_branch; ++branch) {
             // ff, ft, tf, tt for branch
             for (IntS i = 0; i != 4; ++i) {
-                Idx const bus1 = topo.branch_bus_idx[branch][i / 2];  // 0, 0, 1, 1
-                Idx const bus2 = topo.branch_bus_idx[branch][i % 2];  // 0, 1, 0, 1
+                Idx const bus1 = topo.branch_bus_idx[branch][i / 2]; // 0, 0, 1, 1
+                Idx const bus2 = topo.branch_bus_idx[branch][i % 2]; // 0, 1, 0, 1
                 append_element_vector(vec_map_element, bus1, bus2, static_cast<YBusElementType>(i), branch);
             }
         }
         // loop shunt
         for (Idx bus = 0; bus != n_bus; ++bus) {
             for (Idx shunt = topo.shunt_bus_indptr[bus]; shunt != topo.shunt_bus_indptr[bus + 1]; ++shunt) {
                 append_element_vector(vec_map_element, bus, bus, YBusElementType::shunt, shunt);
@@ -192,16 +192,16 @@
                 // record off diag entry
                 if (row != col) {
                     off_diag_map[it_element->element.idx]
                                 // minus 1 because ft is 1 and tf is 2, mapped to 0 and 1
                                 [static_cast<Idx>(it_element->element.element_type) - 1] = nnz_counter_lu;
                 }
                 // inner loop of elements in the same position
-                for (  // use it_element to start
-                    ;  // stop when reach end or new position
+                for ( // use it_element to start
+                    ; // stop when reach end or new position
                     it_element != vec_map_element.cend() && it_element->pos == pos; ++it_element) {
                     // no fill-ins are allowed
                     assert(it_element->element.element_type != YBusElementType::fill_in_ft &&
                            it_element->element.element_type != YBusElementType::fill_in_tf);
                 }
                 // all entries in the same position are looped, append indptr
                 // need to be offset by fill-in
@@ -267,105 +267,59 @@
             lu_transpose_entry[entry_1] = entry_2;
             lu_transpose_entry[entry_2] = entry_1;
         }
     }
 };
 
 // See also "Node Admittance Matrix" in "State Estimation Alliander"
-template <bool sym>
-class YBus {
-   public:
+template <bool sym> class YBus {
+  public:
     YBus(std::shared_ptr<MathModelTopology const> const& topo_ptr,
          std::shared_ptr<MathModelParam<sym> const> const& param,
          std::shared_ptr<YBusStructure const> const& y_bus_struct = {})
         : math_topology_{topo_ptr} {
         // use existing struct or make new struct
         if (y_bus_struct) {
             y_bus_struct_ = y_bus_struct;
-        }
-        else {
+        } else {
             y_bus_struct_ = std::make_shared<YBusStructure const>(YBusStructure{*topo_ptr});
         }
         // update values
         update_admittance(param);
     }
 
     // getter
-    Idx size() const {
-        return (Idx)bus_entry().size();
-    }
-    Idx nnz() const {
-        return row_indptr().back();
-    }
-    Idx nnz_lu() const {
-        return row_indptr_lu().back();
-    }
-    IdxVector const& row_indptr() const {
-        return y_bus_struct_->row_indptr;
-    }
-    IdxVector const& col_indices() const {
-        return y_bus_struct_->col_indices;
-    }
-    IdxVector const& row_indptr_lu() const {
-        return y_bus_struct_->row_indptr_lu;
-    }
-    IdxVector const& col_indices_lu() const {
-        return y_bus_struct_->col_indices_lu;
-    }
-    IdxVector const& lu_transpose_entry() const {
-        return y_bus_struct_->lu_transpose_entry;
-    }
-    std::vector<YBusElement> const& y_bus_element() const {
-        return y_bus_struct_->y_bus_element;
-    }
-    IdxVector const& y_bus_entry_indptr() const {
-        return y_bus_struct_->y_bus_entry_indptr;
-    }
-    MathModelTopology const& math_topology() const {
-        return *math_topology_;
-    }
-    MathModelParam<sym> const& math_model_param() const {
-        return *math_model_param_;
-    }
-
-    ComplexTensorVector<sym> const& admittance() const {
-        return *admittance_;
-    }
-    IdxVector const& bus_entry() const {
-        return y_bus_struct_->bus_entry;
-    }
-    IdxVector const& lu_diag() const {
-        return y_bus_struct_->diag_lu;
-    }
-    IdxVector const& map_lu_y_bus() const {
-        return y_bus_struct_->map_lu_y_bus;
-    }
+    Idx size() const { return (Idx)bus_entry().size(); }
+    Idx nnz() const { return row_indptr().back(); }
+    Idx nnz_lu() const { return row_indptr_lu().back(); }
+    IdxVector const& row_indptr() const { return y_bus_struct_->row_indptr; }
+    IdxVector const& col_indices() const { return y_bus_struct_->col_indices; }
+    IdxVector const& row_indptr_lu() const { return y_bus_struct_->row_indptr_lu; }
+    IdxVector const& col_indices_lu() const { return y_bus_struct_->col_indices_lu; }
+    IdxVector const& lu_transpose_entry() const { return y_bus_struct_->lu_transpose_entry; }
+    std::vector<YBusElement> const& y_bus_element() const { return y_bus_struct_->y_bus_element; }
+    IdxVector const& y_bus_entry_indptr() const { return y_bus_struct_->y_bus_entry_indptr; }
+    MathModelTopology const& math_topology() const { return *math_topology_; }
+    MathModelParam<sym> const& math_model_param() const { return *math_model_param_; }
+
+    ComplexTensorVector<sym> const& admittance() const { return *admittance_; }
+    IdxVector const& bus_entry() const { return y_bus_struct_->bus_entry; }
+    IdxVector const& lu_diag() const { return y_bus_struct_->diag_lu; }
+    IdxVector const& map_lu_y_bus() const { return y_bus_struct_->map_lu_y_bus; }
 
     // getter of shared ptr
-    std::shared_ptr<IdxVector const> shared_indptr() const {
-        return {y_bus_struct_, &y_bus_struct_->row_indptr};
-    }
-    std::shared_ptr<IdxVector const> shared_indices() const {
-        return {y_bus_struct_, &y_bus_struct_->col_indices};
-    }
-    std::shared_ptr<MathModelTopology const> shared_topology() const {
-        return math_topology_;
-    }
-    std::shared_ptr<YBusStructure const> shared_y_bus_struct() const {
-        return y_bus_struct_;
-    }
-    std::shared_ptr<IdxVector const> shared_indptr_lu() const {
-        return {y_bus_struct_, &y_bus_struct_->row_indptr_lu};
-    }
+    std::shared_ptr<IdxVector const> shared_indptr() const { return {y_bus_struct_, &y_bus_struct_->row_indptr}; }
+    std::shared_ptr<IdxVector const> shared_indices() const { return {y_bus_struct_, &y_bus_struct_->col_indices}; }
+    std::shared_ptr<MathModelTopology const> shared_topology() const { return math_topology_; }
+    std::shared_ptr<YBusStructure const> shared_y_bus_struct() const { return y_bus_struct_; }
+    std::shared_ptr<IdxVector const> shared_indptr_lu() const { return {y_bus_struct_, &y_bus_struct_->row_indptr_lu}; }
     std::shared_ptr<IdxVector const> shared_indices_lu() const {
         return {y_bus_struct_, &y_bus_struct_->col_indices_lu};
     }
-    std::shared_ptr<IdxVector const> shared_diag_lu() const {
-        return {y_bus_struct_, &y_bus_struct_->diag_lu};
-    }
+    std::shared_ptr<IdxVector const> shared_diag_lu() const { return {y_bus_struct_, &y_bus_struct_->diag_lu}; }
 
     void update_admittance(std::shared_ptr<MathModelParam<sym> const> const& math_model_param) {
         // overwrite the old cached parameters
         math_model_param_ = math_model_param;
         // construct admittance data
         ComplexTensorVector<sym> admittance(nnz());
         auto const& branch_param = math_model_param_->branch_param;
@@ -377,16 +331,15 @@
             // start admittance accumulation with zero
             ComplexTensor<sym> entry_admittance{0.0};
             // loop over all entries of this position
             for (Idx element = y_bus_entry_indptr[entry]; element != y_bus_entry_indptr[entry + 1]; ++element) {
                 if (y_bus_element[element].element_type == YBusElementType::shunt) {
                     // shunt
                     entry_admittance += shunt_param[y_bus_element[element].idx];
-                }
-                else {
+                } else {
                     // branch
                     entry_admittance += branch_param[y_bus_element[element].idx]
                                             .value[static_cast<Idx>(y_bus_element[element].element_type)];
                 }
             }
             // assign
             admittance[entry] = entry_admittance;
@@ -396,33 +349,29 @@
     }
 
     ComplexValue<sym> calculate_injection(ComplexValueVector<sym> const& u, Idx bus_number) const {
         Idx const begin = row_indptr()[bus_number];
         Idx const end = row_indptr()[bus_number + 1];
         ComplexValue<sym> const i_inj = std::transform_reduce(
             col_indices().cbegin() + begin, col_indices().cbegin() + end, admittance().cbegin() + begin,
-            ComplexValue<sym>{0.0}, std::plus{}, [&u](Idx j, ComplexTensor<sym> const& y) {
-                return dot(y, u[j]);
-            });
+            ComplexValue<sym>{0.0}, std::plus{}, [&u](Idx j, ComplexTensor<sym> const& y) { return dot(y, u[j]); });
         return conj(i_inj) * u[bus_number];
     }
 
     ComplexValueVector<sym> calculate_injection(ComplexValueVector<sym> const& u) const {
         ComplexValueVector<sym> s(size());
-        std::transform(IdxCount{0}, IdxCount{size()}, s.begin(), [this, &u](Idx bus) {
-            return calculate_injection(u, bus);
-        });
+        std::transform(IdxCount{0}, IdxCount{size()}, s.begin(),
+                       [this, &u](Idx bus) { return calculate_injection(u, bus); });
         return s;
     }
 
     // calculate branch flow based on voltage
     template <typename T>
-    requires std::same_as<T, BranchMathOutput<sym>> || std::same_as<T, BranchShortCircuitMathOutput<sym>> std::vector<T>
-    calculate_branch_flow(ComplexValueVector<sym> const& u)
-    const {
+        requires std::same_as<T, BranchMathOutput<sym>> || std::same_as<T, BranchShortCircuitMathOutput<sym>>
+    std::vector<T> calculate_branch_flow(ComplexValueVector<sym> const& u) const {
         std::vector<T> branch_flow(math_topology_->branch_bus_idx.size());
         std::transform(math_topology_->branch_bus_idx.cbegin(), math_topology_->branch_bus_idx.cend(),
                        math_model_param_->branch_param.cbegin(), branch_flow.begin(),
                        [&u](BranchIdx branch_idx, BranchCalcParam<sym> const& param) {
                            auto const [f, t] = branch_idx;
                            // if one side is disconnected, use zero voltage at that side
                            ComplexValue<sym> const uf = f != -1 ? u[f] : ComplexValue<sym>{0.0};
@@ -442,18 +391,17 @@
                            return output;
                        });
         return branch_flow;
     }
 
     // calculate shunt flow based on voltage, injection direction
     template <typename MathOutputType>
-    requires std::same_as<MathOutputType, ApplianceMathOutput<sym>> ||
-        std::same_as<MathOutputType, ApplianceShortCircuitMathOutput<sym>>
-            std::vector<MathOutputType> calculate_shunt_flow(ComplexValueVector<sym> const& u)
-    const {
+        requires std::same_as<MathOutputType, ApplianceMathOutput<sym>> ||
+                 std::same_as<MathOutputType, ApplianceShortCircuitMathOutput<sym>>
+    std::vector<MathOutputType> calculate_shunt_flow(ComplexValueVector<sym> const& u) const {
         std::vector<MathOutputType> shunt_flow(math_topology_->n_shunt());
         // loop all bus, then all shunt within the bus
         for (Idx bus = 0; bus != size(); ++bus) {
             for (Idx shunt = math_topology_->shunt_bus_indptr[bus]; shunt != math_topology_->shunt_bus_indptr[bus + 1];
                  ++shunt) {
                 // See "Branch/Shunt Power Flow" in "State Estimation Alliander"
                 // NOTE: the negative sign for injection direction!
@@ -464,15 +412,15 @@
                     shunt_flow[shunt].s = u[bus] * conj(shunt_flow[shunt].i);
                 }
             }
         }
         return shunt_flow;
     }
 
-   private:
+  private:
     // csr structure
     std::shared_ptr<YBusStructure const> y_bus_struct_;
 
     // admittance
     std::shared_ptr<ComplexTensorVector<sym> const> admittance_;
 
     // cache math topology
@@ -481,17 +429,16 @@
     // cache the math parameters
     std::shared_ptr<MathModelParam<sym> const> math_model_param_;
 };
 
 template class YBus<true>;
 template class YBus<false>;
 
-}  // namespace math_model_impl
+} // namespace math_model_impl
 
-template <bool sym>
-using YBus = math_model_impl::YBus<sym>;
+template <bool sym> using YBus = math_model_impl::YBus<sym>;
 
 using YBusStructure = math_model_impl::YBusStructure;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 using IntS = int8_t;
 
 // couting iterator
 using IdxCount = boost::counting_iterator<Idx>;
 
 // struct of indexing to sub modules
 struct Idx2D {
-    Idx group;  // sequence number of outer module/groups
-    Idx pos;    //  sequence number inside the group
+    Idx group; // sequence number of outer module/groups
+    Idx pos;   //  sequence number inside the group
 
     friend constexpr bool operator==(Idx2D x, Idx2D y) = default;
 };
 
 // math constant
 using namespace std::complex_literals;
 using DoubleComplex = std::complex<double>;
@@ -68,41 +68,38 @@
 constexpr double nan = std::numeric_limits<double>::quiet_NaN();
 constexpr IntS na_IntS = std::numeric_limits<IntS>::min();
 constexpr ID na_IntID = std::numeric_limits<ID>::min();
 
 // power grid constant
 constexpr double base_power_3p = 1e6;
 constexpr double base_power_1p = base_power_3p / 3.0;
-template <bool sym>
-constexpr double u_scale = sym ? 1.0 : inv_sqrt3;
-template <bool sym>
-constexpr double base_power = sym ? base_power_3p : base_power_1p;
+template <bool sym> constexpr double u_scale = sym ? 1.0 : inv_sqrt3;
+template <bool sym> constexpr double base_power = sym ? base_power_3p : base_power_1p;
 // links are direct line between nodes with infinite element_admittance in theory
 // for numerical calculation, a big link element_admittance is assigned
 // 1e6 Siemens element_admittance in 10kV network
 constexpr double g_link = 1e6 / (base_power_3p / 10e3 / 10e3);
 constexpr DoubleComplex y_link{g_link, g_link};
 // default source short circuit power
-constexpr double default_source_sk = 1e10;  // 10 GVA 10^10
+constexpr double default_source_sk = 1e10; // 10 GVA 10^10
 constexpr double default_source_rx_ratio = 0.1;
 constexpr double default_source_z01_ratio = 1.0;
 
 // calculation info
 using CalculationInfo = std::map<std::string, double>;
 using Clock = std::chrono::high_resolution_clock;
 using Duration = std::chrono::duration<double>;
 
 // some usual vector
 using DoubleVector = std::vector<double>;
 using ComplexVector = std::vector<std::complex<double>>;
 using IntSVector = std::vector<IntS>;
 
 // component list
-template <class... T>
-struct ComponentList {};
+template <class... T> struct ComponentList {};
 
 // batch parameter
 struct BatchParameter {};
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -75,10 +75,10 @@
         sparse_mapping.reorder[--counter[it_entry->second]] = it_entry->first;
     }
     assert(sparse_mapping.indptr[0] == 0);
     assert(sparse_mapping.indptr.back() == n_A);
     return sparse_mapping;
 }
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -20,92 +20,65 @@
 
 // enable scalar
 template <class T>
 concept scalar_value = std::same_as<T, double> || std::same_as<T, DoubleComplex>;
 
 namespace three_phase_tensor {
 
-template <class T>
-using Eigen3Vector = Eigen::Array<T, 3, 1>;
-template <class T>
-using Eigen3Tensor = Eigen::Array<T, 3, 3, Eigen::ColMajor>;
+template <class T> using Eigen3Vector = Eigen::Array<T, 3, 1>;
+template <class T> using Eigen3Tensor = Eigen::Array<T, 3, 3, Eigen::ColMajor>;
 
-template <scalar_value T>
-class Vector : public Eigen3Vector<T> {
-   public:
-    Vector() {
-        (*this) = Eigen3Vector<T>::Zero();
-    };
+template <scalar_value T> class Vector : public Eigen3Vector<T> {
+  public:
+    Vector() { (*this) = Eigen3Vector<T>::Zero(); };
     // eigen expression
-    template <typename OtherDerived>
-    Vector(Eigen::ArrayBase<OtherDerived> const& other) : Eigen3Vector<T>{other} {
-    }
-    template <typename OtherDerived>
-    Vector& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
+    template <typename OtherDerived> Vector(Eigen::ArrayBase<OtherDerived> const& other) : Eigen3Vector<T>{other} {}
+    template <typename OtherDerived> Vector& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
         this->Eigen3Vector<T>::operator=(other);
         return *this;
     }
     // constructor of single value
     // for complex number, rotate the single value by 120 and 240 degrees for 1st and 2nd entry
     // this will create a symmetric phasor based on one phasor
     explicit Vector(T const& x) {
         if constexpr (std::same_as<T, double>) {
             (*this) << x, x, x;
-        }
-        else {
+        } else {
             (*this) << x, (x * a2), (x * a);
         }
     }
     // piecewise constructor of single value
     // for both real and complex number, the value is repeated three times (without rotation)
-    explicit Vector(std::piecewise_construct_t, T const& x) {
-        (*this) << x, x, x;
-    }
+    explicit Vector(std::piecewise_construct_t, T const& x) { (*this) << x, x, x; }
     // constructor of three values
-    Vector(T const& x1, T const& x2, T const& x3) {
-        (*this) << x1, x2, x3;
-    }
+    Vector(T const& x1, T const& x2, T const& x3) { (*this) << x1, x2, x3; }
 };
 
-template <scalar_value T>
-class Tensor : public Eigen3Tensor<T> {
-   public:
-    Tensor() {
-        (*this) = Eigen3Tensor<T>::Zero();
-    }
+template <scalar_value T> class Tensor : public Eigen3Tensor<T> {
+  public:
+    Tensor() { (*this) = Eigen3Tensor<T>::Zero(); }
     // additional constructors
-    explicit Tensor(T const& x) {
-        (*this) << x, 0.0, 0.0, 0.0, x, 0.0, 0.0, 0.0, x;
-    }
-    explicit Tensor(T const& s, T const& m) {
-        (*this) << s, m, m, m, s, m, m, m, s;
-    }
-    explicit Tensor(Vector<T> const& v) {
-        (*this) << v(0), 0.0, 0.0, 0.0, v(1), 0.0, 0.0, 0.0, v(2);
-    }
+    explicit Tensor(T const& x) { (*this) << x, 0.0, 0.0, 0.0, x, 0.0, 0.0, 0.0, x; }
+    explicit Tensor(T const& s, T const& m) { (*this) << s, m, m, m, s, m, m, m, s; }
+    explicit Tensor(Vector<T> const& v) { (*this) << v(0), 0.0, 0.0, 0.0, v(1), 0.0, 0.0, 0.0, v(2); }
     // eigen expression
-    template <typename OtherDerived>
-    Tensor(Eigen::ArrayBase<OtherDerived> const& other) : Eigen3Tensor<T>{other} {
-    }
-    template <typename OtherDerived>
-    Tensor& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
+    template <typename OtherDerived> Tensor(Eigen::ArrayBase<OtherDerived> const& other) : Eigen3Tensor<T>{other} {}
+    template <typename OtherDerived> Tensor& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
         this->Eigen3Tensor<T>::operator=(other);
         return *this;
     }
 };
 
-}  // namespace three_phase_tensor
+} // namespace three_phase_tensor
 
 // three phase vector and tensor
-template <bool sym>
-using RealTensor = std::conditional_t<sym, double, three_phase_tensor::Tensor<double>>;
+template <bool sym> using RealTensor = std::conditional_t<sym, double, three_phase_tensor::Tensor<double>>;
 template <bool sym>
 using ComplexTensor = std::conditional_t<sym, DoubleComplex, three_phase_tensor::Tensor<DoubleComplex>>;
-template <bool sym>
-using RealValue = std::conditional_t<sym, double, three_phase_tensor::Vector<double>>;
+template <bool sym> using RealValue = std::conditional_t<sym, double, three_phase_tensor::Vector<double>>;
 template <bool sym>
 using ComplexValue = std::conditional_t<sym, DoubleComplex, three_phase_tensor::Vector<DoubleComplex>>;
 // asserts to ensure alignment
 static_assert(sizeof(RealTensor<false>) == sizeof(double[9]));
 static_assert(alignof(RealTensor<false>) == alignof(double[9]));
 static_assert(std::is_standard_layout_v<RealTensor<false>>);
 static_assert(std::is_trivially_destructible_v<RealTensor<false>>);
@@ -123,202 +96,136 @@
 static_assert(std::is_trivially_destructible_v<ComplexValue<false>>);
 
 // enabler
 template <class T>
 concept column_vector = (T::ColsAtCompileTime == 1);
 template <class T>
 concept rk2_tensor = (static_cast<Idx>(T::RowsAtCompileTime) ==
-                      static_cast<Idx>(T::ColsAtCompileTime));  // rank 2 tensor
+                      static_cast<Idx>(T::ColsAtCompileTime)); // rank 2 tensor
 template <class T>
 concept column_vector_or_tensor = column_vector<T> || rk2_tensor<T>;
 
 // piecewise factory construction for complex vector
-template <bool sym = false>
-inline ComplexValue<sym> piecewise_complex_value(DoubleComplex const& x) {
+template <bool sym = false> inline ComplexValue<sym> piecewise_complex_value(DoubleComplex const& x) {
     if constexpr (sym) {
         return x;
-    }
-    else {
+    } else {
         return ComplexValue<false>{std::piecewise_construct, x};
     }
 }
 
 template <column_vector DerivedA>
 inline ComplexValue<false> piecewise_complex_value(Eigen::ArrayBase<DerivedA> const& val) {
     return val;
 }
 
 // abs
-inline double cabs(double x) {
-    return std::abs(x);
-}
-inline double cabs(DoubleComplex const& x) {
-    return std::sqrt(std::norm(x));
-}
-inline double abs2(DoubleComplex const& x) {
-    return std::norm(x);
-}
-template <column_vector_or_tensor DerivedA>
-inline auto cabs(Eigen::ArrayBase<DerivedA> const& m) {
+inline double cabs(double x) { return std::abs(x); }
+inline double cabs(DoubleComplex const& x) { return std::sqrt(std::norm(x)); }
+inline double abs2(DoubleComplex const& x) { return std::norm(x); }
+template <column_vector_or_tensor DerivedA> inline auto cabs(Eigen::ArrayBase<DerivedA> const& m) {
     return sqrt(abs2(m));
 }
 
 // calculate kron product of two vector
-inline double vector_outer_product(double x, double y) {
-    return x * y;
-}
+inline double vector_outer_product(double x, double y) { return x * y; }
 template <column_vector DerivedA, column_vector DerivedB>
 inline auto vector_outer_product(Eigen::ArrayBase<DerivedA> const& x, Eigen::ArrayBase<DerivedB> const& y) {
     return (x.matrix() * y.matrix().transpose()).array();
 }
 
 // calculate matrix multiply, dot
-inline double dot(double x, double y) {
-    return x * y;
-}
-inline DoubleComplex dot(DoubleComplex const& x, DoubleComplex const& y) {
-    return x * y;
-}
+inline double dot(double x, double y) { return x * y; }
+inline DoubleComplex dot(DoubleComplex const& x, DoubleComplex const& y) { return x * y; }
 
-template <scalar_value... T>
-inline auto dot(T const&... x) {
-    return (... * x);
-}
+template <scalar_value... T> inline auto dot(T const&... x) { return (... * x); }
 
-template <column_vector_or_tensor... Derived>
-inline auto dot(Eigen::ArrayBase<Derived> const&... x) {
+template <column_vector_or_tensor... Derived> inline auto dot(Eigen::ArrayBase<Derived> const&... x) {
     auto res_mat = (... * x.matrix());
     return res_mat.array();
 }
 
 // max of a vector
-inline double max_val(double val) {
-    return val;
-}
-template <column_vector DerivedA>
-inline double max_val(Eigen::ArrayBase<DerivedA> const& val) {
+inline double max_val(double val) { return val; }
+template <column_vector DerivedA> inline double max_val(Eigen::ArrayBase<DerivedA> const& val) {
     return val.maxCoeff();
 }
 
 // function to sum rows of tensor
-template <rk2_tensor DerivedA>
-inline auto sum_row(Eigen::ArrayBase<DerivedA> const& m) {
-    return m.rowwise().sum();
-}
+template <rk2_tensor DerivedA> inline auto sum_row(Eigen::ArrayBase<DerivedA> const& m) { return m.rowwise().sum(); }
 // overload for double
-inline double sum_row(double d) {
-    return d;
-}
+inline double sum_row(double d) { return d; }
 
 // function to sum vector
-template <column_vector DerivedA>
-inline auto sum_val(Eigen::ArrayBase<DerivedA> const& m) {
-    return m.sum();
-}
+template <column_vector DerivedA> inline auto sum_val(Eigen::ArrayBase<DerivedA> const& m) { return m.sum(); }
 // overload for double and complex
-inline double sum_val(double d) {
-    return d;
-}
-inline DoubleComplex sum_val(DoubleComplex const& z) {
-    return z;
-}
+inline double sum_val(double d) { return d; }
+inline DoubleComplex sum_val(DoubleComplex const& z) { return z; }
 
 // function to mean vector
-template <column_vector DerivedA>
-inline auto mean_val(Eigen::ArrayBase<DerivedA> const& m) {
-    return m.mean();
-}
-inline DoubleComplex mean_val(DoubleComplex const& z) {
-    return z;
-}
-inline double mean_val(double z) {
-    return z;
-}
+template <column_vector DerivedA> inline auto mean_val(Eigen::ArrayBase<DerivedA> const& m) { return m.mean(); }
+inline DoubleComplex mean_val(DoubleComplex const& z) { return z; }
+inline double mean_val(double z) { return z; }
 
-template <bool sym, class T>
-inline auto process_mean_val(const T& m) {
+template <bool sym, class T> inline auto process_mean_val(const T& m) {
     if constexpr (sym) {
         return mean_val(m);
-    }
-    else {
+    } else {
         return m;
     }
 }
 
 // diagonal multiply
 template <column_vector DerivedA, rk2_tensor DerivedB, column_vector DerivedC>
 inline auto diag_mult(Eigen::ArrayBase<DerivedA> const& x, Eigen::ArrayBase<DerivedB> const& y,
                       Eigen::ArrayBase<DerivedC> const& z) {
     return (x.matrix().asDiagonal() * y.matrix() * z.matrix().asDiagonal()).array();
 }
 // double overload
-inline double diag_mult(double x, double y, double z) {
-    return x * y * z;
-}
+inline double diag_mult(double x, double y, double z) { return x * y * z; }
 
 // calculate positive sequence
-template <column_vector Derived>
-inline DoubleComplex pos_seq(Eigen::ArrayBase<Derived> const& val) {
+template <column_vector Derived> inline DoubleComplex pos_seq(Eigen::ArrayBase<Derived> const& val) {
     return (val(0) + a * val(1) + a2 * val(2)) / 3.0;
 }
 
-inline DoubleComplex pos_seq(DoubleComplex const& val) {
-    return val;
-}
+inline DoubleComplex pos_seq(DoubleComplex const& val) { return val; }
 
 // inverse of tensor
-inline DoubleComplex inv(DoubleComplex const& val) {
-    return 1.0 / val;
-}
-inline auto inv(ComplexTensor<false> const& val) {
-    return val.matrix().inverse().array();
-}
+inline DoubleComplex inv(DoubleComplex const& val) { return 1.0 / val; }
+inline auto inv(ComplexTensor<false> const& val) { return val.matrix().inverse().array(); }
 
 // add_diag
-inline void add_diag(double& x, double y) {
-    x += y;
-}
-inline void add_diag(DoubleComplex& x, DoubleComplex const& y) {
-    x += y;
-}
+inline void add_diag(double& x, double y) { x += y; }
+inline void add_diag(DoubleComplex& x, DoubleComplex const& y) { x += y; }
 template <rk2_tensor DerivedA, column_vector DerivedB>
 inline void add_diag(Eigen::ArrayBase<DerivedA>& x, Eigen::ArrayBase<DerivedB> const& y) {
     x.matrix().diagonal() += y.matrix();
 }
 template <rk2_tensor DerivedA, column_vector DerivedB>
 inline void add_diag(Eigen::ArrayBase<DerivedA>&& x, Eigen::ArrayBase<DerivedB> const& y) {
     x.matrix().diagonal() += y.matrix();
 }
 
 // zero tensor
-template <bool sym>
-inline const ComplexTensor<sym> zero_tensor = ComplexTensor<sym>{0.0};
+template <bool sym> inline const ComplexTensor<sym> zero_tensor = ComplexTensor<sym>{0.0};
 
 // inverse symmetric param
 inline std::pair<DoubleComplex, DoubleComplex> inv_sym_param(DoubleComplex const& s, DoubleComplex const& m) {
     DoubleComplex const det_1 = 1.0 / (s * s + s * m - 2.0 * m * m);
     return {(s + m) * det_1, -m * det_1};
 }
 
 // is nan
-template <class Derived>
-inline bool is_nan(Eigen::ArrayBase<Derived> const& x) {
-    return x.isNaN().all();
-}
-inline bool is_nan(double x) {
-    return std::isnan(x);
-}
-inline bool is_nan(ID x) {
-    return x == na_IntID;
-}
-inline bool is_nan(IntS x) {
-    return x == na_IntS;
-}
+template <class Derived> inline bool is_nan(Eigen::ArrayBase<Derived> const& x) { return x.isNaN().all(); }
+inline bool is_nan(double x) { return std::isnan(x); }
+inline bool is_nan(ID x) { return x == na_IntID; }
+inline bool is_nan(IntS x) { return x == na_IntS; }
 template <class Enum>
-requires std::same_as<std::underlying_type_t<Enum>, IntS>
+    requires std::same_as<std::underlying_type_t<Enum>, IntS>
 inline bool is_nan(Enum x) {
     return static_cast<IntS>(x) == na_IntS;
 }
 
 /* update real values
 
    RealValue is only updated when the update value is not nan
@@ -332,16 +239,15 @@
 */
 template <bool sym, class Proxy>
 void update_real_value(RealValue<sym> const& new_value, Proxy&& current_value, double scalar) {
     if constexpr (sym) {
         if (!is_nan(new_value)) {
             current_value = scalar * new_value;
         }
-    }
-    else {
+    } else {
         for (size_t i = 0; i != 3; ++i) {
             if (!is_nan(new_value(i))) {
                 current_value(i) = scalar * new_value(i);
             }
         }
     }
 }
@@ -356,31 +262,22 @@
     ComplexTensor<false> m;
     m << 1.0, 1.0, 1.0, 1.0, a, a2, 1.0, a2, a;
     m = m / 3.0;
     return m;
 }
 
 // conjugate (hermitian) transpose
-inline DoubleComplex hermitian_transpose(DoubleComplex const& z) {
-    return conj(z);
-}
-inline double hermitian_transpose(double x) {
-    return x;
-}
-template <rk2_tensor Derived>
-inline auto hermitian_transpose(Eigen::ArrayBase<Derived> const& x) {
+inline DoubleComplex hermitian_transpose(DoubleComplex const& z) { return conj(z); }
+inline double hermitian_transpose(double x) { return x; }
+template <rk2_tensor Derived> inline auto hermitian_transpose(Eigen::ArrayBase<Derived> const& x) {
     return x.matrix().adjoint().array();
 }
 
 // vector of values
-template <bool sym>
-using RealValueVector = std::vector<RealValue<sym>>;
-template <bool sym>
-using ComplexValueVector = std::vector<ComplexValue<sym>>;
-template <bool sym>
-using RealTensorVector = std::vector<RealTensor<sym>>;
-template <bool sym>
-using ComplexTensorVector = std::vector<ComplexTensor<sym>>;
+template <bool sym> using RealValueVector = std::vector<RealValue<sym>>;
+template <bool sym> using ComplexValueVector = std::vector<ComplexValue<sym>>;
+template <bool sym> using RealTensorVector = std::vector<RealTensor<sym>>;
+template <bool sym> using ComplexTensorVector = std::vector<ComplexTensor<sym>>;
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 
 #include <iomanip>
 #include <sstream>
 
 namespace power_grid_model {
 
 class Timer {
-   private:
-    CalculationInfo *info_;
+  private:
+    CalculationInfo* info_;
     int code_;
     std::string name_;
     Clock::time_point start_;
 
-   public:
+  public:
     Timer() : info_(nullptr){};
 
-    Timer(CalculationInfo &info, int code, std::string name)
-        : info_(&info), code_(code), name_(std::move(name)), start_(Clock::now()) {
-    }
+    Timer(CalculationInfo& info, int code, std::string name)
+        : info_(&info), code_(code), name_(std::move(name)), start_(Clock::now()) {}
 
-    Timer(const Timer &) = delete;
-    Timer(Timer &&) = default;
-    Timer &operator=(const Timer &) = delete;
+    Timer(const Timer&) = delete;
+    Timer(Timer&&) = default;
+    Timer& operator=(const Timer&) = delete;
 
-    Timer &operator=(Timer &&timer) noexcept {
+    Timer& operator=(Timer&& timer) noexcept {
         // Stop the current timer
         stop();
 
         // Copy/move members
         info_ = timer.info_;
         code_ = timer.code_;
         name_ = std::move(timer.name_);
@@ -59,25 +58,25 @@
             auto const now = Clock::now();
             auto const duration = Duration(now - start_);
             info_->operator[](Timer::make_key(code_, name_)) += (double)duration.count();
             info_ = nullptr;
         }
     }
 
-    static std::string make_key(int code, const std::string &name) {
+    static std::string make_key(int code, const std::string& name) {
         std::stringstream ss;
         ss << std::setw(4) << std::setfill('0') << code << ".";
         auto key = ss.str();
         for (size_t i = 0, n = key.length() - 1; i < n; ++i) {
             if (key[i] == '0') {
                 break;
             }
             key += "\t";
         }
         key += name;
         return key;
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
-#endif  // POWER_GRID_MODEL_TIMER_HPP
+#endif // POWER_GRID_MODEL_TIMER_HPP
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -42,31 +42,30 @@
     // for 3-way branch, the internal node is appended at the end one by one
     // n_node + k, k as branch3 sequence number
     // branch3 #0, has internal node idx n_node
     // branch3 #1, has internal node idx n_node + 1
     using GlobalGraph = boost::compressed_sparse_row_graph<boost::directedS, GlobalVertex, GlobalEdge,
                                                            boost::no_property, GraphIdx, GraphIdx>;
 
-    using ReorderGraph = boost::adjacency_list<boost::vecS,  // vector as adjacency
-                                               boost::vecS,  // vector for vertices
+    using ReorderGraph = boost::adjacency_list<boost::vecS, // vector as adjacency
+                                               boost::vecS, // vector for vertices
                                                boost::directedS>;
 
     // dfs visitor for global graph
     class GlobalDFSVisitor : public boost::dfs_visitor<> {
-       public:
+      public:
         GlobalDFSVisitor(Idx math_group, std::vector<Idx2D>& node_coupling, std::vector<double>& phase_shift,
                          std::vector<Idx>& dfs_node, std::vector<GraphIdx>& predecessors,
                          std::vector<std::pair<GraphIdx, GraphIdx>>& back_edges)
             : math_group_{math_group},
               node_coupling_{node_coupling},
               phase_shift_{phase_shift},
               dfs_node_{dfs_node},
               predecessors_{predecessors},
-              back_edges_{back_edges} {
-        }
+              back_edges_{back_edges} {}
 
         // accumulate phase shift
         // assign predecessor
         void tree_edge(GlobalGraph::edge_descriptor e, GlobalGraph const& g) {
             GraphIdx const source = boost::source(e, g), target = boost::target(e, g);
             phase_shift_[target] = phase_shift_[source] + g[e].phase_shift;
             predecessors_[target] = source;
@@ -91,33 +90,32 @@
         // assign node to math group
         // append node to dfs list
         void discover_vertex(GlobalGraph::vertex_descriptor u, GlobalGraph const&) {
             node_coupling_[u].group = (Idx)math_group_;
             dfs_node_.push_back((Idx)u);
         }
 
-       private:
+      private:
         Idx math_group_;
         std::vector<Idx2D>& node_coupling_;
         std::vector<double>& phase_shift_;
         std::vector<Idx>& dfs_node_;
         std::vector<GraphIdx>& predecessors_;
         std::vector<std::pair<GraphIdx, GraphIdx>>& back_edges_;
     };
 
-   public:
+  public:
     Topology(ComponentTopology const& comp_topo, ComponentConnections const& comp_conn)
         : comp_topo_{comp_topo},
           comp_conn_{comp_conn},
           phase_shift_(comp_topo_.n_node_total(), 0.0),
           predecessors_(
-              boost::counting_iterator<GraphIdx>{0},  // Predecessors is initialized as 0, 1, 2, ..., n_node_total() - 1
+              boost::counting_iterator<GraphIdx>{0}, // Predecessors is initialized as 0, 1, 2, ..., n_node_total() - 1
               boost::counting_iterator<GraphIdx>{(GraphIdx)comp_topo_.n_node_total()}),
-          node_status_(comp_topo_.n_node_total(), -1) {
-    }
+          node_status_(comp_topo_.n_node_total(), -1) {}
 
     // build topology
     std::pair<std::vector<std::shared_ptr<MathModelTopology const>>,
               std::shared_ptr<TopologicalComponentToMathCoupling const>>
     build_topology() {
         reset_topology();
         build_sparse_graph();
@@ -132,15 +130,15 @@
         for (Idx k = 0; k != (Idx)math_topology_.size(); ++k) {
             pair.first.emplace_back(std::make_shared<MathModelTopology const>(std::move(math_topology_[k])));
         }
         pair.second = std::make_shared<TopologicalComponentToMathCoupling const>(std::move(comp_coup_));
         return pair;
     }
 
-   private:
+  private:
     // input
     ComponentTopology const& comp_topo_;
     ComponentConnections const& comp_conn_;
     // intermediate
     GlobalGraph global_graph_;
     DoubleVector phase_shift_;
     std::vector<GraphIdx> predecessors_;
@@ -239,16 +237,15 @@
             // begin to construct math topology
             MathModelTopology math_topo_single{};
             // reorder node number
             if (back_edges.empty()) {
                 // no cycle, the graph is pure tree structure
                 // just reverse the node
                 std::reverse(dfs_node.begin(), dfs_node.end());
-            }
-            else {
+            } else {
                 // with cycles, meshed graph
                 // use minimum degree
                 math_topo_single.fill_in = reorder_node(dfs_node, back_edges);
             }
             // initialize phase shift
             math_topo_single.phase_shift.resize((Idx)dfs_node.size());
             // i as bus number
@@ -289,22 +286,20 @@
                 // assign cycle status and go to predecessor
                 node_status_[node_in_cycle] = -2;
                 node_in_cycle = predecessors_[node_in_cycle];
             }
         }
 
         // copy all the far-end non-cyclic node, in reverse order
-        std::copy_if(dfs_node_copy.crbegin(), dfs_node_copy.crend(), std::back_inserter(dfs_node), [this](Idx x) {
-            return node_status_[x] == -1;
-        });
+        std::copy_if(dfs_node_copy.crbegin(), dfs_node_copy.crend(), std::back_inserter(dfs_node),
+                     [this](Idx x) { return node_status_[x] == -1; });
         // copy all cyclic node
         std::vector<Idx> cyclic_node;
-        std::copy_if(dfs_node_copy.cbegin(), dfs_node_copy.cend(), std::back_inserter(cyclic_node), [this](Idx x) {
-            return node_status_[x] == -2;
-        });
+        std::copy_if(dfs_node_copy.cbegin(), dfs_node_copy.cend(), std::back_inserter(cyclic_node),
+                     [this](Idx x) { return node_status_[x] == -2; });
         GraphIdx const n_cycle_node = cyclic_node.size();
         // reorder does not make sense if number of cyclic nodes in a sub graph is smaller than 4
         if (n_cycle_node < 4) {
             std::copy(cyclic_node.crbegin(), cyclic_node.crend(), std::back_inserter(dfs_node));
             return fill_in;
         }
 
@@ -483,55 +478,47 @@
                 idx_branch3.pos[n] = branch_pos;
             }
             // set branch idx in coupling
             comp_coup_.branch3[k] = idx_branch3;
         }
     }
 
-    static constexpr auto include_all = [](Idx) {
-        return true;
-    };
+    static constexpr auto include_all = [](Idx) { return true; };
 
     // proxy class to find the coupled object in math model in the coupling process to a single type object
     //    given a particular component index
     struct SingleTypeObjectFinder {
-        Idx size() const {
-            return (Idx)component_obj_idx.size();
-        }
-        Idx2D find_math_object(Idx component_i) const {
-            return objects_coupling[component_obj_idx[component_i]];
-        }
+        Idx size() const { return (Idx)component_obj_idx.size(); }
+        Idx2D find_math_object(Idx component_i) const { return objects_coupling[component_obj_idx[component_i]]; }
         IdxVector const& component_obj_idx;
         std::vector<Idx2D> const& objects_coupling;
     };
 
     // proxy class to find coupled branch in math model for sensor measured at from side, or at 1/2/3 side of branch3
     // they are all coupled to the from-side of some branches in math model
     // the key is to find relevant coupling, either via branch or branch3
     struct SensorBranchObjectFinder {
-        Idx size() const {
-            return (Idx)sensor_obj_idx.size();
-        }
+        Idx size() const { return (Idx)sensor_obj_idx.size(); }
         Idx2D find_math_object(Idx component_i) const {
             Idx const obj_idx = sensor_obj_idx[component_i];
             switch (power_sensor_terminal_type[component_i]) {
                 using enum MeasuredTerminalType;
 
-                case branch_from:
-                    return branch_coupling[obj_idx];
-                // return relevant branch mapped from branch3
-                case branch3_1:
-                    return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[0]};
-                case branch3_2:
-                    return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[1]};
-                case branch3_3:
-                    return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[2]};
-                default:
-                    assert(false);
-                    return {};
+            case branch_from:
+                return branch_coupling[obj_idx];
+            // return relevant branch mapped from branch3
+            case branch3_1:
+                return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[0]};
+            case branch3_2:
+                return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[1]};
+            case branch3_3:
+                return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[2]};
+            default:
+                assert(false);
+                return {};
             }
         }
         IdxVector const& sensor_obj_idx;
         std::vector<MeasuredTerminalType> const& power_sensor_terminal_type;
         std::vector<Idx2D> const& branch_coupling;
         std::vector<Idx2DBranch3> const& branch3_coupling;
     };
@@ -552,15 +539,15 @@
         // Collect objects and components per topology
         for (Idx component_i = 0; component_i != n_components; ++component_i) {
             if (!include(component_i)) {
                 continue;
             }
             Idx2D const math_idx = object_finder.find_math_object(component_i);
             Idx const topo_idx = math_idx.group;
-            if (topo_idx >= 0) {  // Consider non-isolated objects only
+            if (topo_idx >= 0) { // Consider non-isolated objects only
                 topo_obj_idx[topo_idx].push_back(math_idx.pos);
                 topo_component_idx[topo_idx].push_back(component_i);
             }
         }
 
         // Couple components per topology
         for (Idx topo_idx = 0; topo_idx != n_math_topologies; ++topo_idx) {
@@ -592,49 +579,45 @@
 
         // load gen
         couple_object_components<&MathModelTopology::load_gen_bus_indptr, &MathModelTopology::n_bus>(
             {comp_topo_.load_gen_node_idx, comp_coup_.node}, comp_coup_.load_gen);
 
         // set load gen type
         // resize vector
-        std::for_each(math_topology_.begin(), math_topology_.end(), [](MathModelTopology& topo) {
-            topo.load_gen_type.resize(topo.n_load_gen());
-        });
+        std::for_each(math_topology_.begin(), math_topology_.end(),
+                      [](MathModelTopology& topo) { topo.load_gen_type.resize(topo.n_load_gen()); });
         // assign load type
         for (Idx k = 0; k != (Idx)comp_topo_.load_gen_node_idx.size(); ++k) {
             Idx2D const idx_math = comp_coup_.load_gen[k];
             if (idx_math.group == -1) {
                 continue;
             }
             math_topology_[idx_math.group].load_gen_type[idx_math.pos] = comp_topo_.load_gen_type[k];
         }
 
         // source
         couple_object_components<&MathModelTopology::source_bus_indptr, &MathModelTopology::n_bus>(
-            {comp_topo_.source_node_idx, comp_coup_.node}, comp_coup_.source, [this](Idx i) {
-                return comp_conn_.source_connected[i];
-            });
+            {comp_topo_.source_node_idx, comp_coup_.node}, comp_coup_.source,
+            [this](Idx i) { return comp_conn_.source_connected[i]; });
     }
 
     void couple_sensors() {
         // voltage sensors
         couple_object_components<&MathModelTopology::voltage_sensor_indptr, &MathModelTopology::n_bus>(
             {comp_topo_.voltage_sensor_node_idx, comp_coup_.node}, comp_coup_.voltage_sensor);
 
         // source power sensors
         couple_object_components<&MathModelTopology::source_power_sensor_indptr, &MathModelTopology::n_source>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.source}, comp_coup_.power_sensor, [this](Idx i) {
-                return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::source;
-            });
+            {comp_topo_.power_sensor_object_idx, comp_coup_.source}, comp_coup_.power_sensor,
+            [this](Idx i) { return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::source; });
 
         // shunt power sensors
         couple_object_components<&MathModelTopology::shunt_power_sensor_indptr, &MathModelTopology::n_shunt>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.shunt}, comp_coup_.power_sensor, [this](Idx i) {
-                return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
-            });
+            {comp_topo_.power_sensor_object_idx, comp_coup_.shunt}, comp_coup_.power_sensor,
+            [this](Idx i) { return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::shunt; });
 
         // load + generator power sensors
         couple_object_components<&MathModelTopology::load_gen_power_sensor_indptr, &MathModelTopology::n_load_gen>(
             {comp_topo_.power_sensor_object_idx, comp_coup_.load_gen}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
                        comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
@@ -654,22 +637,20 @@
                                                                  comp_topo_.power_sensor_terminal_type,
                                                                  comp_coup_.branch, comp_coup_.branch3};
         couple_object_components<&MathModelTopology::branch_from_power_sensor_indptr, &MathModelTopology::n_branch>(
             object_finder_from_sensor, comp_coup_.power_sensor, predicate_from_sensor);
 
         // branch 'to' power sensors
         couple_object_components<&MathModelTopology::branch_to_power_sensor_indptr, &MathModelTopology::n_branch>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.branch}, comp_coup_.power_sensor, [this](Idx i) {
-                return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
-            });
+            {comp_topo_.power_sensor_object_idx, comp_coup_.branch}, comp_coup_.power_sensor,
+            [this](Idx i) { return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to; });
 
         // node injection power sensors
         couple_object_components<&MathModelTopology::bus_power_sensor_indptr, &MathModelTopology::n_bus>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.node}, comp_coup_.power_sensor, [this](Idx i) {
-                return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::node;
-            });
+            {comp_topo_.power_sensor_object_idx, comp_coup_.node}, comp_coup_.power_sensor,
+            [this](Idx i) { return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::node; });
     }
 };
 
-}  // namespace power_grid_model
+} // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 #else
 #define PGM_HELPER_DLL_IMPORT
 #define PGM_HELPER_DLL_EXPORT
 #define PGM_HELPER_DLL_LOCAL
 #endif
 #endif
 // Now we use the generic helper definitions above to define PGM_API and PGM_LOCAL.
-#ifdef PGM_DLL_EXPORTS  // defined if we are building the POWER_GRID_MODEL DLL (instead of using it)
+#ifdef PGM_DLL_EXPORTS // defined if we are building the POWER_GRID_MODEL DLL (instead of using it)
 #define PGM_API PGM_HELPER_DLL_EXPORT
 #else
 #define PGM_API PGM_HELPER_DLL_IMPORT
-#endif  // PGM_DLL_EXPORTS
+#endif // PGM_DLL_EXPORTS
 #define PGM_LOCAL PGM_HELPER_DLL_LOCAL
 // API_MACRO_BLOCK
 
 // integers
 #ifdef __cplusplus
 #include <cstddef>
 #include <cstdint>
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 #include "power_grid_model_c/basics.h"
 #include "power_grid_model_c/buffer.h"
 #include "power_grid_model_c/handle.h"
 #include "power_grid_model_c/meta_data.h"
 #include "power_grid_model_c/model.h"
 #include "power_grid_model_c/options.h"
 
-#endif  // POWER_GRID_MODEL_C_H
+#endif // POWER_GRID_MODEL_C_H
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #include <cstdlib>
 
 namespace {
 using namespace power_grid_model;
 
 using meta_data::RawDataConstPtr;
 using meta_data::RawDataPtr;
-}  // namespace
+} // namespace
 
 // buffer control
 RawDataPtr PGM_create_buffer(PGM_Handle*, PGM_MetaComponent const* component, PGM_Idx size) {
 #ifdef _WIN32
     return _aligned_malloc(component->size * size, component->alignment);
 #else
     return std::aligned_alloc(component->alignment, component->size * size);
@@ -46,21 +46,20 @@
         stride = static_cast<PGM_Idx>(attribute->size);
     }
     for (Idx i = buffer_offset; i != size + buffer_offset; ++i) {
         ValuePtr const shifted_value_ptr =
             reinterpret_cast<std::conditional_t<is_get, char*, char const*>>(value_ptr) + stride * i;
         if constexpr (is_get) {
             attribute->get_value(buffer_ptr, shifted_value_ptr, i);
-        }
-        else {
+        } else {
             attribute->set_value(buffer_ptr, shifted_value_ptr, i);
         }
     }
 }
-}  // namespace
+} // namespace
 void PGM_buffer_set_value(PGM_Handle*, PGM_MetaAttribute const* attribute, RawDataPtr buffer_ptr,
                           RawDataConstPtr src_ptr, PGM_Idx buffer_offset, PGM_Idx size, PGM_Idx src_stride) {
     buffer_get_set_value<false>(attribute, buffer_ptr, src_ptr, buffer_offset, size, src_stride);
 }
 void PGM_buffer_get_value(PGM_Handle*, PGM_MetaAttribute const* attribute, RawDataConstPtr buffer_ptr,
                           RawDataPtr dest_ptr, PGM_Idx buffer_offset, PGM_Idx size, PGM_Idx dest_stride) {
     buffer_get_set_value<true>(attribute, buffer_ptr, dest_ptr, buffer_offset, size, dest_stride);
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -5,41 +5,25 @@
 #define PGM_DLL_EXPORTS
 #include "power_grid_model_c/handle.h"
 
 #include "handle.hpp"
 
 namespace {
 using namespace power_grid_model;
-}  // namespace
+} // namespace
 
 // create and destroy handle
-PGM_Handle* PGM_create_handle() {
-    return new PGM_Handle{};
-}
-void PGM_destroy_handle(PGM_Handle* handle) {
-    delete handle;
-}
+PGM_Handle* PGM_create_handle() { return new PGM_Handle{}; }
+void PGM_destroy_handle(PGM_Handle* handle) { delete handle; }
 
 // error handling
-PGM_Idx PGM_error_code(PGM_Handle const* handle) {
-    return handle->err_code;
-}
-char const* PGM_error_message(PGM_Handle const* handle) {
-    return handle->err_msg.c_str();
-}
-PGM_Idx PGM_n_failed_scenarios(PGM_Handle const* handle) {
-    return static_cast<Idx>(handle->failed_scenarios.size());
-}
-PGM_Idx const* PGM_failed_scenarios(PGM_Handle const* handle) {
-    return handle->failed_scenarios.data();
-}
+PGM_Idx PGM_error_code(PGM_Handle const* handle) { return handle->err_code; }
+char const* PGM_error_message(PGM_Handle const* handle) { return handle->err_msg.c_str(); }
+PGM_Idx PGM_n_failed_scenarios(PGM_Handle const* handle) { return static_cast<Idx>(handle->failed_scenarios.size()); }
+PGM_Idx const* PGM_failed_scenarios(PGM_Handle const* handle) { return handle->failed_scenarios.data(); }
 char const** PGM_batch_errors(PGM_Handle const* handle) {
     handle->batch_errs_c_str.clear();
     std::transform(handle->batch_errs.begin(), handle->batch_errs.end(), std::back_inserter(handle->batch_errs_c_str),
-                   [](auto const& x) {
-                       return x.c_str();
-                   });
+                   [](auto const& x) { return x.c_str(); });
     return handle->batch_errs_c_str.data();
 }
-void PGM_clear_error(PGM_Handle* handle) {
-    *handle = PGM_Handle{};
-}
+void PGM_clear_error(PGM_Handle* handle) { *handle = PGM_Handle{}; }
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -12,92 +12,63 @@
 namespace {
 using namespace power_grid_model;
 
 // assert index type
 static_assert(std::is_same_v<PGM_Idx, Idx>);
 static_assert(std::is_same_v<PGM_ID, ID>);
 
-template <class Functor>
-auto call_with_bound(PGM_Handle* handle, Functor func) -> std::invoke_result_t<Functor> {
+template <class Functor> auto call_with_bound(PGM_Handle* handle, Functor func) -> std::invoke_result_t<Functor> {
     static std::remove_cv_t<std::remove_reference_t<std::invoke_result_t<Functor>>> const empty{};
     try {
         return func();
-    }
-    catch (std::out_of_range& e) {
+    } catch (std::out_of_range& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = std::string(e.what()) + "\n You supplied wrong name and/or index!\n";
         return empty;
     }
 }
-}  // namespace
+} // namespace
 
 // retrieve meta data
 // dataset
-PGM_Idx PGM_meta_n_datasets(PGM_Handle*) {
-    return meta_data::meta_data().n_datasets();
-}
+PGM_Idx PGM_meta_n_datasets(PGM_Handle*) { return meta_data::meta_data().n_datasets(); }
 PGM_MetaDataset const* PGM_meta_get_dataset_by_idx(PGM_Handle* handle, PGM_Idx idx) {
-    return call_with_bound(handle, [idx]() -> decltype(auto) {
-        return &meta_data::meta_data().datasets.at(idx);
-    });
+    return call_with_bound(handle, [idx]() -> decltype(auto) { return &meta_data::meta_data().datasets.at(idx); });
 }
 PGM_MetaDataset const* PGM_meta_get_dataset_by_name(PGM_Handle* handle, char const* dataset) {
-    return call_with_bound(handle, [dataset]() -> decltype(auto) {
-        return &meta_data::meta_data().get_dataset(dataset);
-    });
-}
-char const* PGM_meta_dataset_name(PGM_Handle*, PGM_MetaDataset const* dataset) {
-    return dataset->name.c_str();
+    return call_with_bound(handle,
+                           [dataset]() -> decltype(auto) { return &meta_data::meta_data().get_dataset(dataset); });
 }
+char const* PGM_meta_dataset_name(PGM_Handle*, PGM_MetaDataset const* dataset) { return dataset->name.c_str(); }
 // component
-PGM_Idx PGM_meta_n_components(PGM_Handle*, PGM_MetaDataset const* dataset) {
-    return dataset->n_components();
-}
+PGM_Idx PGM_meta_n_components(PGM_Handle*, PGM_MetaDataset const* dataset) { return dataset->n_components(); }
 PGM_MetaComponent const* PGM_meta_get_component_by_idx(PGM_Handle* handle, PGM_MetaDataset const* dataset,
                                                        PGM_Idx idx) {
-    return call_with_bound(handle, [idx, dataset]() -> decltype(auto) {
-        return &dataset->components.at(idx);
-    });
+    return call_with_bound(handle, [idx, dataset]() -> decltype(auto) { return &dataset->components.at(idx); });
 }
 PGM_MetaComponent const* PGM_meta_get_component_by_name(PGM_Handle* handle, char const* dataset,
                                                         char const* component) {
     return call_with_bound(handle, [component, dataset]() -> decltype(auto) {
         return &meta_data::meta_data().get_dataset(dataset).get_component(component);
     });
 }
-char const* PGM_meta_component_name(PGM_Handle*, PGM_MetaComponent const* component) {
-    return component->name.c_str();
-}
-size_t PGM_meta_component_size(PGM_Handle*, PGM_MetaComponent const* component) {
-    return component->size;
-}
-size_t PGM_meta_component_alignment(PGM_Handle*, PGM_MetaComponent const* component) {
-    return component->alignment;
-}
+char const* PGM_meta_component_name(PGM_Handle*, PGM_MetaComponent const* component) { return component->name.c_str(); }
+size_t PGM_meta_component_size(PGM_Handle*, PGM_MetaComponent const* component) { return component->size; }
+size_t PGM_meta_component_alignment(PGM_Handle*, PGM_MetaComponent const* component) { return component->alignment; }
 // attributes
-PGM_Idx PGM_meta_n_attributes(PGM_Handle*, PGM_MetaComponent const* component) {
-    return component->n_attributes();
-}
+PGM_Idx PGM_meta_n_attributes(PGM_Handle*, PGM_MetaComponent const* component) { return component->n_attributes(); }
 PGM_MetaAttribute const* PGM_meta_get_attribute_by_idx(PGM_Handle* handle, PGM_MetaComponent const* component,
                                                        PGM_Idx idx) {
-    return call_with_bound(handle, [idx, component]() -> decltype(auto) {
-        return &component->attributes.at(idx);
-    });
+    return call_with_bound(handle, [idx, component]() -> decltype(auto) { return &component->attributes.at(idx); });
 }
 PGM_MetaAttribute const* PGM_meta_get_attribute_by_name(PGM_Handle* handle, char const* dataset, char const* component,
                                                         char const* attribute) {
     return call_with_bound(handle, [component, dataset, attribute]() -> decltype(auto) {
         return &meta_data::meta_data().get_dataset(dataset).get_component(component).get_attribute(attribute);
     });
 }
-char const* PGM_meta_attribute_name(PGM_Handle*, PGM_MetaAttribute const* attribute) {
-    return attribute->name.c_str();
-}
+char const* PGM_meta_attribute_name(PGM_Handle*, PGM_MetaAttribute const* attribute) { return attribute->name.c_str(); }
 PGM_Idx PGM_meta_attribute_ctype(PGM_Handle*, PGM_MetaAttribute const* attribute) {
     return static_cast<PGM_Idx>(attribute->ctype);
 }
-size_t PGM_meta_attribute_offset(PGM_Handle*, PGM_MetaAttribute const* attribute) {
-    return attribute->offset;
-}
-int PGM_is_little_endian(PGM_Handle*) {
-    return meta_data::is_little_endian();
-}
+size_t PGM_meta_attribute_offset(PGM_Handle*, PGM_MetaAttribute const* attribute) { return attribute->offset; }
+int PGM_is_little_endian(PGM_Handle*) { return meta_data::is_little_endian(); }
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #include <power_grid_model/power_grid_model.hpp>
 
 namespace {
 using namespace power_grid_model;
 
 using meta_data::RawDataConstPtr;
 using meta_data::RawDataPtr;
-}  // namespace
+} // namespace
 
 // aliases main class
 struct PGM_PowerGridModel : public MainModel {
     using MainModel::MainModel;
 };
 
 // create model
@@ -31,16 +31,15 @@
     PGM_clear_error(handle);
     ConstDataset dataset{};
     for (Idx i = 0; i != n_components; ++i) {
         dataset[components[i]] = ConstDataPointer{input_data[i], component_sizes[i]};
     }
     try {
         return new PGM_PowerGridModel{system_frequency, dataset, 0};
-    }
-    catch (std::exception& e) {
+    } catch (std::exception& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
         return nullptr;
     }
 }
 
 // update model
@@ -49,40 +48,37 @@
     PGM_clear_error(handle);
     ConstDataset dataset{};
     for (Idx i = 0; i != n_components; ++i) {
         dataset[components[i]] = ConstDataPointer{update_data[i], component_sizes[i]};
     }
     try {
         model->update_component<MainModel::permanent_update_t>(dataset);
-    }
-    catch (std::exception& e) {
+    } catch (std::exception& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
     }
 }
 
 // copy model
 PGM_PowerGridModel* PGM_copy_model(PGM_Handle* handle, PGM_PowerGridModel const* model) {
     try {
         return new PGM_PowerGridModel{*model};
-    }
-    catch (std::exception& e) {
+    } catch (std::exception& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
         return nullptr;
     }
 }
 
 // get indexer
 void PGM_get_indexer(PGM_Handle* handle, PGM_PowerGridModel const* model, char const* component, PGM_Idx size,
                      PGM_ID const* ids, PGM_Idx* indexer) {
     try {
         model->get_indexer(component, ids, size, indexer);
-    }
-    catch (std::exception& e) {
+    } catch (std::exception& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
     }
 }
 
 // run calculation
 void PGM_calculate(PGM_Handle* handle, PGM_PowerGridModel* model, PGM_Options const* opt, PGM_Idx n_output_components,
@@ -106,72 +102,60 @@
     // prepare update dataset
     ConstDataset update_dataset{};
     for (Idx i = 0; i != n_update_components; ++i) {
         if (n_component_elements_per_scenario[i] < 0) {
             // use indptr as sparse batch
             update_dataset[update_components[i]] =
                 ConstDataPointer(update_data[i], indptrs_per_component[i], n_scenarios);
-        }
-        else {
+        } else {
             // use dense batch
             update_dataset[update_components[i]] =
                 ConstDataPointer(update_data[i], n_scenarios, n_component_elements_per_scenario[i]);
         }
     }
     // call calculation
     try {
         auto const calculation_method = static_cast<CalculationMethod>(opt->calculation_method);
         switch (opt->calculation_type) {
-            case PGM_power_flow:
-                if (opt->symmetric) {
-                    handle->batch_parameter =
-                        model->calculate_power_flow<true>(opt->err_tol, opt->max_iter, calculation_method,
-                                                          output_dataset, update_dataset, opt->threading);
-                }
-                else {
-                    handle->batch_parameter =
-                        model->calculate_power_flow<false>(opt->err_tol, opt->max_iter, calculation_method,
-                                                           output_dataset, update_dataset, opt->threading);
-                }
-                break;
-            case PGM_state_estimation:
-                if (opt->symmetric) {
-                    handle->batch_parameter =
-                        model->calculate_state_estimation<true>(opt->err_tol, opt->max_iter, calculation_method,
-                                                                output_dataset, update_dataset, opt->threading);
-                }
-                else {
-                    handle->batch_parameter =
-                        model->calculate_state_estimation<false>(opt->err_tol, opt->max_iter, calculation_method,
-                                                                 output_dataset, update_dataset, opt->threading);
-                }
-                break;
-            case PGM_short_circuit: {
-                constexpr double voltage_scaling_factor_c{1.1};
-                handle->batch_parameter = model->calculate_short_circuit(
-                    voltage_scaling_factor_c, calculation_method, output_dataset, update_dataset, opt->threading);
-                break;
+        case PGM_power_flow:
+            if (opt->symmetric) {
+                handle->batch_parameter = model->calculate_power_flow<true>(
+                    opt->err_tol, opt->max_iter, calculation_method, output_dataset, update_dataset, opt->threading);
+            } else {
+                handle->batch_parameter = model->calculate_power_flow<false>(
+                    opt->err_tol, opt->max_iter, calculation_method, output_dataset, update_dataset, opt->threading);
+            }
+            break;
+        case PGM_state_estimation:
+            if (opt->symmetric) {
+                handle->batch_parameter = model->calculate_state_estimation<true>(
+                    opt->err_tol, opt->max_iter, calculation_method, output_dataset, update_dataset, opt->threading);
+            } else {
+                handle->batch_parameter = model->calculate_state_estimation<false>(
+                    opt->err_tol, opt->max_iter, calculation_method, output_dataset, update_dataset, opt->threading);
             }
-            default:
-                throw MissingCaseForEnumError{"CalculationType", opt->calculation_type};
+            break;
+        case PGM_short_circuit: {
+            constexpr double voltage_scaling_factor_c{1.1};
+            handle->batch_parameter = model->calculate_short_circuit(voltage_scaling_factor_c, calculation_method,
+                                                                     output_dataset, update_dataset, opt->threading);
+            break;
         }
-    }
-    catch (BatchCalculationError& e) {
+        default:
+            throw MissingCaseForEnumError{"CalculationType", opt->calculation_type};
+        }
+    } catch (BatchCalculationError& e) {
         handle->err_code = PGM_batch_error;
         handle->err_msg = e.what();
         handle->failed_scenarios = e.failed_scenarios();
         handle->batch_errs = e.err_msgs();
-    }
-    catch (std::exception& e) {
+    } catch (std::exception& e) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
-    }
-    catch (...) {
+    } catch (...) {
         handle->err_code = PGM_regular_error;
         handle->err_msg = "Unknown error!\n";
     }
 }
 
 // destroy model
-void PGM_destroy_model(PGM_PowerGridModel* model) {
-    delete model;
-}
+void PGM_destroy_model(PGM_PowerGridModel* model) { delete model; }
```

### Comparing `power-grid-model-1.5.1/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.2/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/pyproject.toml` & `power-grid-model-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/setup.py` & `power-grid-model-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/__init__.py` & `power-grid-model-1.5.2/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.2/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.2/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/options.py` & `power-grid-model-1.5.2/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.2/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.2/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.2/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/data_types.py` & `power-grid-model-1.5.2/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/enum.py` & `power-grid-model-1.5.2/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/utils.py` & `power-grid-model-1.5.2/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.2/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.2/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.1/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.2/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.2/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.2/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.2/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.2/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.2/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.2/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.2/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.2/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.2/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/test_error_handling.py` & `power-grid-model-1.5.2/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/test_meta_data.py` & `power-grid-model-1.5.2/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.2/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/test_utils.py` & `power-grid-model-1.5.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/utils.py` & `power-grid-model-1.5.2/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.2/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.2/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.2/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.2/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.2/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.2/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.1/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.2/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

