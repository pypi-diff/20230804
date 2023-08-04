# Comparing `tmp/mindsdb_sql-0.6.7.tar.gz` & `tmp/mindsdb_sql-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.7.tar", last modified: Thu Jul 27 14:13:03 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.7.0.tar", last modified: Fri Aug  4 13:19:18 2023, max compression
```

## Comparing `mindsdb_sql-0.6.7.tar` & `mindsdb_sql-0.7.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/
--rw-rw-rw-   0        0        0      535 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      591 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0      503 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/data.py
--rw-rw-rw-   0        0        0     3196 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     3154 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      833 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1595 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8179 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    46322 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
--rw-rw-rw-   0        0        0     2246 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/trigger.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    54291 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21394 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8739 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    13439 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3380 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:13:03.000000 mindsdb_sql-0.6.7/sly/
--rw-rw-rw-   0        0        0      109 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/__init__.py
--rw-rw-rw-   0        0        0      777 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/ast.py
--rw-rw-rw-   0        0        0    16752 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/lex.py
--rw-rw-rw-   0        0        0    89289 2023-07-27 14:12:43.000000 mindsdb_sql-0.6.7/sly/yacc.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/
+-rw-rw-rw-   0        0        0      535 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7227 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      591 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0      503 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/data.py
+-rw-rw-rw-   0        0        0     3196 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     3154 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      833 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8230 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    46345 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+-rw-rw-rw-   0        0        0     2246 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/trigger.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    54291 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21394 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8739 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13439 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20662 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3380 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:19:18.000000 mindsdb_sql-0.7.0/sly/
+-rw-rw-rw-   0        0        0      109 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/sly/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/sly/ast.py
+-rw-rw-rw-   0        0        0    16752 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/sly/lex.py
+-rw-rw-rw-   0        0        0    89289 2023-08-04 13:18:51.000000 mindsdb_sql-0.7.0/sly/yacc.py
```

### Comparing `mindsdb_sql-0.6.7/PKG-INFO` & `mindsdb_sql-0.7.0/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: mindsdb_sql
-Version: 0.6.7
+Name: mindsdb-sql
+Version: 0.7.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.7/README.md` & `mindsdb_sql-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 ## Architecture
 
 Only one renderer is available at the moment: SqlalchemyRender.
 - It converts AST-query to sqlalchemy query. 
 It uses [imperative](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#orm-imperative-mapping) mapping for this 
 - Then created sqlalchemy object is compiled inside sqlalchemy using chosen dialect 
 
-Supported dialects at the moment: mysql, postgresql, sqlite, mssql, firebird, oracle, sybase
+Supported dialects at the moment: mysql, postgresql, sqlite, mssql, oracle
 
 Notes:
 - it is not possible to use more than 2 part in table name
   - it can be (integration.table) or (schema.table)
   - but can't be (integration.schema.table)
 - sometimes conditions in rendered sql can be slightly changed, for example 'not a=b' to 'a!=b'
```

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/__init__.py` & `mindsdb_sql-0.7.0/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         SHOW, SCHEMAS, SCHEMA, DATABASES, DATABASE, TABLES, TABLE, FULL, EXTENDED, PROCESSLIST,
         MUTEX, CODE, SLAVE, REPLICA, REPLICAS, CHANNEL, TRIGGERS, TRIGGER, KEYS, STORAGE, LOGS, BINARY,
         MASTER, PRIVILEGES, PROFILES, HOSTS, OPEN, INDEXES,
         VARIABLES, SESSION, STATUS,
         GLOBAL, PROCEDURE, FUNCTION, INDEX, WARNINGS,
         ENGINES, CHARSET, COLLATION, PLUGINS, CHARACTER,
         PERSIST, PERSIST_ONLY, DEFAULT,
-        IF_EXISTS, COLUMNS, FIELDS, COLLATE,
+        IF_EXISTS, COLUMNS, FIELDS, COLLATE, SEARCH_PATH,
         # SELECT Keywords
         WITH, SELECT, DISTINCT, FROM, WHERE, AS,
         LIMIT, OFFSET, ASC, DESC, NULLS_FIRST, NULLS_LAST,
         GROUP_BY, HAVING, ORDER_BY,
         STAR, FOR, UPDATE,
 
         JOIN, INNER, OUTER, CROSS, LEFT, RIGHT, ON,
@@ -178,14 +178,15 @@
     PRIVILEGES = r'\bPRIVILEGES\b'
     PROFILES = r'\bPROFILES\b'
     HOSTS = r'\bHOSTS\b'
     OPEN = r'\bOPEN\b'
     INDEXES = r'\bINDEXES\b'
     REPLACE = r'\bREPLACE\b'
     COLLATE = r'\bCOLLATE\b'
+    SEARCH_PATH = r'\bSEARCH_PATH\b'
 
     # SELECT
 
     ON = r'\bON\b'
     ASC = r'\bASC\b'
     DESC = r'\bDESC\b'
     NULLS_FIRST = r'\bNULLS FIRST\b'
```

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,14 +449,15 @@
        'INTEGRATIONS',
        'DATASOURCES',
        'PUBLICATIONS',
        'DATASETS',
        'MODELS',
        'ML_ENGINES',
        'HANDLERS',
+       'SEARCH_PATH',
        'ALL')
     def show_category(self, p):
         return ' '.join([x for x in p])
 
     # custom show commands
     @_('SHOW ENGINE identifier STATUS',
        'SHOW ENGINE identifier MUTEX')
```

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mindsdb/trigger.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mindsdb/trigger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.7.0/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/query_planner.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/steps.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.7.0/mindsdb_sql/planner/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.7.0/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import datetime as dt
 
 import sqlalchemy as sa
 from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.orm.query import aliased
-from sqlalchemy.dialects import mysql, postgresql, sqlite, mssql, firebird, oracle, sybase
+from sqlalchemy.orm import aliased
+from sqlalchemy.dialects import mysql, postgresql, sqlite, mssql, oracle
 from sqlalchemy.schema import CreateTable, DropTable
 
 from mindsdb_sql.parser import ast
 
 
+sa_type_names = [
+    key for key, val in sa.types.__dict__.items() if hasattr(val, '__module__')
+    and val.__module__ in ('sqlalchemy.sql.sqltypes', 'sqlalchemy.sql.type_api')
+]
+
+
 class RenderError(Exception):
     ...
 
 
 class SqlalchemyRender:
 
     def __init__(self, dialect_name):
         dialects = {
             'mysql': mysql,
             'postgresql': postgresql,
             'postgres': postgresql,
             'sqlite': sqlite,
             'mssql': mssql,
-            'firebird': firebird,
             'oracle': oracle,
-            'sybase': sybase,
             'Snowflake': oracle,
         }
 
         if isinstance(dialect_name, str):
             dialect = dialects[dialect_name].dialect
         else:
             dialect = dialect_name
@@ -42,15 +46,15 @@
             self.dialect.server_version_info = (10,)
             self.dialect._setup_version_attributes()
         elif dialect_name == 'mysql':
             # update version for support float cast
             self.dialect.server_version_info = (8, 0, 17)
 
         self.types_map = {}
-        for type_name in sa.types.__all__:
+        for type_name in sa_type_names:
             self.types_map[type_name.upper()] = getattr(sa.types, type_name)
 
     def to_column(self, parts):
         # because sqlalchemy doesn't allow columns consist from parts therefore we do it manually
 
         parts2 = []
 
@@ -125,15 +129,15 @@
             else:
                 alias = str(t.op)
             col = col.label(alias)
         elif isinstance(t, ast.BinaryOperation):
             methods = {
                 "+": "__add__",
                 "-": "__sub__",
-                "/": "__div__",
+                "/": "__truediv__",
                 "*": "__mul__",
                 "%": "__mod__",
                 "=": "__eq__",
                 "!=": "__ne__",
                 ">": "__gt__",
                 "<": "__lt__",
                 ">=": "__ge__",
@@ -326,15 +330,15 @@
     def prepare_select(self, node):
 
         cols = []
         for t in node.targets:
             col = self.to_expression(t)
             cols.append(col)
 
-        query = sa.select(cols)
+        query = sa.select(*cols)
 
         if node.cte is not None:
             for cte in node.cte:
                 if cte.columns is not None and len(cte.columns) > 0:
                     raise NotImplementedError('CTE columns')
 
                 stmt = self.prepare_select(cte.query)
```

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: mindsdb-sql
-Version: 0.6.7
+Name: mindsdb_sql
+Version: 0.7.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.7/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.7.0/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/setup.py` & `mindsdb_sql-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/sly/ast.py` & `mindsdb_sql-0.7.0/sly/ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/sly/lex.py` & `mindsdb_sql-0.7.0/sly/lex.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.7/sly/yacc.py` & `mindsdb_sql-0.7.0/sly/yacc.py`

 * *Files identical despite different names*

