# Comparing `tmp/jaxsim-0.1.dev191.tar.gz` & `tmp/jaxsim-0.1.dev196.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev191.tar", last modified: Fri Jun 30 21:04:34 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev196.tar", last modified: Fri Aug  4 08:33:16 2023, max compression
```

## Comparing `jaxsim-0.1.dev191.tar` & `jaxsim-0.1.dev196.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.739724 jaxsim-0.1.dev191/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:04:34.759724 jaxsim-0.1.dev191/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.739724 jaxsim-0.1.dev191/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    45600 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.747724 jaxsim-0.1.dev191/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/parsers/rod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.751724 jaxsim-0.1.dev191/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.743724 jaxsim-0.1.dev191/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 21:04:34.000000 jaxsim-0.1.dev191/src/jaxsim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:34.755724 jaxsim-0.1.dev191/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/test_eom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/test_forward_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_idyntree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 21:04:16.000000 jaxsim-0.1.dev191/tests/utils_rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.588308 jaxsim-0.1.dev196/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.588308 jaxsim-0.1.dev196/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 08:33:16.600308 jaxsim-0.1.dev196/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.588308 jaxsim-0.1.dev196/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.588308 jaxsim-0.1.dev196/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45663 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/parsers/rod/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/rod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/rod/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/parsers/rod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16009 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.592308 jaxsim-0.1.dev196/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 08:33:16.000000 jaxsim-0.1.dev196/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:16.596308 jaxsim-0.1.dev196/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/test_eom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/test_forward_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/utils_idyntree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-04 08:33:01.000000 jaxsim-0.1.dev196/tests/utils_rng.py
```

### Comparing `jaxsim-0.1.dev191/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev196/.github/workflows/ci_cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: "3.10"
 
       - name: Install Python tools
         run: pip install build twine
 
       - name: Create distributions
         run: python -m build -o dist/
 
@@ -54,16 +54,14 @@
       matrix:
         os:
           - ubuntu-22.04
           - macos-latest
           # https://github.com/google/jax/issues/5795
           # - windows-latest
         python:
-          - "3.8"
-          - "3.9"
           - "3.10"
           - "3.11"
 
     steps:
 
       - name: Set up Python
         uses: actions/setup-python@v4
```

### Comparing `jaxsim-0.1.dev191/.github/workflows/style.yml` & `jaxsim-0.1.dev196/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/.gitignore` & `jaxsim-0.1.dev196/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/LICENSE` & `jaxsim-0.1.dev196/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/PKG-INFO` & `jaxsim-0.1.dev196/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev191
+Version: 0.1.dev196
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -15,25 +15,23 @@
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 # JAXsim
```

### Comparing `jaxsim-0.1.dev191/README.md` & `jaxsim-0.1.dev196/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/setup.cfg` & `jaxsim-0.1.dev196/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -29,31 +29,29 @@
 	Framework :: Robot Framework
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Games/Entertainment :: Simulation
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Software Development
 
 [options]
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
-python_requires = >=3.8
+python_requires = >=3.10
 install_requires = 
 	coloredlogs
 	jax >= 0.4.1
 	jaxlib
 	jaxlie
 	jax_dataclasses >= 1.4.0
 	pptree
```

### Comparing `jaxsim-0.1.dev191/src/jaxsim/__init__.py` & `jaxsim-0.1.dev196/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev196/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev196/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev196/src/jaxsim/high_level/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pathlib
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
+import rod
 from jax_dataclasses import Static
 
 import jaxsim.physics.algos.aba
 import jaxsim.physics.algos.crba
 import jaxsim.physics.algos.forward_kinematics
 import jaxsim.physics.algos.rnea
 import jaxsim.physics.model.physics_model
@@ -121,26 +122,27 @@
 
     # ========================
     # Initialization and state
     # ========================
 
     @staticmethod
     def build_from_model_description(
-        model_description: Union[str, pathlib.Path],
+        model_description: Union[str, pathlib.Path, rod.Model],
         model_name: Optional[str] = None,
         vel_repr: VelRepr = VelRepr.Mixed,
         gravity: jtp.Array = jaxsim.physics.default_gravity(),
         is_urdf: Optional[bool] = None,
         considered_joints: Optional[List[str]] = None,
     ) -> "Model":
         """
         Build a Model object from a model description.
 
         Args:
-            model_description: Either a path to a file or a string containing the URDF/SDF description.
+            model_description: A path to an SDF/URDF file, a string containing its content,
+                or a pre-parsed/pre-built rod model.
             model_name: The optional name of the model that overrides the one in the description.
             vel_repr: The velocity representation to use.
             gravity: The 3D gravity vector.
             is_urdf: Whether the model description is a URDF or an SDF. This is
                 automatically inferred if the model description is a path to a file.
             considered_joints: The list of joints to consider. If None, all joints are considered.
```

### Comparing `jaxsim-0.1.dev191/src/jaxsim/logging.py` & `jaxsim-0.1.dev196/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev196/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev196/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev196/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev196/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev196/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev196/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev196/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev196/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev196/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/rod/parser.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/rod/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,42 +28,46 @@
     collision_shapes: List[descriptions.CollisionShape]
 
     sdf_model: Optional[rod.Model] = None
     model_pose: kinematic_graph.RootPose = kinematic_graph.RootPose()
 
 
 def extract_model_data(
-    model_description: Union[pathlib.Path, str],
+    model_description: Union[pathlib.Path, str, rod.Model],
     model_name: Optional[str] = None,
     is_urdf: Optional[bool] = None,
 ) -> SDFData:
     """
     Extract data from an SDF/URDF resource useful to build a JaxSim model.
 
     Args:
-        model_description: Either a path to an SDF/URDF file or a string containing its content.
+        model_description: A path to an SDF/URDF file, a string containing its content,
+          or a pre-parsed/pre-built rod model.
         model_name: The name of the model to extract from the SDF resource.
         is_urdf: Whether the SDF resource is a URDF file. Needed only if model_description
             is a URDF string.
 
     Returns:
         The extracted model data.
     """
 
-    # Parse the SDF resource
-    sdf_element = rod.Sdf.load(sdf=model_description, is_urdf=is_urdf)
+    if isinstance(model_description, rod.Model):
+        sdf_model = model_description
+    else:
+        # Parse the SDF resource
+        sdf_element = rod.Sdf.load(sdf=model_description, is_urdf=is_urdf)
 
-    if len(sdf_element.models()) == 0:
-        raise RuntimeError("Failed to find any model in SDF resource")
+        if len(sdf_element.models()) == 0:
+            raise RuntimeError("Failed to find any model in SDF resource")
 
-    # Assume the SDF resource has only one model, or the desired model name is given
-    sdf_models = {m.name: m for m in sdf_element.models()}
-    sdf_model = (
-        sdf_element.models()[0] if len(sdf_models) == 1 else sdf_models[model_name]
-    )
+        # Assume the SDF resource has only one model, or the desired model name is given
+        sdf_models = {m.name: m for m in sdf_element.models()}
+        sdf_model = (
+            sdf_element.models()[0] if len(sdf_models) == 1 else sdf_models[model_name]
+        )
 
     # Log model name
     logging.debug(msg=f"Found model '{sdf_model.name}' in SDF resource")
 
     # Jaxsim supports only models compatible with URDF, i.e. those having all links
     # directly attached to their parent joint without additional roto-translations.
     sdf_model.switch_frame_convention(frame_convention=rod.FrameConvention.Urdf)
@@ -294,21 +298,23 @@
         base_link_name=sdf_model.get_canonical_link(),
         model_pose=model_pose,
         sdf_model=sdf_model,
     )
 
 
 def build_model_description(
-    model_description: Union[pathlib.Path, str], is_urdf: Optional[bool] = False
+    model_description: Union[pathlib.Path, str, rod.Model],
+    is_urdf: Optional[bool] = False,
 ) -> descriptions.ModelDescription:
     """
     Builds a model description from an SDF/URDF resource.
 
     Args:
-        model_description: Either a path to an SDF/URDF file or a string containing its content.
+        model_description: A path to an SDF/URDF file, a string containing its content,
+          or a pre-parsed/pre-built rod model.
         is_urdf: Whether the SDF resource is a URDF file. Needed only if model_description
             is a URDF string.
     Returns:
         The parsed model description.
     """
 
     # Parse data from the SDF assuming it contains a single model
```

### Comparing `jaxsim-0.1.dev191/src/jaxsim/parsers/rod/utils.py` & `jaxsim-0.1.dev196/src/jaxsim/parsers/rod/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev196/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/ode.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import functools
 import pathlib
 from typing import Dict, List, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import jax_dataclasses
+import rod
 from jax_dataclasses import Static
 
 import jaxsim.high_level
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.physics
 import jaxsim.simulation.simulator_callbacks as scb
 import jaxsim.typing as jtp
@@ -222,23 +223,24 @@
         for model_name, model in self.data.models.items():
             model.physics_model.set_gravity(gravity=gravity)
 
         self._set_mutability(self._mutability())
 
     def insert_model_from_description(
         self,
-        model_description: Union[pathlib.Path, str],
+        model_description: Union[pathlib.Path, str, rod.Model],
         model_name: Optional[str] = None,
         considered_joints: Optional[List[str]] = None,
     ) -> Model:
         """
         Insert a model from a model description.
 
         Args:
-            model_description: Either a path to a file or a string containing the URDF/SDF description.
+            model_description: A path to an SDF/URDF file, a string containing its content,
+                or a pre-parsed/pre-built rod model.
             model_name: The optional name of the model that overrides the one in the description.
             considered_joints: Optional list of joints to consider.
                                It is also useful to specify the joint serialization.
 
         Returns:
             The newly inserted model.
         """
```

### Comparing `jaxsim-0.1.dev191/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev196/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/typing.py` & `jaxsim-0.1.dev196/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim/utils.py` & `jaxsim-0.1.dev196/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev196/src/jaxsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev191
+Version: 0.1.dev196
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -15,25 +15,23 @@
 Classifier: Framework :: Robot Framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 # JAXsim
```

### Comparing `jaxsim-0.1.dev191/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev196/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/tests/test_eom.py` & `jaxsim-0.1.dev196/tests/test_eom.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/tests/test_forward_dynamics.py` & `jaxsim-0.1.dev196/tests/test_forward_dynamics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/tests/utils_idyntree.py` & `jaxsim-0.1.dev196/tests/utils_idyntree.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/tests/utils_models.py` & `jaxsim-0.1.dev196/tests/utils_models.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev191/tests/utils_rng.py` & `jaxsim-0.1.dev196/tests/utils_rng.py`

 * *Files identical despite different names*

