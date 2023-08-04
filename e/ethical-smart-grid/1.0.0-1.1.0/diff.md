# Comparing `tmp/ethical_smart_grid-1.0.0.tar.gz` & `tmp/ethical_smart_grid-1.1.0.tar.gz`

## Comparing `ethical_smart_grid-1.0.0.tar` & `ethical_smart_grid-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/requirements.txt
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/__init__.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/model.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/naive/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/naive/random_model.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/qsom/__init__.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/qsom/qsom.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/qsom/qsom_agent.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/qsom/som.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/util/__init__.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/util/action_perturbator.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/algorithms/util/action_selector.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/Readme.md
--rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_office_annually.npz
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_office_daily.npz
--rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_residential_annually.npz
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_residential_daily.npz
--rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_school_annually.npz
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/data/openei/profile_school_daily.npz
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/__init__.py
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/environment.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/make_env.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/world.py
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/__init__.py
--rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/agent.py
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/data_conversion.py
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/profile/__init__.py
--rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/profile/agent_profile.py
--rwxr-xr-x   0        0        0     6772 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/profile/comfort.py
--rwxr-xr-x   0        0        0     3364 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/profile/need.py
--rwxr-xr-x   0        0        0     3306 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/agents/profile/production.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/observation/__init__.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/observation/global_observation.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/observation/local_observation.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/observation/observation_manager.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/observation/observations.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/__init__.py
--rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/reward.py
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/reward_collection.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/__init__.py
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/adaptability.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/equity.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/multi_objective_product.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/multi_objective_sum.py
--rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/over_consumption.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/__init__.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/adaptability.py
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/comfort.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/equity.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/multi_objective_sum.py
--rwxr-xr-x   0        0        0      808 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/over_consumption.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/util/__init__.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/util/available_energy.py
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/util/bounded.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/util/equity.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/util/interpolate.py
--rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/wrappers/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/smartgrid/wrappers/reward_aggregator.py
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_action.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_bounded.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_energy_generator.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_interpolate.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_models.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/tests/test_world.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/.gitignore
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/Readme.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 ethical_smart_grid-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/codemeta.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/__init__.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/model.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/naive/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/naive/random_model.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/qsom/__init__.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/qsom/qsom.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/qsom/qsom_agent.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/qsom/som.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/util/__init__.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/util/action_perturbator.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/algorithms/util/action_selector.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/Readme.md
+-rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_office_annually.npz
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_office_daily.npz
+-rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_residential_annually.npz
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_residential_daily.npz
+-rw-r--r--   0        0        0    70870 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_school_annually.npz
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/data/openei/profile_school_daily.npz
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/__init__.py
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/environment.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/make_env.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/scenarii.py
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/world.py
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/__init__.py
+-rw-r--r--   0        0        0    10887 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/agent.py
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/data_conversion.py
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/profile/__init__.py
+-rw-r--r--   0        0        0    10394 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/profile/agent_profile.py
+-rwxr-xr-x   0        0        0     6772 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/profile/comfort.py
+-rwxr-xr-x   0        0        0     3364 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/profile/need.py
+-rwxr-xr-x   0        0        0     3306 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/agents/profile/production.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/observation/__init__.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/observation/global_observation.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/observation/local_observation.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/observation/observation_manager.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/observation/observations.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/__init__.py
+-rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/reward.py
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/reward_collection.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/__init__.py
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/adaptability.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/equity.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/multi_objective_product.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/multi_objective_sum.py
+-rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/over_consumption.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/__init__.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/adaptability.py
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/comfort.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/equity.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/multi_objective_sum.py
+-rwxr-xr-x   0        0        0      808 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/over_consumption.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/util/__init__.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/util/available_energy.py
+-rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/util/bounded.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/util/equity.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/util/interpolate.py
+-rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/wrappers/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/smartgrid/wrappers/reward_aggregator.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_action.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_bounded.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_energy_generator.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_interpolate.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_models.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/tests/test_world.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/Readme.md
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 ethical_smart_grid-1.1.0/PKG-INFO
```

### Comparing `ethical_smart_grid-1.0.0/algorithms/model.py` & `ethical_smart_grid-1.1.0/algorithms/model.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/naive/random_model.py` & `ethical_smart_grid-1.1.0/algorithms/naive/random_model.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/qsom/qsom.py` & `ethical_smart_grid-1.1.0/algorithms/qsom/qsom.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/qsom/qsom_agent.py` & `ethical_smart_grid-1.1.0/algorithms/qsom/qsom_agent.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/qsom/som.py` & `ethical_smart_grid-1.1.0/algorithms/qsom/som.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/util/__init__.py` & `ethical_smart_grid-1.1.0/algorithms/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/util/action_perturbator.py` & `ethical_smart_grid-1.1.0/algorithms/util/action_perturbator.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/algorithms/util/action_selector.py` & `ethical_smart_grid-1.1.0/algorithms/util/action_selector.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_office_annually.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_office_annually.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_office_daily.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_office_daily.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_residential_annually.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_residential_annually.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_residential_daily.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_residential_daily.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_school_annually.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_school_annually.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/data/openei/profile_school_daily.npz` & `ethical_smart_grid-1.1.0/data/openei/profile_school_daily.npz`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/environment.py` & `ethical_smart_grid-1.1.0/smartgrid/environment.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/make_env.py` & `ethical_smart_grid-1.1.0/smartgrid/make_env.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/world.py` & `ethical_smart_grid-1.1.0/smartgrid/world.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/__init__.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/agent.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/data_conversion.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/data_conversion.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/profile/agent_profile.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/profile/agent_profile.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/profile/comfort.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/profile/comfort.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/profile/need.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/profile/need.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/agents/profile/production.py` & `ethical_smart_grid-1.1.0/smartgrid/agents/profile/production.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/observation/__init__.py` & `ethical_smart_grid-1.1.0/smartgrid/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/observation/global_observation.py` & `ethical_smart_grid-1.1.0/smartgrid/observation/global_observation.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/observation/local_observation.py` & `ethical_smart_grid-1.1.0/smartgrid/observation/local_observation.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/observation/observation_manager.py` & `ethical_smart_grid-1.1.0/smartgrid/observation/observation_manager.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/observation/observations.py` & `ethical_smart_grid-1.1.0/smartgrid/observation/observations.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/__init__.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/reward.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/reward.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/reward_collection.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/reward_collection.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/__init__.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/__init__.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/adaptability.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/adaptability.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/equity.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/equity.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/multi_objective_product.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/multi_objective_product.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/multi_objective_sum.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/multi_objective_sum.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/differentiated/over_consumption.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/differentiated/over_consumption.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/adaptability.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/adaptability.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/comfort.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/comfort.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/equity.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/equity.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/multi_objective_sum.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/multi_objective_sum.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/rewards/numeric/per_agent/over_consumption.py` & `ethical_smart_grid-1.1.0/smartgrid/rewards/numeric/per_agent/over_consumption.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/util/available_energy.py` & `ethical_smart_grid-1.1.0/smartgrid/util/available_energy.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/util/bounded.py` & `ethical_smart_grid-1.1.0/smartgrid/util/bounded.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/util/equity.py` & `ethical_smart_grid-1.1.0/smartgrid/util/equity.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/util/interpolate.py` & `ethical_smart_grid-1.1.0/smartgrid/util/interpolate.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/smartgrid/wrappers/reward_aggregator.py` & `ethical_smart_grid-1.1.0/smartgrid/wrappers/reward_aggregator.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_action.py` & `ethical_smart_grid-1.1.0/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_bounded.py` & `ethical_smart_grid-1.1.0/tests/test_bounded.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_energy_generator.py` & `ethical_smart_grid-1.1.0/tests/test_energy_generator.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_interpolate.py` & `ethical_smart_grid-1.1.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_models.py` & `ethical_smart_grid-1.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/tests/test_world.py` & `ethical_smart_grid-1.1.0/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/LICENSE.md` & `ethical_smart_grid-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ethical_smart_grid-1.0.0/pyproject.toml` & `ethical_smart_grid-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ethical-smart-grid"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name = "Clément Scheirlinck", email = "clement.scheirlinck@etu.univ-lyon1.fr" },
 ]
 maintainers = [
     { name = "Rémy Chaput", email = "rchaput.pro@gmail.com" },
 ]
 description = "A RL environment for learning ethically-aligned behaviours in a Smart Grid simulator."
@@ -69,10 +69,10 @@
     "/*.ipynb",
     "/.pytest_cache",
     "/.ruff_cache",
 ]
 
 # Also include the `data` folder, and move it to `smartgrid/data` when installed.
 [tool.hatch.build.targets.wheel]
-only-include = ["smartgrid", "data"]
+only-include = ["smartgrid", "data", "algorithms"]
 [tool.hatch.build.targets.wheel.sources]
 "data" = "smartgrid/data"
```

### Comparing `ethical_smart_grid-1.0.0/PKG-INFO` & `ethical_smart_grid-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethical-smart-grid
-Version: 1.0.0
+Version: 1.1.0
 Summary: A RL environment for learning ethically-aligned behaviours in a Smart Grid simulator.
 Project-URL: Source code, https://github.com/ethicsai/ethical-smart-grid
 Project-URL: Bug Tracker, https://github.com/ethicsai/ethical-smart-grid/issues
 Project-URL: Documentation, https://ethicsai.github.io/ethical-smart-grid/
 Author-email: Clément Scheirlinck <clement.scheirlinck@etu.univ-lyon1.fr>
 Maintainer-email: Rémy Chaput <rchaput.pro@gmail.com>
 License: MIT License
@@ -59,14 +59,21 @@
 Requires-Dist: pytest~=7.2.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Ethical Smart Grid Simulator
 
 > Authors: Clément Scheirlinck, Rémy Chaput
 
+<!-- Badges -->
+![](https://img.shields.io/pypi/pyversions/ethical-smart-grid)
+[![](https://img.shields.io/github/actions/workflow/status/ethicsai/ethical-smart-grid/docs.yml?label=Docs)](https://github.com/ethicsai/ethical-smart-grid/actions/workflows/docs.yml)
+[![](https://img.shields.io/github/actions/workflow/status/ethicsai/ethical-smart-grid/testing.yml?label=Automatic%20testing)](https://github.com/ethicsai/ethical-smart-grid/actions/workflows/testing.yml)
+![](https://img.shields.io/pypi/l/ethical-smart-grid)
+![](https://img.shields.io/github/v/release/ethicsai/ethical-smart-grid)
+
 ## Description
 
 This is a third-party [Gym] environment, focusing on learning ethically-aligned
 behaviours in a Smart Grid use-case.
 
 A Smart Grid contains several *prosumer* (prosumer-consumer) agents that
 interact in a shared environment by consuming and exchanging energy.
@@ -83,44 +90,57 @@
 Clone this repository, open a Python shell (3.7+), and execute the following
 instructions:
 
 ```python
 from smartgrid import make_basic_smartgrid
 from algorithms.qsom import QSOM
 
-env = make_basic_smartgrid()
+env = make_basic_smartgrid(max_step=10)
 model = QSOM(env)
 
 done = False
 obs = env.reset()
 while not done:
     actions = model.forward(obs)
     obs, rewards, terminated, truncated, _ = env.step(actions)
+    print(rewards)
     model.backward(obs, rewards)
     done = all(terminated) or all(truncated)
+
 env.close()
 ```
 
+This will initialize a SmartGrid environment, learning agents that use the QSOM
+algorithm, and run the simulation for 10 steps (configurable through the `max_step=10`
+argument).
+
+To go further, please refer to the [documentation]; the [Custom scenario] and
+[Adding a new model] pages can be particularly interesting to learn,
+respectively, how to configure the environment, and how to implement a new
+learning algorithm.
+Finally, [extending the environment][Extending] allows creating new components
+(agents' profiles, reward functions, ...) to further customize the environment.
+
 ## Versioning
 
 This project follows the [Semver] (Semantic Versioning): all versions respect
 the `<major>.<minor>.<patch>` format. The `patch` number is increased when a
 bugfix is released. The `minor` number is increased when new features are added
 that *do not* break the code public API, i.e., it is compatible with the
 previous minor version. Finally, the `major` number is increased when a breaking
 change is introduced; an important distinction is that such a change may not
 be "important" in terms of lines of code, or number of features modified.
 Simply changing a function's return type can be considered a breaking change
 in the public API, and thus worthy of a "major" update.
 
 ## Building and testing locally
 
-This GitHub repository includes actions that automatically [test](actions-test)
-the package and [build](actions-docs) the documentation on each commit, and 
-[publish](actions-publish) the package to [PyPi] on each release.
+This GitHub repository includes actions that automatically [test][actions-test]
+the package and [build][actions-docs] the documentation on each commit, and 
+[publish][actions-publish] the package to [PyPi] on each release.
 
 Instructions to perform these steps locally are given here, for potential
 new contributors or forks:
 
 - *Running the tests*
 
 Tests are defined using [unittest] and run through [pytest]; please install it
@@ -149,24 +169,62 @@
 To build the package, use `hatch build` at the root of this repository. This
 will create the *source distribution* (sdist) at
 `dist/ethica_smart_grid_simulator-<version>.tar.gz`, and the *built distribution*
 (wheel) at `dist/ethical_smart_grid_simulator-<version>-py3-none-any.whl`.
 
 To publish these files to [PyPi], use `hatch publish`.
 
+
+## Community
+
+The community guidelines are available in the [CONTRIBUTING.md](CONTRIBUTING.md)
+file; you can find a (short) summary below.
+
+### Getting support
+
+If you have a question (something that is not clear, how to get a specific
+result, ...), do not hesitate to create a new [Discussion under the Q&A category](https://github.com/ethicsai/ethical-smart-grid/discussions/new?category=q-a).
+
+Please do *not* use the issue tracker for support, to avoid cluttering it.
+
+### Report a bug
+
+If you found a bug (an error raised, or something not working as expected), you
+can report it on the [Issue Tracker](https://github.com/ethicsai/ethical-smart-grid/issues/new).
+
+Please try to be as *precise* as possible.
+
+### Contributing
+
+We very much welcome and appreciate contributions!
+
+For fixing bugs, or improving the documentation, you can create a
+[Pull Request](https://github.com/ethicsai/ethical-smart-grid/pulls).
+
+New features are also welcome, but larger features should be discussed first in
+a new [Discussion under the Ideas category](https://github.com/ethicsai/ethical-smart-grid/discussions/new?category=ideas).
+
+All ideas, suggestions, and requests are also welcome for discussion.
+
+
 ## License
 
 The source code is licensed under the [MIT License].
 Some included data may be protected by other licenses, please refer to the
 [LICENSE.md] file for details.
 
 [Gym]: https://gymnasium.farama.org/
+[documentation]: https://ethicsai.github.io/ethical-smart-grid/
+[Custom scenario]: https://ethicsai.github.io/ethical-smart-grid/custom_scenario.html
+[Adding a new model]: https://ethicsai.github.io/ethical-smart-grid/adding_model.html
+[Extending]: https://ethicsai.github.io/ethical-smart-grid/extending/index.html
 [Semver]: https://semver.org/
 [PyPi]: https://pypi.org/project/ethical-smart-grid/
 [unittest]: https://docs.python.org/3/library/unittest.html
 [pytest]: https://pytest.org/
 [actions-test]: https://github.com/ethicsai/ethical-smart-grid/actions/workflows/testing.yml
 [actions-docs]: https://github.com/ethicsai/ethical-smart-grid/actions/workflows/docs.yml
 [actions-publish]: https://github.com/ethicsai/ethical-smart-grid/actions/workflows/package.yml
+[Sphinx]: https://www.sphinx-doc.org/
 [hatch]: https://hatch.pypa.io/latest/
 [MIT License]: https://choosealicense.com/licenses/mit/
 [LICENSE.md]: LICENSE.md
```

