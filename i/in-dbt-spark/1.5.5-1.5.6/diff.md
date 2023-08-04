# Comparing `tmp/in-dbt-spark-1.5.5.tar.gz` & `tmp/in-dbt-spark-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.5.5.tar", last modified: Thu Jul 27 06:32:58 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.5.6.tar", last modified: Fri Aug  4 18:25:53 2023, max compression
```

## Comparing `in-dbt-spark-1.5.5.tar` & `in-dbt-spark-1.5.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.141893 in-dbt-spark-1.5.5/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.141893 in-dbt-spark-1.5.5/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.145892 in-dbt-spark-1.5.5/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.145892 in-dbt-spark-1.5.5/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.141893 in-dbt-spark-1.5.5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.145892 in-dbt-spark-1.5.5/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.145892 in-dbt-spark-1.5.5/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.145892 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 06:32:58.000000 in-dbt-spark-1.5.5/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 06:32:58.149893 in-dbt-spark-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-27 06:32:46.000000 in-dbt-spark-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.050978 in-dbt-spark-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-04 18:25:53.050978 in-dbt-spark-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.042978 in-dbt-spark-1.5.6/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.042978 in-dbt-spark-1.5.6/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.042978 in-dbt-spark-1.5.6/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.046978 in-dbt-spark-1.5.6/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.042978 in-dbt-spark-1.5.6/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.046978 in-dbt-spark-1.5.6/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.046978 in-dbt-spark-1.5.6/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.046978 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.046978 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.050978 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:25:53.050978 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-04 18:25:52.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 18:25:53.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:25:52.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:25:52.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-04 18:25:52.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-04 18:25:52.000000 in-dbt-spark-1.5.6/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 18:25:53.050978 in-dbt-spark-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-04 18:25:41.000000 in-dbt-spark-1.5.6/setup.py
```

### Comparing `in-dbt-spark-1.5.5/PKG-INFO` & `in-dbt-spark-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.5
+Version: 1.5.6
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.5 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.6 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
```

### Comparing `in-dbt-spark-1.5.5/README.md` & `in-dbt-spark-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/client.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/models.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/session.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/session_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import dbt.exceptions
 from dbt.adapters.setu.client import SetuClient
 from dbt.events import AdapterLogger
 from dbt.adapters.setu.constants import VALID_STATEMENT_KINDS
 from dbt.adapters.setu.models import StatementKind, Output, StatementState, Statement
 from dbt.adapters.setu.utils import (
-    get_dataframe_from_json_output,
     polling_intervals,
     waiting_for_output,
     get_data_from_json_output,
 )
 
 logger = AdapterLogger("Spark")
 
@@ -27,20 +26,19 @@
     def __init__(self, client: SetuClient, session_id: str):
         self.session_id: str = session_id
         self.client: SetuClient = client
         self.statement: Optional[Statement] = None
 
     def description(self):
         self.fetchall()
-        pandas_df = get_dataframe_from_json_output(self.statement.output.json)
-        columns = pandas_df.columns
-        data = []
-        for column in columns:
-            data.append([column])
-        return data
+        json_output = self.statement.output.json
+        columns = json_output["schema"]["fields"]
+
+        # Old behavior but with an added index field["type"]
+        return [[column["name"], column["type"]] for column in columns]
 
     def execute(self, code: str) -> Output:
         statement_kind: StatementKind = self.get_statement_kind(code)
         logger.info(f"statement_kind = {statement_kind} ")
         formatted_code: str = self.get_formatted_code(code)
         logger.info(f"formatted_code = {formatted_code} ")
         if statement_kind not in VALID_STATEMENT_KINDS:
```

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.5.6/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/__init__.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/column.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/python_submissions.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/adapters/spark/session.py` & `in-dbt-spark-1.5.6/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/materializations/validate.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.5.6/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.5.6/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.5.6/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.5
+Version: 1.5.6
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.5 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.6 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
```

### Comparing `in-dbt-spark-1.5.5/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.5.6/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.5/setup.py` & `in-dbt-spark-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.5.5"
+package_version = "1.5.6"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
```

