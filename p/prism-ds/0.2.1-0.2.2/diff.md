# Comparing `tmp/prism-ds-0.2.1.tar.gz` & `tmp/prism-ds-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prism-ds-0.2.1.tar", last modified: Wed Aug  2 01:51:02 2023, max compression
+gzip compressed data, was "prism-ds-0.2.2.tar", last modified: Fri Aug  4 02:28:35 2023, max compression
```

## Comparing `prism-ds-0.2.1.tar` & `prism-ds-0.2.2.tar`

### file list

```diff
@@ -1,473 +1,476 @@
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.623278 prism-ds-0.2.1/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.1/LICENSE
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.1/MANIFEST.in
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5522 2023-08-02 01:51:02.623398 prism-ds-0.2.1/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4561 2023-07-20 13:03:06.000000 prism-ds-0.2.1/README.md
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.431580 prism-ds-0.2.1/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.1/prism/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/admin.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.433341 prism-ds-0.2.1/prism/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7762 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18549 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/docker_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    43144 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/agents/ec2.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/agents/meta.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.434233 prism-ds-0.2.1/prism/agents/scripts/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.1/prism/agents/scripts/__init__.py
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3447 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/agents/scripts/apply.sh
--rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.1/prism/agents/scripts/run.sh
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.437209 prism-ds-0.2.1/prism/cli/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/cli/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10729 2023-07-22 13:39:04.000000 prism-ds-0.2.1/prism/cli/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7470 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10421 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4817 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/cli/init.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9402 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/cli/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/cli/spark_submit.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.437466 prism-ds-0.2.1/prism/client/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    16701 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/client/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4970 2023-08-02 01:20:09.000000 prism-ds-0.2.1/prism/constants.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.438182 prism-ds-0.2.1/prism/decorators/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/decorators/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.438412 prism-ds-0.2.1/prism/docs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/docs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.442170 prism-ds-0.2.1/prism/docs/build/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/311ea03002abadcdcaba.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/54968a39190c43d592b9.svg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/docs/build/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/ce188596011a8fa32931.png
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560712 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/docs/build/index.html
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-07-18 21:18:50.000000 prism-ds-0.2.1/prism/docs/build/main.js.LICENSE.txt
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.442546 prism-ds-0.2.1/prism/event_managers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/event_managers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-07-13 03:54:01.000000 prism-ds-0.2.1/prism/event_managers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7852 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/exceptions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.444820 prism-ds-0.2.1/prism/infra/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/infra/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6833 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/compiled_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14303 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/compiler.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13388 2023-08-02 01:20:09.000000 prism-ds-0.2.1/prism/infra/executor.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3900 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2704 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/manifest.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3716 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/pipeline.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1421 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/infra/sys_path.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2628 2023-07-31 12:18:05.000000 prism-ds-0.2.1/prism/infra/task_manager.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24529 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/main.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.447147 prism-ds-0.2.1/prism/mixins/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/mixins/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/mixins/agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3165 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/mixins/aws.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1288 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11668 2023-07-31 12:14:11.000000 prism-ds-0.2.1/prism/mixins/compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/create_agent.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5706 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/create_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/mixins/create_trigger.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/mixins/graph.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.1/prism/mixins/run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4232 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/mixins/sys_handler.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.447859 prism-ds-0.2.1/prism/parsers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/parsers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31631 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/parsers/ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-07-15 21:15:27.000000 prism-ds-0.2.1/prism/parsers/base.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/parsers/yml_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22013 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/prism_logging.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450070 prism-ds-0.2.1/prism/profiles/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/profiles/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/profiles/adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3733 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/bigquery.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15570 2023-08-01 03:49:48.000000 prism-ds-0.2.1/prism/profiles/dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/profiles/meta.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4567 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-07-05 11:15:15.000000 prism-ds-0.2.1/prism/profiles/profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/profiles/pyspark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4557 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/redshift.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4176 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/profiles/trino.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450596 prism-ds-0.2.1/prism/spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/spark/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/spark/script.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/spark/wrapper.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1448 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.450753 prism-ds-0.2.1/prism/templates/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.1/prism/templates/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.451404 prism-ds-0.2.1/prism/templates/agents/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/agents/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/agents/docker.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.1/prism/templates/agents/ec2.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.451978 prism-ds-0.2.1/prism/templates/minimal_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/minimal_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/minimal_project/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1326 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452328 prism-ds-0.2.1/prism/templates/minimal_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/minimal_project/tasks/decorated_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452496 prism-ds-0.2.1/prism/templates/profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.452807 prism-ds-0.2.1/prism/templates/profile/bigquery/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/bigquery/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453107 prism-ds-0.2.1/prism/templates/profile/dbt/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/dbt/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453345 prism-ds-0.2.1/prism/templates/profile/postgres/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/postgres/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453510 prism-ds-0.2.1/prism/templates/profile/pyspark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/pyspark/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453670 prism-ds-0.2.1/prism/templates/profile/redshift/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/redshift/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453832 prism-ds-0.2.1/prism/templates/profile/snowflake/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/snowflake/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.453985 prism-ds-0.2.1/prism/templates/profile/trino/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/templates/profile/trino/profile.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.454612 prism-ds-0.2.1/prism/templates/starter_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/templates/starter_project/.gitignore
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/starter_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.454898 prism-ds-0.2.1/prism/templates/starter_project/data/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/starter_project/data/.exists
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455007 prism-ds-0.2.1/prism/templates/starter_project/dev/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      786 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/dev/dev.ipynb
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455174 prism-ds-0.2.1/prism/templates/starter_project/output/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.1/prism/templates/starter_project/output/.exists
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.455454 prism-ds-0.2.1/prism/templates/starter_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/templates/starter_project/tasks/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/starter_project/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.456563 prism-ds-0.2.1/prism/templates/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/pyspark_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/pyspark_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/python_cls.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.1/prism/templates/tasks/python_dec.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/tasks/sql.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.457052 prism-ds-0.2.1/prism/templates/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/templates/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/triggers/function.yml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/templates/triggers/prism_project.yml
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.457245 prism-ds-0.2.1/prism/tests/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.460271 prism-ds-0.2.1/prism/tests/integration/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/integration/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7886 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/integration_test_class.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15381 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_client.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10484 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_compile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/tests/integration/test_connect.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6512 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_create.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4012 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_dbt.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5728 2023-08-01 13:15:50.000000 prism-ds-0.2.1/prism/tests/integration/test_hooks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.1/prism/tests/integration/test_init.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.425999 prism-ds-0.2.1/prism/tests/integration/test_projects/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.461343 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-08-01 03:53:18.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.462126 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.462557 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1343 2023-08-01 03:53:18.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.463131 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.463425 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464090 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      825 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464365 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.464861 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      806 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      807 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.465111 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.466439 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      935 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1027 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      801 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1033 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.467453 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.468294 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1100 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      868 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.471493 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.477865 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1127 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      923 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      913 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.481120 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.486764 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      969 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      974 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      910 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1257 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.487861 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.495540 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1751 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1139 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      940 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      636 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.496498 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.504216 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      982 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1548 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1632 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1765 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/parquet.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      498 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/txt.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.508391 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.508528 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.509054 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      569 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.515156 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.515594 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.522136 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1059 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.522403 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.525616 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-09 15:09:25.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.525948 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526330 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1067 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526516 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.526820 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.529696 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1196 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1195 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1045 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.532132 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.540889 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1239 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      597 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.541371 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.543667 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1287 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1133 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1871 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.543963 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.544982 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module02.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.547303 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1151 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.548605 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/module01.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.555398 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.555874 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.556384 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.556674 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.557122 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.559756 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560145 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560503 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.560959 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.561388 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/utils.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.561684 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.562315 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      687 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      995 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.562724 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.563033 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      388 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/extract.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      785 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.563299 prism-ds-0.2.1/prism/tests/integration/test_projects/common/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/common/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/integration/test_projects/common/functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    54115 2023-07-22 18:17:28.000000 prism-ds-0.2.1/prism/tests/integration/test_run.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14051 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_spark_submit.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5594 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/integration/test_targets.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.568903 prism-ds-0.2.1/prism/tests/unit/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.572845 prism-ds-0.2.1/prism/tests/unit/dummy_modules/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/unit/dummy_modules/dummy_module1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.1/prism/tests/unit/test_adapter_profile.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.572963 prism-ds-0.2.1/prism/tests/unit/test_agent/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1230 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_agent/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10244 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_agents.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    28403 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_dag_fns.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.573223 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       65 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/__init__.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.577953 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.584243 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      467 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task03.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      172 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task04.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task05.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task06.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      365 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task07.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task08.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      169 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task09.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task10.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task11.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task12.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task13.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task14.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task15.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.584840 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task01.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task02.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      145 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task03.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.592323 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      247 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.602033 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      251 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.607573 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      253 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25008 2023-07-20 00:59:23.000000 prism-ds-0.2.1/prism/tests/unit/test_ast_parser.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/test_import.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.1/prism/tests/unit/test_jinja.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.611924 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/no_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/non_null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/null_profile.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      996 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/triggers_normal.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7948 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_project.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.619099 prism-ds-0.2.1/prism/tests/unit/test_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      117 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_bad_run_no_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_diff_import_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      163 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_if_name_main.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      118 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_no_run_func.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_other_classes.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      346 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      329 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/cls_tasks_refs.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_dec_no_parentheses.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_run_extra_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_bad_run_missing_arg.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_diff_decorator_structure.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_multiple_prism_tasks.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_no_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_one_prism_task.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_other_functions.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_task_with_target.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      361 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/dec_tasks_refs.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.620457 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/func_0.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/func_1.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/hello.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_tasks/refd_tasks/world.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8773 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.621592 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      936 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/prism_project.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/test_fn.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.621857 prism-ds-0.2.1/prism/triggers/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19492 2023-07-20 00:59:24.000000 prism-ds-0.2.1/prism/triggers/__init__.py
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.1/prism/ui.py
-drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-02 01:51:02.623169 prism-ds-0.2.1/prism_ds.egg-info/
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5522 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/PKG-INFO
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19334 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/SOURCES.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/dependency_links.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/entry_points.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.1/prism_ds.egg-info/not-zip-safe
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      564 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/requires.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-08-02 01:51:02.000000 prism-ds-0.2.1/prism_ds.egg-info/top_level.txt
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.1/pyproject.toml
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1766 2023-08-02 01:51:02.623823 prism-ds-0.2.1/setup.cfg
--rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.1/setup.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.432286 prism-ds-0.2.2/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11312 2022-08-08 04:50:27.000000 prism-ds-0.2.2/LICENSE
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      219 2023-05-16 12:01:01.000000 prism-ds-0.2.2/MANIFEST.in
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5599 2023-08-04 02:28:35.432470 prism-ds-0.2.2/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4615 2023-08-04 02:16:43.000000 prism-ds-0.2.2/README.md
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.230528 prism-ds-0.2.2/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:34:22.000000 prism-ds-0.2.2/prism/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/admin.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.235456 prism-ds-0.2.2/prism/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7762 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/agents/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    18549 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/agents/docker_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    43144 2023-07-22 18:17:28.000000 prism-ds-0.2.2/prism/agents/ec2.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      533 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/agents/meta.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.237519 prism-ds-0.2.2/prism/agents/scripts/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-16 12:00:13.000000 prism-ds-0.2.2/prism/agents/scripts/__init__.py
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)     3447 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/agents/scripts/apply.sh
+-rwxr-xr-x   0 mihirtrivedi   (501) staff       (20)      710 2023-06-28 01:05:16.000000 prism-ds-0.2.2/prism/agents/scripts/run.sh
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.249821 prism-ds-0.2.2/prism/cli/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/cli/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10729 2023-07-22 13:39:04.000000 prism-ds-0.2.2/prism/cli/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7470 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/cli/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10421 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/cli/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4457 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/cli/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4222 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/cli/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4817 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/cli/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4444 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/cli/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5443 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/cli/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5506 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/cli/init.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9402 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/cli/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      724 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/cli/spark_submit.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.251060 prism-ds-0.2.2/prism/client/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    16701 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/client/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4984 2023-08-04 02:16:43.000000 prism-ds-0.2.2/prism/constants.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.256159 prism-ds-0.2.2/prism/decorators/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/decorators/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7124 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/decorators/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3116 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/decorators/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.256480 prism-ds-0.2.2/prism/docs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/docs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.275336 prism-ds-0.2.2/prism/docs/build/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    50665 2023-07-18 21:18:50.000000 prism-ds-0.2.2/prism/docs/build/311ea03002abadcdcaba.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6035 2023-07-18 21:18:50.000000 prism-ds-0.2.2/prism/docs/build/54968a39190c43d592b9.svg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15406 2023-07-18 21:18:50.000000 prism-ds-0.2.2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       79 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/docs/build/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4653 2023-07-18 21:18:50.000000 prism-ds-0.2.2/prism/docs/build/ce188596011a8fa32931.png
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)   560712 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/docs/build/index.html
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      961 2023-07-18 21:18:50.000000 prism-ds-0.2.2/prism/docs/build/main.js.LICENSE.txt
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.276088 prism-ds-0.2.2/prism/event_managers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/event_managers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6081 2023-07-13 03:54:01.000000 prism-ds-0.2.2/prism/event_managers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7852 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/exceptions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.278487 prism-ds-0.2.2/prism/infra/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/infra/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6833 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/compiled_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14303 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/compiler.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13388 2023-08-02 01:20:09.000000 prism-ds-0.2.2/prism/infra/executor.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3951 2023-08-04 02:16:43.000000 prism-ds-0.2.2/prism/infra/hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2704 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/manifest.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3716 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/pipeline.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    17198 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1421 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/infra/sys_path.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2628 2023-07-31 12:18:05.000000 prism-ds-0.2.2/prism/infra/task_manager.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    24529 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/main.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.286963 prism-ds-0.2.2/prism/mixins/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.2/prism/mixins/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2405 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/mixins/agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3165 2023-07-22 18:17:28.000000 prism-ds-0.2.2/prism/mixins/aws.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1288 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/mixins/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    11668 2023-07-31 12:14:11.000000 prism-ds-0.2.2/prism/mixins/compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7301 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/mixins/connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2312 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/mixins/create_agent.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5706 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/mixins/create_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5428 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/mixins/create_trigger.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2438 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/mixins/graph.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1107 2023-04-02 17:52:18.000000 prism-ds-0.2.2/prism/mixins/run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4232 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/mixins/sys_handler.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.290691 prism-ds-0.2.2/prism/parsers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/parsers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    31631 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/parsers/ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2206 2023-07-15 21:15:27.000000 prism-ds-0.2.2/prism/parsers/base.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3049 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/parsers/yml_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    22013 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/prism_logging.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.296911 prism-ds-0.2.2/prism/profiles/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/profiles/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2745 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/profiles/adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     3733 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/profiles/bigquery.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15570 2023-08-01 03:49:48.000000 prism-ds-0.2.2/prism/profiles/dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      539 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/profiles/meta.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4567 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/profiles/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6381 2023-08-04 02:16:43.000000 prism-ds-0.2.2/prism/profiles/presto.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     9117 2023-07-05 11:15:15.000000 prism-ds-0.2.2/prism/profiles/profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4089 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/profiles/pyspark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4557 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/profiles/redshift.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4176 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/profiles/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6358 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/profiles/trino.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.300701 prism-ds-0.2.2/prism/spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/spark/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      439 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/spark/script.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2889 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/spark/wrapper.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1448 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5171 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.300972 prism-ds-0.2.2/prism/templates/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-17 00:55:51.000000 prism-ds-0.2.2/prism/templates/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.301738 prism-ds-0.2.2/prism/templates/agents/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       59 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/templates/agents/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      233 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/templates/agents/docker.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-05-20 15:36:38.000000 prism-ds-0.2.2/prism/templates/agents/ec2.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.303003 prism-ds-0.2.2/prism/templates/minimal_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-16 12:31:03.000000 prism-ds-0.2.2/prism/templates/minimal_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/minimal_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1326 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/minimal_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.303330 prism-ds-0.2.2/prism/templates/minimal_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/minimal_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/minimal_project/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.303505 prism-ds-0.2.2/prism/templates/profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.303686 prism-ds-0.2.2/prism/templates/profile/bigquery/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/bigquery/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.303946 prism-ds-0.2.2/prism/templates/profile/dbt/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      141 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/dbt/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.304197 prism-ds-0.2.2/prism/templates/profile/postgres/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/postgres/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.306114 prism-ds-0.2.2/prism/templates/profile/presto/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      191 2023-08-04 02:16:43.000000 prism-ds-0.2.2/prism/templates/profile/presto/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.306271 prism-ds-0.2.2/prism/templates/profile/pyspark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      478 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/pyspark/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.306452 prism-ds-0.2.2/prism/templates/profile/redshift/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      180 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/redshift/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.306614 prism-ds-0.2.2/prism/templates/profile/snowflake/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      193 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/snowflake/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.306777 prism-ds-0.2.2/prism/templates/profile/trino/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      189 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/templates/profile/trino/profile.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.307726 prism-ds-0.2.2/prism/templates/starter_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       19 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/templates/starter_project/.gitignore
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/starter_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.308014 prism-ds-0.2.2/prism/templates/starter_project/data/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.2/prism/templates/starter_project/data/.exists
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.308139 prism-ds-0.2.2/prism/templates/starter_project/dev/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      786 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/starter_project/dev/dev.ipynb
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.308337 prism-ds-0.2.2/prism/templates/starter_project/output/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-16 12:31:03.000000 prism-ds-0.2.2/prism/templates/starter_project/output/.exists
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1112 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/starter_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.311336 prism-ds-0.2.2/prism/templates/starter_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/starter_project/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/templates/starter_project/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/starter_project/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.316919 prism-ds-0.2.2/prism/templates/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.2/prism/templates/tasks/pyspark_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.2/prism/templates/tasks/pyspark_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      426 2023-05-27 16:07:03.000000 prism-ds-0.2.2/prism/templates/tasks/python_cls.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      427 2023-05-27 16:07:03.000000 prism-ds-0.2.2/prism/templates/tasks/python_dec.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      155 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/tasks/sql.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.319763 prism-ds-0.2.2/prism/templates/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       61 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/templates/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      267 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/templates/triggers/function.yml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      208 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/templates/triggers/prism_project.yml
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.320112 prism-ds-0.2.2/prism/tests/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.330037 prism-ds-0.2.2/prism/tests/integration/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/integration/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7886 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/integration_test_class.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    15381 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_client.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10484 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_compile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10444 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/tests/integration/test_connect.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     6512 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_create.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4012 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_dbt.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5728 2023-08-01 13:15:50.000000 prism-ds-0.2.2/prism/tests/integration/test_hooks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4539 2023-05-30 01:42:39.000000 prism-ds-0.2.2/prism/tests/integration/test_init.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.219600 prism-ds-0.2.2/prism/tests/integration/test_projects/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.336665 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1120 2023-08-01 03:53:18.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.338042 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      938 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       66 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.340828 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       68 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1343 2023-08-01 03:53:18.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.344559 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1011 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      937 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.344910 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.350320 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      825 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      857 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.353658 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.354298 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      806 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      807 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.354616 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.356642 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      935 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1027 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      801 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1033 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.360533 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.361586 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1100 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      868 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.362312 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      772 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.363454 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      983 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1127 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      923 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      913 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.363947 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.365667 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      969 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1090 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      974 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      910 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1257 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.365961 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.366860 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1751 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1139 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      940 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      636 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.367212 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.372474 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      982 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1548 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1632 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1765 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      498 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/txt.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.372644 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.372752 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.373696 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      569 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      576 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.374137 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.374309 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.375344 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1059 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.375789 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.376096 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-09 15:09:25.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.376820 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.377852 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      934 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1067 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.378110 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      875 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      812 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.378794 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.380606 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1196 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1195 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1045 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      808 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.380882 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.381789 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1239 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      597 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.382103 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.387111 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1287 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1133 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1871 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     2147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1073 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.389707 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.390107 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      345 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/tasks/module02.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.391034 prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1151 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.392869 prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      358 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/tasks/module01.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.393720 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.394045 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.396268 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.396643 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.397502 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.397795 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      773 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.398166 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.398524 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      578 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      620 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.399011 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1211 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.399423 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      399 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      703 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/utils.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.399739 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.400170 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      687 2023-07-22 18:17:28.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      995 2023-07-22 18:17:28.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.400538 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1070 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.400891 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      388 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/extract.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      785 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.401265 prism-ds-0.2.2/prism/tests/integration/test_projects/common/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/common/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      376 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/integration/test_projects/common/functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    54115 2023-07-22 18:17:28.000000 prism-ds-0.2.2/prism/tests/integration/test_run.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    14051 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_spark_submit.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5594 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/integration/test_targets.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.404284 prism-ds-0.2.2/prism/tests/unit/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/unit/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.404583 prism-ds-0.2.2/prism/tests/unit/dummy_modules/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        0 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/unit/dummy_modules/dummy_module1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    13721 2023-06-28 00:14:15.000000 prism-ds-0.2.2/prism/tests/unit/test_adapter_profile.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.404682 prism-ds-0.2.2/prism/tests/unit/test_agent/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1230 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_agent/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    10244 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_agents.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    28403 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_dag_fns.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.404965 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       65 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/__init__.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.406309 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      239 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      173 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      204 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/dag_cycle/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.409571 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      467 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task03.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      172 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task04.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task05.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task06.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      365 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task07.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task08.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      169 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task09.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task10.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      179 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task11.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task12.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      147 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task13.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task14.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      150 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_15nodes/task15.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.410447 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task01.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      146 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task02.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      145 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_3nodes/task03.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.411979 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      247 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      148 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      198 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_5nodes/taskE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.413353 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      251 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_norefs/moduleE.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.414511 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      253 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleA.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      129 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleB.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleC.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleD.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_all_things_dag/task_ref_selfref/moduleE.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    25008 2023-07-20 00:59:23.000000 prism-ds-0.2.2/prism/tests/unit/test_ast_parser.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      405 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/unit/test_import.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     4992 2023-05-26 22:30:47.000000 prism-ds-0.2.2/prism/tests/unit/test_jinja.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.416383 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1068 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      915 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/multiple_profiles.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      879 2022-08-08 04:50:27.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/no_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      909 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/non_null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      894 2023-03-01 23:08:44.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/null_profile.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1000 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      996 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/triggers_normal.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     7948 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_project.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.425826 prism-ds-0.2.2/prism/tests/unit/test_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      133 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      117 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      125 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_bad_run_no_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_diff_import_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      163 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_if_name_main.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      212 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      118 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_no_run_func.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      123 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      185 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_other_classes.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      346 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      329 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/cls_tasks_refs.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       92 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_bad_dec_no_parentheses.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      105 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_bad_run_extra_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       87 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_bad_run_missing_arg.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      124 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_diff_decorator_structure.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      156 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_multiple_prism_tasks.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       49 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_no_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       93 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_one_prism_task.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      126 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_other_functions.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      301 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_task_with_target.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      361 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/dec_tasks_refs.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.429231 prism-ds-0.2.2/prism/tests/unit/test_tasks/refd_tasks/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/refd_tasks/func_0.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/refd_tasks/func_1.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/refd_tasks/hello.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      116 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_tasks/refd_tasks/world.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     8773 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_trigger.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.429655 prism-ds-0.2.2/prism/tests/unit/test_trigger_yml/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      936 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/tests/unit/test_trigger_yml/prism_project.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      111 2023-04-04 01:59:51.000000 prism-ds-0.2.2/prism/tests/unit/test_trigger_yml/test_fn.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.429961 prism-ds-0.2.2/prism/triggers/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19492 2023-07-20 00:59:24.000000 prism-ds-0.2.2/prism/triggers/__init__.py
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      810 2023-05-04 14:39:42.000000 prism-ds-0.2.2/prism/ui.py
+drwxr-xr-x   0 mihirtrivedi   (501) staff       (20)        0 2023-08-04 02:28:35.431868 prism-ds-0.2.2/prism_ds.egg-info/
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     5599 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/PKG-INFO
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)    19402 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       44 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/entry_points.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)        1 2023-06-26 13:49:56.000000 prism-ds-0.2.2/prism_ds.egg-info/not-zip-safe
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      600 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/requires.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       11 2023-08-04 02:28:35.000000 prism-ds-0.2.2/prism_ds.egg-info/top_level.txt
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)      743 2022-11-12 14:33:04.000000 prism-ds-0.2.2/pyproject.toml
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)     1803 2023-08-04 02:28:35.432960 prism-ds-0.2.2/setup.cfg
+-rw-r--r--   0 mihirtrivedi   (501) staff       (20)       70 2023-05-04 13:05:27.000000 prism-ds-0.2.2/setup.py
```

### Comparing `prism-ds-0.2.1/LICENSE` & `prism-ds-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/PKG-INFO` & `prism-ds-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.1
+Version: 0.2.2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -20,14 +20,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: trino
+Provides-Extra: presto
 Provides-Extra: pyspark
 Provides-Extra: dbt
 Provides-Extra: docker
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
@@ -88,14 +89,15 @@
 ### Adapters
 Adapters allow users to connect to data warehouses or analytics engines. Prism currently supports the following adapters:
 | Adapter      | Command |
 | ------------ | ----------- |
 | **dbt** | ```pip install "prism-ds[dbt]"``` |
 | **Google BigQuery** | ```pip install "prism-ds[bigquery]"``` |
 | **Postgres** | ```pip install "prism-ds[postgres]"``` |
+| **Presto** | ```pip install "prism-ds[presto]"``` |
 | **PySpark** | ```pip install "prism-ds[pyspark]"``` |
 | **Redshift** | ```pip install "prism-ds[redshift]"``` |
 | **Snowflake** | ```pip install "prism-ds[snowflake]"``` |
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.1 Summary: The easiest way to
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.2 Summary: The easiest way to
 create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: snowflake Provides-
 Extra: bigquery Provides-Extra: redshift Provides-Extra: postgres Provides-
-Extra: trino Provides-Extra: pyspark Provides-Extra: dbt Provides-Extra: docker
-Provides-Extra: testing License-File: LICENSE
+Extra: trino Provides-Extra: presto Provides-Extra: pyspark Provides-Extra: dbt
+Provides-Extra: docker Provides-Extra: testing License-File: LICENSE
                                  [prism logo]
           [PyPI] [https://static.pepy.tech/personalized-badge/prism-
 ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
 [![CI Linux](https://github.com/runprism/prism/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-linux.yml)
 [![CI MacOS](https://github.com/runprism/prism/actions/workflows/ci-macos.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-macos.yml)
@@ -49,20 +49,21 @@
 (https://github.com/runprism/prism_examples). ## Integrations Prism integrates
 with a wide variety of third-party developer tools There are two kinds of
 integrations that Prism supports: adapters, and agents. ### Adapters Adapters
 allow users to connect to data warehouses or analytics engines. Prism currently
 supports the following adapters: | Adapter | Command | | ------------ | -------
 ---- | | **dbt** | ```pip install "prism-ds[dbt]"``` | | **Google BigQuery** |
 ```pip install "prism-ds[bigquery]"``` | | **Postgres** | ```pip install
-"prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
-| | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
-```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
-ds[trino]"``` | ### Agents Agents allow users to run their projects on external
-computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
-and more. Prism currently supports the following agents: | Agent | Command | |
------------- | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
-We're always looking to improve our product. Here's what we're working on at
-the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
-more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
-**Cloud deployment**: Managed orchestration platform to deploy Prism projects
-in the cloud Let us know if you'd like to see another feature!
+"prism-ds[postgres]"``` | | **Presto** | ```pip install "prism-ds[presto]"``` |
+| **PySpark** | ```pip install "prism-ds[pyspark]"``` | | **Redshift** | ```pip
+install "prism-ds[redshift]"``` | | **Snowflake** | ```pip install "prism-ds
+[snowflake]"``` | | **Trino** | ```pip install "prism-ds[trino]"``` | ###
+Agents Agents allow users to run their projects on external computing
+environments, e.g., Docker containers, EC2 instances, EMR clusters, and more.
+Prism currently supports the following agents: | Agent | Command | | ----------
+-- | ----------- | | **docker** | ```pip install "prism-ds[docker]"``` | |
+**ec2** | N/A - comes with base Prism | ## Product Roadmap We're always looking
+to improve our product. Here's what we're working on at the moment: -
+**Additional Agents**: EMR clusters, Databricks clusters, and more! -
+**Additional adapters**: Celery, Dask, MySQL, Presto, and more! - **Cloud
+deployment**: Managed orchestration platform to deploy Prism projects in the
+cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-ds-0.2.1/README.md` & `prism-ds-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 ### Adapters
 Adapters allow users to connect to data warehouses or analytics engines. Prism currently supports the following adapters:
 | Adapter      | Command |
 | ------------ | ----------- |
 | **dbt** | ```pip install "prism-ds[dbt]"``` |
 | **Google BigQuery** | ```pip install "prism-ds[bigquery]"``` |
 | **Postgres** | ```pip install "prism-ds[postgres]"``` |
+| **Presto** | ```pip install "prism-ds[presto]"``` |
 | **PySpark** | ```pip install "prism-ds[pyspark]"``` |
 | **Redshift** | ```pip install "prism-ds[redshift]"``` |
 | **Snowflake** | ```pip install "prism-ds[snowflake]"``` |
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
```

#### html2text {}

```diff
@@ -36,20 +36,21 @@
 (https://github.com/runprism/prism_examples). ## Integrations Prism integrates
 with a wide variety of third-party developer tools There are two kinds of
 integrations that Prism supports: adapters, and agents. ### Adapters Adapters
 allow users to connect to data warehouses or analytics engines. Prism currently
 supports the following adapters: | Adapter | Command | | ------------ | -------
 ---- | | **dbt** | ```pip install "prism-ds[dbt]"``` | | **Google BigQuery** |
 ```pip install "prism-ds[bigquery]"``` | | **Postgres** | ```pip install
-"prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
-| | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
-```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
-ds[trino]"``` | ### Agents Agents allow users to run their projects on external
-computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
-and more. Prism currently supports the following agents: | Agent | Command | |
------------- | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
-We're always looking to improve our product. Here's what we're working on at
-the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
-more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
-**Cloud deployment**: Managed orchestration platform to deploy Prism projects
-in the cloud Let us know if you'd like to see another feature!
+"prism-ds[postgres]"``` | | **Presto** | ```pip install "prism-ds[presto]"``` |
+| **PySpark** | ```pip install "prism-ds[pyspark]"``` | | **Redshift** | ```pip
+install "prism-ds[redshift]"``` | | **Snowflake** | ```pip install "prism-ds
+[snowflake]"``` | | **Trino** | ```pip install "prism-ds[trino]"``` | ###
+Agents Agents allow users to run their projects on external computing
+environments, e.g., Docker containers, EC2 instances, EMR clusters, and more.
+Prism currently supports the following agents: | Agent | Command | | ----------
+-- | ----------- | | **docker** | ```pip install "prism-ds[docker]"``` | |
+**ec2** | N/A - comes with base Prism | ## Product Roadmap We're always looking
+to improve our product. Here's what we're working on at the moment: -
+**Additional Agents**: EMR clusters, Databricks clusters, and more! -
+**Additional adapters**: Celery, Dask, MySQL, Presto, and more! - **Cloud
+deployment**: Managed orchestration platform to deploy Prism projects in the
+cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-ds-0.2.1/prism/admin.py` & `prism-ds-0.2.2/prism/admin.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/base.py` & `prism-ds-0.2.2/prism/agents/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/docker_agent.py` & `prism-ds-0.2.2/prism/agents/docker_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/ec2.py` & `prism-ds-0.2.2/prism/agents/ec2.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/meta.py` & `prism-ds-0.2.2/prism/agents/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/scripts/apply.sh` & `prism-ds-0.2.2/prism/agents/scripts/apply.sh`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/agents/scripts/run.sh` & `prism-ds-0.2.2/prism/agents/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/agent.py` & `prism-ds-0.2.2/prism/cli/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/base.py` & `prism-ds-0.2.2/prism/cli/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/compile.py` & `prism-ds-0.2.2/prism/cli/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/connect.py` & `prism-ds-0.2.2/prism/cli/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/create_agent.py` & `prism-ds-0.2.2/prism/cli/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/create_task.py` & `prism-ds-0.2.2/prism/cli/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/create_trigger.py` & `prism-ds-0.2.2/prism/cli/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/graph.py` & `prism-ds-0.2.2/prism/cli/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/init.py` & `prism-ds-0.2.2/prism/cli/init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/run.py` & `prism-ds-0.2.2/prism/cli/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/cli/spark_submit.py` & `prism-ds-0.2.2/prism/cli/spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/client/__init__.py` & `prism-ds-0.2.2/prism/client/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/constants.py` & `prism-ds-0.2.2/prism/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #############
 # Constants #
 #############
 
 # Version number
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # Root directory of project
 ROOT_DIR = str(Path(os.path.dirname(__file__)).parent)
 
 # Files to ignore when instantiating Prism project
 IGNORE_FILES = ["__pycache__", '*checkpoint.ipynb', '.ipynb_checkpoints']
 
@@ -31,14 +31,15 @@
     "bigquery",
     "dbt",
     "postgres",
     "pyspark",
     "redshift",
     "snowflake",
     "trino",
+    "presto",
 ]
 
 # Task types
 VALID_TASK_TYPES = [
     "python",
     "pyspark",
 ]
```

### Comparing `prism-ds-0.2.1/prism/decorators/target.py` & `prism-ds-0.2.2/prism/decorators/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/decorators/task.py` & `prism-ds-0.2.2/prism/decorators/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/311ea03002abadcdcaba.png` & `prism-ds-0.2.2/prism/docs/build/311ea03002abadcdcaba.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/54968a39190c43d592b9.svg` & `prism-ds-0.2.2/prism/docs/build/54968a39190c43d592b9.svg`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/737ad70b3f2d3a9b5f6e.ico` & `prism-ds-0.2.2/prism/docs/build/737ad70b3f2d3a9b5f6e.ico`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/ce188596011a8fa32931.png` & `prism-ds-0.2.2/prism/docs/build/ce188596011a8fa32931.png`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/index.html` & `prism-ds-0.2.2/prism/docs/build/index.html`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/docs/build/main.js.LICENSE.txt` & `prism-ds-0.2.2/prism/docs/build/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/event_managers/base.py` & `prism-ds-0.2.2/prism/event_managers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/exceptions.py` & `prism-ds-0.2.2/prism/exceptions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/compiled_task.py` & `prism-ds-0.2.2/prism/infra/compiled_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/compiler.py` & `prism-ds-0.2.2/prism/infra/compiler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/executor.py` & `prism-ds-0.2.2/prism/infra/executor.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/hooks.py` & `prism-ds-0.2.2/prism/infra/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         For SQL adapters, get the database connection:
             - BigQuery --> google.cloud.bigquery.Client
             - Postgres --> psycopg2.Connection
             - Redshift --> psycopg2.Connection
             - Snowflake --> snowflake.connector.Connection
             - Trino --> trino.dbapi.Connection
+            - Presto --> prestodb.dbapi.Connection
 
         args:
             adapter_name: SQL adapter
         returns
             database connection as a class object
         """
         try:
```

### Comparing `prism-ds-0.2.1/prism/infra/manifest.py` & `prism-ds-0.2.2/prism/infra/manifest.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/pipeline.py` & `prism-ds-0.2.2/prism/infra/pipeline.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/project.py` & `prism-ds-0.2.2/prism/infra/project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/sys_path.py` & `prism-ds-0.2.2/prism/infra/sys_path.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/infra/task_manager.py` & `prism-ds-0.2.2/prism/infra/task_manager.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/main.py` & `prism-ds-0.2.2/prism/main.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/agent.py` & `prism-ds-0.2.2/prism/mixins/agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/aws.py` & `prism-ds-0.2.2/prism/mixins/aws.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/base.py` & `prism-ds-0.2.2/prism/mixins/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/compile.py` & `prism-ds-0.2.2/prism/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/connect.py` & `prism-ds-0.2.2/prism/mixins/connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/create_agent.py` & `prism-ds-0.2.2/prism/mixins/create_agent.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/create_task.py` & `prism-ds-0.2.2/prism/mixins/create_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/create_trigger.py` & `prism-ds-0.2.2/prism/mixins/create_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/graph.py` & `prism-ds-0.2.2/prism/mixins/graph.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/run.py` & `prism-ds-0.2.2/prism/mixins/run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/mixins/sys_handler.py` & `prism-ds-0.2.2/prism/mixins/sys_handler.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/parsers/ast_parser.py` & `prism-ds-0.2.2/prism/parsers/ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/parsers/base.py` & `prism-ds-0.2.2/prism/parsers/base.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/parsers/yml_parser.py` & `prism-ds-0.2.2/prism/parsers/yml_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/prism_logging.py` & `prism-ds-0.2.2/prism/prism_logging.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/adapter.py` & `prism-ds-0.2.2/prism/profiles/adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/bigquery.py` & `prism-ds-0.2.2/prism/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/dbt.py` & `prism-ds-0.2.2/prism/profiles/dbt.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/meta.py` & `prism-ds-0.2.2/prism/profiles/meta.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/postgres.py` & `prism-ds-0.2.2/prism/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/profile.py` & `prism-ds-0.2.2/prism/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/pyspark.py` & `prism-ds-0.2.2/prism/profiles/pyspark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/redshift.py` & `prism-ds-0.2.2/prism/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/snowflake.py` & `prism-ds-0.2.2/prism/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/profiles/trino.py` & `prism-ds-0.2.2/prism/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/spark/wrapper.py` & `prism-ds-0.2.2/prism/spark/wrapper.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/target.py` & `prism-ds-0.2.2/prism/target.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/task.py` & `prism-ds-0.2.2/prism/task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/minimal_project/prism_project.py` & `prism-ds-0.2.2/prism/templates/minimal_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/minimal_project/tasks/class_task.py` & `prism-ds-0.2.2/prism/templates/minimal_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/minimal_project/tasks/decorated_task.py` & `prism-ds-0.2.2/prism/templates/minimal_project/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/starter_project/dev/dev.ipynb` & `prism-ds-0.2.2/prism/templates/starter_project/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/starter_project/prism_project.py` & `prism-ds-0.2.2/prism/templates/starter_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/starter_project/tasks/class_task.py` & `prism-ds-0.2.2/prism/templates/starter_project/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/templates/starter_project/tasks/decorated_task.py` & `prism-ds-0.2.2/prism/templates/starter_project/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/integration_test_class.py` & `prism-ds-0.2.2/prism/tests/integration/integration_test_class.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_client.py` & `prism-ds-0.2.2/prism/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_compile.py` & `prism-ds-0.2.2/prism/tests/integration/test_compile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_connect.py` & `prism-ds-0.2.2/prism/tests/integration/test_connect.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_create.py` & `prism-ds-0.2.2/prism/tests/integration/test_create.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_dbt.py` & `prism-ds-0.2.2/prism/tests/integration/test_dbt.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_hooks.py` & `prism-ds-0.2.2/prism/tests/integration/test_hooks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_init.py` & `prism-ds-0.2.2/prism/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/class_task.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001_init/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/tasks/class_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/001a_init_minimal/tasks/decorated_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/functions.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/002_no_project_py/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/003_project_with_cycle/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/004_simple_project/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/004_simple_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_modules/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/functions.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/005_simple_project_no_null_tasks/tasks/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/006_simple_project_with_profile/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/007_spark_project/tasks/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv_iter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/csv_mult.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/008_targets/tasks/parquet.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/008_targets/tasks/parquet.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/009_simple_dbt_project/prism/tasks/filter_customers.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/010_project_nested_module_dirs/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/extract/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/load/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/011_bad_task_ref/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module02.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module02.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module03.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module03.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/modules/module04.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/modules/module04.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/tasks/local_tasks.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/012_concurrency_local/tasks/non_local_task.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/bad_adapter.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/postgres.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/snowflake.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/modules/spark.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/013_hooks_sql_spark/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/014_test_triggers_normal/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/015_test_triggers_no_dir/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/016_test_triggers_error/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/017_test_triggers_extra_key/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/018_test_triggers_no_include/tasks/module01.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/tasks/extract.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/019_dec_targets/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/020_dec_retries/tasks/load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/extract.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/021_project_with_local_tasks/tasks/transform_load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py` & `prism-ds-0.2.2/prism/tests/integration/test_projects/022_project_with_bad_local_tasks/tasks/transform_load.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_run.py` & `prism-ds-0.2.2/prism/tests/integration/test_run.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_spark_submit.py` & `prism-ds-0.2.2/prism/tests/integration/test_spark_submit.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/integration/test_targets.py` & `prism-ds-0.2.2/prism/tests/integration/test_targets.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_adapter_profile.py` & `prism-ds-0.2.2/prism/tests/unit/test_adapter_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_agent/prism_project.py` & `prism-ds-0.2.2/prism/tests/unit/test_agent/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_agents.py` & `prism-ds-0.2.2/prism/tests/unit/test_agents.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_all_dag_fns.py` & `prism-ds-0.2.2/prism/tests/unit/test_all_dag_fns.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_ast_parser.py` & `prism-ds-0.2.2/prism/tests/unit/test_ast_parser.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_jinja.py` & `prism-ds-0.2.2/prism/tests/unit/test_jinja.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/bad_trigger_key.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/bad_trigger_key.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/multiple_profiles.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/multiple_profiles.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/no_profile.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/no_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/non_null_profile.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/non_null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/null_profile.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/null_profile.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/on_failure_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/on_success_triggers_only.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_prism_project_py/triggers_normal.py` & `prism-ds-0.2.2/prism/tests/unit/test_prism_project_py/triggers_normal.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_project.py` & `prism-ds-0.2.2/prism/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_trigger.py` & `prism-ds-0.2.2/prism/tests/unit/test_trigger.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/tests/unit/test_trigger_yml/prism_project.py` & `prism-ds-0.2.2/prism/tests/unit/test_trigger_yml/prism_project.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/triggers/__init__.py` & `prism-ds-0.2.2/prism/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism/ui.py` & `prism-ds-0.2.2/prism/ui.py`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/prism_ds.egg-info/PKG-INFO` & `prism-ds-0.2.2/prism_ds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prism-ds
-Version: 0.2.1
+Version: 0.2.2
 Summary: The easiest way to create data pipelines in Python.
 Author: prism founders
 Author-email: hello@runprism.com
 License: Apache-2.0
 Project-URL: homepage, https://www.runprism.com
 Project-URL: documentation, https://docs.runprism.com
 Project-URL: repository, https://github.com/runprism/prism
@@ -20,14 +20,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: snowflake
 Provides-Extra: bigquery
 Provides-Extra: redshift
 Provides-Extra: postgres
 Provides-Extra: trino
+Provides-Extra: presto
 Provides-Extra: pyspark
 Provides-Extra: dbt
 Provides-Extra: docker
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
@@ -88,14 +89,15 @@
 ### Adapters
 Adapters allow users to connect to data warehouses or analytics engines. Prism currently supports the following adapters:
 | Adapter      | Command |
 | ------------ | ----------- |
 | **dbt** | ```pip install "prism-ds[dbt]"``` |
 | **Google BigQuery** | ```pip install "prism-ds[bigquery]"``` |
 | **Postgres** | ```pip install "prism-ds[postgres]"``` |
+| **Presto** | ```pip install "prism-ds[presto]"``` |
 | **PySpark** | ```pip install "prism-ds[pyspark]"``` |
 | **Redshift** | ```pip install "prism-ds[redshift]"``` |
 | **Snowflake** | ```pip install "prism-ds[snowflake]"``` |
 | **Trino** | ```pip install "prism-ds[trino]"``` |
 
 ### Agents
 Agents allow users to run their projects on external computing environments, e.g., Docker containers, EC2 instances, EMR clusters, and more. Prism currently supports the following agents:
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: prism-ds Version: 0.2.1 Summary: The easiest way to
+Metadata-Version: 2.1 Name: prism-ds Version: 0.2.2 Summary: The easiest way to
 create data pipelines in Python. Author: prism founders Author-email:
 hello@runprism.com License: Apache-2.0 Project-URL: homepage, https://
 www.runprism.com Project-URL: documentation, https://docs.runprism.com Project-
 URL: repository, https://github.com/runprism/prism Platform: unix Platform:
 linux Platform: osx Platform: win32 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: snowflake Provides-
 Extra: bigquery Provides-Extra: redshift Provides-Extra: postgres Provides-
-Extra: trino Provides-Extra: pyspark Provides-Extra: dbt Provides-Extra: docker
-Provides-Extra: testing License-File: LICENSE
+Extra: trino Provides-Extra: presto Provides-Extra: pyspark Provides-Extra: dbt
+Provides-Extra: docker Provides-Extra: testing License-File: LICENSE
                                  [prism logo]
           [PyPI] [https://static.pepy.tech/personalized-badge/prism-
 ds?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
 [![CI Linux](https://github.com/runprism/prism/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-linux.yml)
 [![CI MacOS](https://github.com/runprism/prism/actions/workflows/ci-macos.yml/
 badge.svg)](https://github.com/runprism/prism/actions/workflows/ci-macos.yml)
@@ -49,20 +49,21 @@
 (https://github.com/runprism/prism_examples). ## Integrations Prism integrates
 with a wide variety of third-party developer tools There are two kinds of
 integrations that Prism supports: adapters, and agents. ### Adapters Adapters
 allow users to connect to data warehouses or analytics engines. Prism currently
 supports the following adapters: | Adapter | Command | | ------------ | -------
 ---- | | **dbt** | ```pip install "prism-ds[dbt]"``` | | **Google BigQuery** |
 ```pip install "prism-ds[bigquery]"``` | | **Postgres** | ```pip install
-"prism-ds[postgres]"``` | | **PySpark** | ```pip install "prism-ds[pyspark]"```
-| | **Redshift** | ```pip install "prism-ds[redshift]"``` | | **Snowflake** |
-```pip install "prism-ds[snowflake]"``` | | **Trino** | ```pip install "prism-
-ds[trino]"``` | ### Agents Agents allow users to run their projects on external
-computing environments, e.g., Docker containers, EC2 instances, EMR clusters,
-and more. Prism currently supports the following agents: | Agent | Command | |
------------- | ----------- | | **docker** | ```pip install "prism-ds
-[docker]"``` | | **ec2** | N/A - comes with base Prism | ## Product Roadmap
-We're always looking to improve our product. Here's what we're working on at
-the moment: - **Additional Agents**: EMR clusters, Databricks clusters, and
-more! - **Additional adapters**: Celery, Dask, MySQL, Presto, and more! -
-**Cloud deployment**: Managed orchestration platform to deploy Prism projects
-in the cloud Let us know if you'd like to see another feature!
+"prism-ds[postgres]"``` | | **Presto** | ```pip install "prism-ds[presto]"``` |
+| **PySpark** | ```pip install "prism-ds[pyspark]"``` | | **Redshift** | ```pip
+install "prism-ds[redshift]"``` | | **Snowflake** | ```pip install "prism-ds
+[snowflake]"``` | | **Trino** | ```pip install "prism-ds[trino]"``` | ###
+Agents Agents allow users to run their projects on external computing
+environments, e.g., Docker containers, EC2 instances, EMR clusters, and more.
+Prism currently supports the following agents: | Agent | Command | | ----------
+-- | ----------- | | **docker** | ```pip install "prism-ds[docker]"``` | |
+**ec2** | N/A - comes with base Prism | ## Product Roadmap We're always looking
+to improve our product. Here's what we're working on at the moment: -
+**Additional Agents**: EMR clusters, Databricks clusters, and more! -
+**Additional adapters**: Celery, Dask, MySQL, Presto, and more! - **Cloud
+deployment**: Managed orchestration platform to deploy Prism projects in the
+cloud Let us know if you'd like to see another feature!
```

### Comparing `prism-ds-0.2.1/prism_ds.egg-info/SOURCES.txt` & `prism-ds-0.2.2/prism_ds.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 prism/parsers/yml_parser.py
 prism/profiles/__init__.py
 prism/profiles/adapter.py
 prism/profiles/bigquery.py
 prism/profiles/dbt.py
 prism/profiles/meta.py
 prism/profiles/postgres.py
+prism/profiles/presto.py
 prism/profiles/profile.py
 prism/profiles/pyspark.py
 prism/profiles/redshift.py
 prism/profiles/snowflake.py
 prism/profiles/trino.py
 prism/spark/__init__.py
 prism/spark/script.py
@@ -96,14 +97,15 @@
 prism/templates/minimal_project/prism_project.py
 prism/templates/minimal_project/tasks/class_task.py
 prism/templates/minimal_project/tasks/decorated_task.py
 prism/templates/profile/__init__.py
 prism/templates/profile/bigquery/profile.yml
 prism/templates/profile/dbt/profile.yml
 prism/templates/profile/postgres/profile.yml
+prism/templates/profile/presto/profile.yml
 prism/templates/profile/pyspark/profile.yml
 prism/templates/profile/redshift/profile.yml
 prism/templates/profile/snowflake/profile.yml
 prism/templates/profile/trino/profile.yml
 prism/templates/starter_project/.gitignore
 prism/templates/starter_project/__init__.py
 prism/templates/starter_project/prism_project.py
```

### Comparing `prism-ds-0.2.1/prism_ds.egg-info/requires.txt` & `prism-ds-0.2.2/prism_ds.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 [docker]
 docker>=6.0
 
 [postgres]
 psycopg2-binary>=2.9
 
+[presto]
+presto-python-client>=0.8
+
 [pyspark]
 pyspark>=3
 
 [redshift]
 psycopg2-binary>=2.9
 
 [snowflake]
```

### Comparing `prism-ds-0.2.1/pyproject.toml` & `prism-ds-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prism-ds-0.2.1/setup.cfg` & `prism-ds-0.2.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = prism-ds
 description = The easiest way to create data pipelines in Python.
 long_description_content_type = text/markdown
 long_description = file: README.md
-version = 0.2.1
+version = 0.2.2
 author = prism founders
 author_email = hello@runprism.com
 license = Apache-2.0
 license_files = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
@@ -52,14 +52,16 @@
 	db-dtypes>=1
 redshift = 
 	psycopg2-binary>=2.9
 postgres = 
 	psycopg2-binary>=2.9
 trino = 
 	trino>=0.319
+presto = 
+	presto-python-client>=0.8
 pyspark = 
 	pyspark>=3
 dbt = 
 	dbt-core>=1,<1.6.0
 docker = 
 	docker>=6.0
 testing =
```

