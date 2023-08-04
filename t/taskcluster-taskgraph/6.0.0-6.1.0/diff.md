# Comparing `tmp/taskcluster-taskgraph-6.0.0.tar.gz` & `tmp/taskcluster-taskgraph-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-6.0.0.tar", last modified: Tue Jul 25 19:06:11 2023, max compression
+gzip compressed data, was "taskcluster-taskgraph-6.1.0.tar", last modified: Fri Aug  4 14:22:18 2023, max compression
```

## Comparing `taskcluster-taskgraph-6.0.0.tar` & `taskcluster-taskgraph-6.1.0.tar`

### file list

```diff
@@ -1,148 +1,150 @@
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    16725 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/LICENSE
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      175 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/MANIFEST.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/PKG-INFO
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3659 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/README.rst
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      602 2023-05-15 20:06:30.000000 taskcluster-taskgraph-6.0.0/pyproject.toml
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.692823 taskcluster-taskgraph-6.0.0/requirements/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      179 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/requirements/base.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    20339 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/requirements/base.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       22 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/requirements/dev.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1281 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/requirements/dev.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       58 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/requirements/test.in
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9241 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/requirements/test.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       38 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/setup.cfg
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1555 2023-05-09 14:44:30.000000 taskcluster-taskgraph-6.0.0/setup.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.688823 taskcluster-taskgraph-6.0.0/src/
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.696823 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4054 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        1 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       50 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      203 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       10 2023-07-25 19:06:11.000000 taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.696823 taskcluster-taskgraph-6.0.0/src/taskgraph/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      729 2023-07-25 19:03:48.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/__init__.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      416 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1836 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/add_new_jobs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1309 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1941 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel_all.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1086 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13122 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/registry.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9387 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/retrigger.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10661 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/actions/util.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4822 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/config.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5184 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/create.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12882 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7834 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2793 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/files_changed.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      866 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/filter_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15667 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/generator.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4680 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/graph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1185 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/default.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2147 2023-03-28 13:22:32.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/loader/transform.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    26201 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/main.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9192 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/morph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.700823 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      123 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18341 2023-05-29 20:22:45.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2380 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/strategies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11918 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/parameters.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    29990 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/fetch-content
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)      896 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/hgrc
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    30813 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/robustcheckout.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    45128 2023-07-12 13:54:36.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/run-task
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3324 2023-02-24 14:13:32.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/target_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3240 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2434 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/taskgraph.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      110 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5146 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2607 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      707 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/code_review.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7606 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/docker_image.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10479 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/fetch.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6760 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/from_deps.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.704823 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    17324 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5897 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/common.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1220 2023-05-25 14:12:26.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/index_search.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8385 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6015 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/toolchain.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6019 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/notify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    52254 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4272 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task_context.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.712823 taskcluster-taskgraph-6.0.0/src/taskgraph/util/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/__init__.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2855 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/archive.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2964 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/attributes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3406 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2433 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2734 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/dependencies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11699 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1661 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/hash.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3419 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/keyed_by.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1331 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/memoize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3184 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/parameterization.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4466 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1576 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/python_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      787 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/readonlydict.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8323 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/schema.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1317 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/shell.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12445 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskcluster.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1969 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskgraph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2139 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/templates.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3390 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/time.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2687 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/treeherder.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18780 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/vcs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8947 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/verify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2498 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/workertypes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      990 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/src/taskgraph/util/yaml.py
-drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-07-25 19:06:11.724823 taskcluster-taskgraph-6.0.0/test/
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1584 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_actions_rebuild_cached_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1670 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_actions_registry.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3654 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_create.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7688 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/test/test_decision.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3505 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_files_changed.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8883 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_generator.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7063 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_graph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7940 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/test/test_main.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2701 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_morph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15584 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.0.0/test/test_optimize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1727 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_optimize_strategies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13921 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.0.0/test/test_parameters.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2491 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/test/test_scripts_fetch_content.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12257 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/test/test_scripts_run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12046 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_target_tasks.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3759 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_taskgraph.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1812 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.0.0/test/test_transform_docker_image.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2716 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transform_task_context.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      874 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_base.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1527 2023-05-02 13:16:10.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_fetch.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6985 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_from_deps.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3798 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6157 2023-07-25 18:49:08.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job_run_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7131 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_job_toolchain.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6948 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_notify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    25785 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.0.0/test/test_transforms_task.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3596 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_attributes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1120 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.0.0/test/test_util_dependencies.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10212 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_docker.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2340 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_memoize.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7556 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.0.0/test/test_util_parameterization.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5906 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1045 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_python_path.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1234 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_readonlydict.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6961 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_schema.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10115 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.0.0/test/test_util_taskcluster.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     1677 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_templates.py
--rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     2239 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_time.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      913 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_treeherder.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15598 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.0.0/test/test_util_vcs.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4981 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.0.0/test/test_util_verify.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      942 2023-03-03 20:39:07.000000 taskcluster-taskgraph-6.0.0/test/test_util_workertypes.py
--rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1005 2023-07-24 11:50:22.000000 taskcluster-taskgraph-6.0.0/test/test_util_yaml.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.198424 taskcluster-taskgraph-6.1.0/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    16725 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/LICENSE
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      175 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.1.0/MANIFEST.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-08-04 14:22:18.198424 taskcluster-taskgraph-6.1.0/PKG-INFO
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3659 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/README.rst
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      602 2023-05-15 20:06:30.000000 taskcluster-taskgraph-6.1.0/pyproject.toml
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.186424 taskcluster-taskgraph-6.1.0/requirements/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      179 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/requirements/base.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    20339 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/requirements/base.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       22 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.1.0/requirements/dev.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1281 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.1.0/requirements/dev.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       58 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.1.0/requirements/test.in
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9241 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/requirements/test.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       38 2023-08-04 14:22:18.198424 taskcluster-taskgraph-6.1.0/setup.cfg
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1555 2023-05-09 14:44:30.000000 taskcluster-taskgraph-6.1.0/setup.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.182424 taskcluster-taskgraph-6.1.0/src/
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.186424 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      665 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4123 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        1 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       50 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      203 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)       10 2023-08-04 14:22:18.000000 taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.186424 taskcluster-taskgraph-6.1.0/src/taskgraph/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      729 2023-08-04 14:21:11.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/__init__.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      416 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1836 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/add_new_jobs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1309 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/cancel.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1941 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/cancel_all.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1086 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13122 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/registry.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9387 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/retrigger.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10661 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/actions/util.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4822 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/config.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5184 2023-03-27 14:05:26.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/create.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12882 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7834 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2793 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/files_changed.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      866 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/filter_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15667 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/generator.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4680 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/graph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/loader/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/loader/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1185 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/loader/default.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2147 2023-03-28 13:22:32.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/loader/transform.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    26201 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/main.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9192 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/morph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      123 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18341 2023-05-29 20:22:45.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2380 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/strategies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11918 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/parameters.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    29990 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/fetch-content
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)      896 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/hgrc
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    30813 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/robustcheckout.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)    45128 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/run-task
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3324 2023-02-24 14:13:32.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/target_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3240 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2434 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/taskgraph.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      110 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5146 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2607 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2592 2023-08-04 14:11:25.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/chunking.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      707 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/code_review.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7606 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/docker_image.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10479 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/fetch.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8734 2023-08-04 14:11:25.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/from_deps.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.190424 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    17458 2023-08-04 14:11:25.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5897 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/common.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1220 2023-05-25 14:12:26.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/index_search.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8385 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6015 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/toolchain.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6019 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/notify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    52254 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4272 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/task_context.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.194424 taskcluster-taskgraph-6.1.0/src/taskgraph/util/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)        0 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/__init__.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2855 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/archive.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2964 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/attributes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3406 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2433 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2734 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/dependencies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    11699 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1661 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/hash.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3419 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/keyed_by.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1331 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 bhearsum  (1000) bhearsum  (1000)     3184 2023-08-04 13:27:58.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/parameterization.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4466 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1576 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/python_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      787 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/readonlydict.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8323 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/schema.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1317 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/shell.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12445 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/taskcluster.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1969 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/taskgraph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2139 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/templates.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3390 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/time.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2687 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/treeherder.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    18780 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/vcs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8947 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/verify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2498 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/workertypes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      990 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/src/taskgraph/util/yaml.py
+drwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)        0 2023-08-04 14:22:18.198424 taskcluster-taskgraph-6.1.0/test/
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1584 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_actions_rebuild_cached_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1670 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_actions_registry.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3654 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_create.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7688 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.1.0/test/test_decision.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3505 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_files_changed.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     8883 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/test/test_generator.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7063 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/test/test_graph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7940 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.1.0/test/test_main.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2701 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_morph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15584 2023-06-05 16:10:05.000000 taskcluster-taskgraph-6.1.0/test/test_optimize.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1727 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_optimize_strategies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    13921 2023-03-14 14:30:55.000000 taskcluster-taskgraph-6.1.0/test/test_parameters.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2491 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/test/test_scripts_fetch_content.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12257 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/test/test_scripts_run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    12046 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_target_tasks.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3759 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/test/test_taskgraph.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      814 2023-08-04 14:11:25.000000 taskcluster-taskgraph-6.1.0/test/test_transform_chunking.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1812 2023-05-25 14:01:37.000000 taskcluster-taskgraph-6.1.0/test/test_transform_docker_image.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2716 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/test/test_transform_task_context.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      874 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_base.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1527 2023-05-02 13:16:10.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_fetch.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     9899 2023-08-04 14:11:25.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_from_deps.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3798 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_job.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6157 2023-08-02 16:56:43.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_job_run_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7131 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_job_toolchain.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6948 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_notify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    25785 2023-07-10 15:52:14.000000 taskcluster-taskgraph-6.1.0/test/test_transforms_task.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     3596 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_attributes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1120 2023-06-22 23:33:17.000000 taskcluster-taskgraph-6.1.0/test/test_util_dependencies.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10212 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_docker.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     2340 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_memoize.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     7556 2023-02-01 03:17:01.000000 taskcluster-taskgraph-6.1.0/test/test_util_parameterization.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     5906 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1045 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_python_path.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1234 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_readonlydict.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     6961 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_schema.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    10115 2023-02-27 19:27:15.000000 taskcluster-taskgraph-6.1.0/test/test_util_taskcluster.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     1677 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_templates.py
+-rwxrwxr-x   0 bhearsum  (1000) bhearsum  (1000)     2239 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_time.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      913 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_treeherder.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)    15598 2023-07-07 15:10:12.000000 taskcluster-taskgraph-6.1.0/test/test_util_vcs.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     4981 2023-01-13 21:44:18.000000 taskcluster-taskgraph-6.1.0/test/test_util_verify.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)      942 2023-03-03 20:39:07.000000 taskcluster-taskgraph-6.1.0/test/test_util_workertypes.py
+-rw-rw-r--   0 bhearsum  (1000) bhearsum  (1000)     1005 2023-08-02 15:17:20.000000 taskcluster-taskgraph-6.1.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-6.0.0/LICENSE` & `taskcluster-taskgraph-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/PKG-INFO` & `taskcluster-taskgraph-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 6.0.0
+Version: 6.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-6.0.0/README.rst` & `taskcluster-taskgraph-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/pyproject.toml` & `taskcluster-taskgraph-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/requirements/base.txt` & `taskcluster-taskgraph-6.1.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/requirements/dev.txt` & `taskcluster-taskgraph-6.1.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/requirements/test.txt` & `taskcluster-taskgraph-6.1.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/setup.py` & `taskcluster-taskgraph-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 6.0.0
+Version: 6.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-6.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-6.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 src/taskgraph/run-task/fetch-content
 src/taskgraph/run-task/hgrc
 src/taskgraph/run-task/robustcheckout.py
 src/taskgraph/run-task/run-task
 src/taskgraph/transforms/__init__.py
 src/taskgraph/transforms/base.py
 src/taskgraph/transforms/cached_tasks.py
+src/taskgraph/transforms/chunking.py
 src/taskgraph/transforms/code_review.py
 src/taskgraph/transforms/docker_image.py
 src/taskgraph/transforms/fetch.py
 src/taskgraph/transforms/from_deps.py
 src/taskgraph/transforms/notify.py
 src/taskgraph/transforms/task.py
 src/taskgraph/transforms/task_context.py
@@ -100,14 +101,15 @@
 test/test_optimize.py
 test/test_optimize_strategies.py
 test/test_parameters.py
 test/test_scripts_fetch_content.py
 test/test_scripts_run_task.py
 test/test_target_tasks.py
 test/test_taskgraph.py
+test/test_transform_chunking.py
 test/test_transform_docker_image.py
 test/test_transform_task_context.py
 test/test_transforms_base.py
 test/test_transforms_fetch.py
 test/test_transforms_from_deps.py
 test/test_transforms_job.py
 test/test_transforms_job_run_task.py
```

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "6.0.0"
+__version__ = "6.1.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/config.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/create.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/main.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-6.1.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/task.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/from_deps.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 """
 from copy import deepcopy
 from textwrap import dedent
 
 from voluptuous import Any, Extra, Optional, Required
 
 from taskgraph.transforms.base import TransformSequence
+from taskgraph.transforms.job import fetches_schema
 from taskgraph.util.attributes import attrmatch
-from taskgraph.util.dependencies import GROUP_BY_MAP
+from taskgraph.util.dependencies import GROUP_BY_MAP, get_dependencies
 from taskgraph.util.schema import Schema, validate_schema
 
 FROM_DEPS_SCHEMA = Schema(
     {
         Required("from-deps"): {
             Optional(
                 "kinds",
@@ -33,14 +34,24 @@
                 The first kind in the list is the "primary" kind. The
                 dependency of this kind will be used to derive the label
                 and copy attributes (if `copy-attributes` is True).
                 """.lstrip()
                 ),
             ): list,
             Optional(
+                "set-name",
+                description=dedent(
+                    """
+                When True, `from_deps` will derive a name for the generated
+                tasks from the name of the primary dependency. Defaults to
+                True.
+                """.lstrip()
+                ),
+            ): bool,
+            Optional(
                 "with-attributes",
                 description=dedent(
                     """
                 Limit dependencies to tasks whose attributes match
                 using :func:`~taskgraph.util.attributes.attrmatch`.
                 """.lstrip()
                 ),
@@ -76,14 +87,25 @@
                     """
                 If true (the default), there must be only a single unique task
                 for each kind in a dependency group. Setting this to false
                 disables that requirement.
                 """.lstrip()
                 ),
             ): bool,
+            Optional(
+                "fetches",
+                description=dedent(
+                    """
+                If present, a `fetches` entry will be added for each task
+                dependency. Attributes of the upstream task may be used as
+                substitution values in the `artifact` or `dest` values of the
+                `fetches` entry.
+                """.lstrip()
+                ),
+            ): {str: [fetches_schema]},
         },
         Extra: object,
     },
 )
 """Schema for from_deps transforms."""
 
 transforms = TransformSequence()
@@ -144,16 +166,18 @@
                 )
             groups = func(config, deps, arg)
         else:
             func = GROUP_BY_MAP[group_by]
             groups = func(config, deps)
 
         # Split the task, one per group.
+        set_name = from_deps.get("set-name", True)
         copy_attributes = from_deps.get("copy-attributes", False)
         unique_kinds = from_deps.get("unique-kinds", True)
+        fetches = from_deps.get("fetches", [])
         for group in groups:
             # Verify there is only one task per kind in each group.
             group_kinds = {t.kind for t in group}
             if unique_kinds and len(group_kinds) < len(group):
                 raise Exception(
                     "The from_deps transforms only allow a single task per kind in a group!"
                 )
@@ -173,18 +197,41 @@
 
             new_task.setdefault("attributes", {})[
                 "primary-kind-dependency"
             ] = primary_kind
 
             primary_dep = [dep for dep in group if dep.kind == primary_kind][0]
 
-            if primary_dep.label.startswith(primary_kind):
-                new_task["name"] = primary_dep.label[len(primary_kind) + 1 :]
-            else:
-                new_task["name"] = primary_dep.label
+            if set_name:
+                if primary_dep.label.startswith(primary_kind):
+                    new_task["name"] = primary_dep.label[len(primary_kind) + 1 :]
+                else:
+                    new_task["name"] = primary_dep.label
 
             if copy_attributes:
-                attrs = new_task.get("attributes", {})
+                attrs = new_task.setdefault("attributes", {})
                 new_task["attributes"] = primary_dep.attributes.copy()
                 new_task["attributes"].update(attrs)
 
+            if fetches:
+                task_fetches = new_task.setdefault("fetches", {})
+
+                for dep_task in get_dependencies(config, new_task):
+                    fetches_from_dep = []
+                    for kind, kind_fetches in fetches.items():
+                        if kind != dep_task.kind:
+                            continue
+
+                        for fetch in kind_fetches:
+                            entry = fetch.copy()
+                            entry["artifact"] = entry["artifact"].format(
+                                **dep_task.attributes
+                            )
+                            if "dest" in entry:
+                                entry["dest"] = entry["dest"].format(
+                                    **dep_task.attributes
+                                )
+                            fetches_from_dep.append(entry)
+
+                    task_fetches[dep_task.label] = fetches_from_dep
+
             yield new_task
```

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,24 @@
 from taskgraph.util.python_path import import_sibling_modules
 from taskgraph.util.schema import Schema, validate_schema
 from taskgraph.util.taskcluster import get_artifact_prefix
 from taskgraph.util.workertypes import worker_type_implementation
 
 logger = logging.getLogger(__name__)
 
+# Fetches may be accepted in other transforms and eventually passed along
+# to a `job` (eg: from_deps). Defining this here allows them to re-use
+# the schema and avoid duplication.
+fetches_schema = {
+    Required("artifact"): str,
+    Optional("dest"): str,
+    Optional("extract"): bool,
+    Optional("verify-hash"): bool,
+}
+
 # Schema for a build description
 job_description_schema = Schema(
     {
         # The name of the job and the job's label.  At least one must be specified,
         # and the label will be generated from the name if necessary, by prepending
         # the kind.
         Optional("name"): str,
@@ -72,20 +82,15 @@
             Optional("files-changed"): [str],
         },
         # A list of artifacts to install from 'fetch' tasks.
         Optional("fetches"): {
             Any("toolchain", "fetch"): [str],
             str: [
                 str,
-                {
-                    Required("artifact"): str,
-                    Optional("dest"): str,
-                    Optional("extract"): bool,
-                    Optional("verify-hash"): bool,
-                },
+                fetches_schema,
             ],
         },
         # A description of how to run this job.
         "run": {
             # The key to a job implementation in a peer module to this one
             "using": str,
             # Base work directory used to set up the task.
```

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/transforms/task_context.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/transforms/task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-6.1.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-6.1.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_actions_registry.py` & `taskcluster-taskgraph-6.1.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_create.py` & `taskcluster-taskgraph-6.1.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_decision.py` & `taskcluster-taskgraph-6.1.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_files_changed.py` & `taskcluster-taskgraph-6.1.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_generator.py` & `taskcluster-taskgraph-6.1.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_graph.py` & `taskcluster-taskgraph-6.1.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_main.py` & `taskcluster-taskgraph-6.1.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_morph.py` & `taskcluster-taskgraph-6.1.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_optimize.py` & `taskcluster-taskgraph-6.1.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-6.1.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_parameters.py` & `taskcluster-taskgraph-6.1.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-6.1.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-6.1.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_target_tasks.py` & `taskcluster-taskgraph-6.1.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_taskgraph.py` & `taskcluster-taskgraph-6.1.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-6.1.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transform_task_context.py` & `taskcluster-taskgraph-6.1.0/test/test_transform_task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_base.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_from_deps.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,14 +82,57 @@
 
 def assert_group_by_all_dupe_allowed(tasks):
     handle_exception(tasks)
     assert len(tasks) == 1
     assert tasks[0]["dependencies"] == {"a": "a", "b": "b", "c": "c"}
 
 
+def assert_dont_set_name(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 1
+    assert tasks[0]["name"] == "a-special-name"
+
+
+def assert_group_by_all_with_fetch(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 1
+    assert tasks[0]["dependencies"] == {
+        "foo1": "foo1",
+        "foo2": "foo2",
+        "foo3": "foo3",
+        "foo4": "foo4",
+    }
+    assert tasks[0]["fetches"] == {
+        "foo1": [
+            {
+                "artifact": "foo.1.txt",
+                "dest": "foo-1.txt",
+            },
+        ],
+        "foo2": [
+            {
+                "artifact": "foo.2.txt",
+                "dest": "foo-2.txt",
+            },
+        ],
+        "foo3": [
+            {
+                "artifact": "foo.3.txt",
+                "dest": "foo-3.txt",
+            },
+        ],
+        "foo4": [
+            {
+                "artifact": "foo.4.txt",
+                "dest": "foo-4.txt",
+            },
+        ],
+    }
+
+
 @pytest.mark.parametrize(
     "task, kind_config, deps",
     (
         pytest.param(
             # task
             {"from-deps": {}},
             # kind config
@@ -114,14 +157,29 @@
             None,
             # deps
             None,
             id="defaults",
         ),
         pytest.param(
             # task
+            {
+                "name": "a-special-name",
+                "from-deps": {
+                    "group-by": "all",
+                    "set-name": False,
+                },
+            },
+            # kind config
+            None,
+            # deps
+            None,
+            id="dont_set_name",
+        ),
+        pytest.param(
+            # task
             {"from-deps": {}},
             # kind config
             None,
             # deps
             None,
             id="group_by_single",
         ),
@@ -217,14 +275,59 @@
             {
                 "a": make_task("a", kind="foo"),
                 "b": make_task("b", kind="foo"),
                 "c": make_task("c", kind="foo"),
             },
             id="group_by_all_dupe_allowed",
         ),
+        pytest.param(
+            # task
+            {
+                "from-deps": {
+                    "group-by": "all",
+                    "unique-kinds": False,
+                    "kinds": ["foo"],
+                    "fetches": {
+                        "foo": [
+                            {
+                                "artifact": "foo.{this_chunk}.txt",
+                                "dest": "foo-{this_chunk}.txt",
+                            },
+                        ],
+                    },
+                },
+            },
+            # kind config
+            None,
+            # deps
+            {
+                "foo1": make_task(
+                    "foo1",
+                    kind="foo",
+                    attributes={"this_chunk": "1", "total_chunks": "4", "kind": "foo"},
+                ),
+                "foo2": make_task(
+                    "foo2",
+                    kind="foo",
+                    attributes={"this_chunk": "2", "total_chunks": "4", "kind": "foo"},
+                ),
+                "foo3": make_task(
+                    "foo3",
+                    kind="foo",
+                    attributes={"this_chunk": "3", "total_chunks": "4", "kind": "foo"},
+                ),
+                "foo4": make_task(
+                    "foo4",
+                    kind="foo",
+                    attributes={"this_chunk": "4", "total_chunks": "4", "kind": "foo"},
+                ),
+                "bar": make_task("bar", kind="bar", attributes={"kind": "bar"}),
+            },
+            id="group_by_all_with_fetch",
+        ),
     ),
 )
 def test_transforms(
     request, make_transform_config, run_transform, task, kind_config, deps
 ):
     task.setdefault("name", "task")
     task.setdefault("description", "description")
```

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_job.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_transforms_task.py` & `taskcluster-taskgraph-6.1.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_attributes.py` & `taskcluster-taskgraph-6.1.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-6.1.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_docker.py` & `taskcluster-taskgraph-6.1.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_memoize.py` & `taskcluster-taskgraph-6.1.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-6.1.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_path.py` & `taskcluster-taskgraph-6.1.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_python_path.py` & `taskcluster-taskgraph-6.1.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-6.1.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_schema.py` & `taskcluster-taskgraph-6.1.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-6.1.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_templates.py` & `taskcluster-taskgraph-6.1.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_time.py` & `taskcluster-taskgraph-6.1.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-6.1.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_vcs.py` & `taskcluster-taskgraph-6.1.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_verify.py` & `taskcluster-taskgraph-6.1.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-6.1.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-6.0.0/test/test_util_yaml.py` & `taskcluster-taskgraph-6.1.0/test/test_util_yaml.py`

 * *Files identical despite different names*

