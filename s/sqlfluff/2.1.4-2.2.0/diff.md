# Comparing `tmp/sqlfluff-2.1.4.tar.gz` & `tmp/sqlfluff-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-fzrqvhpn/sqlfluff-2.1.4.tar", last modified: Tue Jul 25 10:29:09 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-5v3w3hqn/sqlfluff-2.2.0.tar", last modified: Fri Aug  4 16:59:24 2023, max compression
```

## Comparing `sqlfluff-2.1.4.tar` & `sqlfluff-2.2.0.tar`

### file list

```diff
@@ -1,258 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)   397137 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    46018 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    45351 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    51152 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    42757 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19891 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74094 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   135036 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    22693 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68578 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    94477 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    81269 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   165929 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36674 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   202161 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   101470 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   178244 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:29:09.000000 sqlfluff-2.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-25 10:28:50.000000 sqlfluff-2.1.4/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   404917 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49618 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45081 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41836 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34855 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72059 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62745 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25117 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45777 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135469 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22693 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68578 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33819 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94477 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81899 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165929 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36794 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72597 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202309 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101524 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178244 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20397 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31729 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93553 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25461 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 16:59:23.000000 sqlfluff-2.2.0/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:59:24.000000 sqlfluff-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-04 16:59:05.000000 sqlfluff-2.2.0/test/test_testing.py
```

### Comparing `sqlfluff-2.1.4/CHANGELOG.md` & `sqlfluff-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,100 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.2.0] - 2023-08-04
+
+## Highlights
+
+This release changes some of the interfaces between SQLFluff core and
+our plugin ecosystem. The only *breaking* change is in the interface
+between SQLFluff and *templater* plugins (which are not common in the
+ecosystem, hence why this is only a minor and not a major release).
+
+For all plugins, we also recommend a different structure for their
+imports (especially for rule plugins which are more common in the
+ecosystem) - for performance and stability reasons. Some users had
+been experiencing very long import times with previous releases as
+a result of the layout of plugin imports. Users with affected plugins
+will begin to see a warning from this release onward, which can be
+resolved for their plugin by updating to a new version of that plugin
+which follows the guidelines.
+
+For more details (especially if you're a plugin maintainer) see our
+[release notes](https://docs.sqlfluff.com/en/latest/releasenotes.html).
+
+Additionally this release includes:
+- Some internal performance gains which may cumulatively save
+  roughly 10% of the time spent in the parsing phase of larger files.
+- Improvements to the Simple API, including the ability to pass in
+  a `FluffConfig` object directly, and better support for parsing
+  config files directly from strings (see
+  [the included example](examples/05_simple_api_config.py)).
+- A bugfix for `AM06`.
+- A new `--warn-unused-ignores` CLI option (and corresponding config
+  setting) to allow warnings to be shown if any `noqa` comments in
+  SQL files are unused.
+- Improvements to Redshift, Oracle, Clickhouse, Materialize &
+  MySQL dialects.
+- A selection of internal improvements, documentation and type hints.
+
+Thanks also to [@kaiyannameighu](https://github.com/kaiyannameighu),
+[@josef-v](https://github.com/josef-v),
+[@aglebov](https://github.com/aglebov) &
+[@joaostorrer](https://github.com/joaostorrer) who made their first
+contributions as part of this release! 🎉🎉🎉
+
+## What’s Changed
+
+* Mypy: Ephemeral + Tuple Return on .parse() [#5044](https://github.com/sqlfluff/sqlfluff/pull/5044) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Add support to oracle's global and private temporary tables [#5039](https://github.com/sqlfluff/sqlfluff/pull/5039) [@joaostorrer](https://github.com/joaostorrer)
+* Redshift-dialect: Support GRANT USAGE ON DATASHARE [#5007](https://github.com/sqlfluff/sqlfluff/pull/5007) [@josef-v](https://github.com/josef-v)
+* :white_check_mark: Add strict typing for errors module [#5047](https://github.com/sqlfluff/sqlfluff/pull/5047) [@pwildenhain](https://github.com/pwildenhain)
+* Less copying in the ParseContext [#5046](https://github.com/sqlfluff/sqlfluff/pull/5046) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Adding support to use `ADD COLUMN IF NOT EXISTS` syntax on `ALTER TABLE` [#5035](https://github.com/sqlfluff/sqlfluff/pull/5035) [@wfelipew](https://github.com/wfelipew)
+* Closes #4815 [#5042](https://github.com/sqlfluff/sqlfluff/pull/5042) [@joaostorrer](https://github.com/joaostorrer)
+* Fix for multiprocessing warnings. [#5032](https://github.com/sqlfluff/sqlfluff/pull/5032) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Mypy gain: Remove unnecessary tuple construction in MatchResult [#5045](https://github.com/sqlfluff/sqlfluff/pull/5045) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* mypy strict in config [#5036](https://github.com/sqlfluff/sqlfluff/pull/5036) [@pwildenhain](https://github.com/pwildenhain)
+* strict mypy: match_wrapper & match_logging [#5033](https://github.com/sqlfluff/sqlfluff/pull/5033) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* MyPy on errors, helpers, markers & context + remove ParseContext.denylist [#5030](https://github.com/sqlfluff/sqlfluff/pull/5030) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Warn on unused `noqa` directives [#5029](https://github.com/sqlfluff/sqlfluff/pull/5029) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Even more mypy strict [#5023](https://github.com/sqlfluff/sqlfluff/pull/5023) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Handle windows paths better in config files. [#5022](https://github.com/sqlfluff/sqlfluff/pull/5022) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix for parsing of Oracle functions with named arguments [#5027](https://github.com/sqlfluff/sqlfluff/pull/5027) [@joaostorrer](https://github.com/joaostorrer)
+* DOC: Fix .sqlfluff example in Getting Started [#5026](https://github.com/sqlfluff/sqlfluff/pull/5026) [@aglebov](https://github.com/aglebov)
+* Fix: Add exception to the warning & config for the BaseRule. [#5025](https://github.com/sqlfluff/sqlfluff/pull/5025) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Move from `make_template` to `render_func` in jinja and dbt [#4942](https://github.com/sqlfluff/sqlfluff/pull/4942) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Streamline imports to reduce initial load times #4917 [#5020](https://github.com/sqlfluff/sqlfluff/pull/5020) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* More mypy strict [#5019](https://github.com/sqlfluff/sqlfluff/pull/5019) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Simple API config and examples [#5018](https://github.com/sqlfluff/sqlfluff/pull/5018) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Fix some new linting issues [#5021](https://github.com/sqlfluff/sqlfluff/pull/5021) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* A step towards mypy strict [#5014](https://github.com/sqlfluff/sqlfluff/pull/5014) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Materialize: Make RETURNING a reserved keyword [#5017](https://github.com/sqlfluff/sqlfluff/pull/5017) [@bobbyiliev](https://github.com/bobbyiliev)
+* Config from string and load default_config as resource [#5012](https://github.com/sqlfluff/sqlfluff/pull/5012) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Documentation for the test suite (#2180) [#5011](https://github.com/sqlfluff/sqlfluff/pull/5011) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Add support to oracle's listagg function [#4999](https://github.com/sqlfluff/sqlfluff/pull/4999) [@joaostorrer](https://github.com/joaostorrer)
+* Assorted typehints [#5013](https://github.com/sqlfluff/sqlfluff/pull/5013) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Refactor: Extract noqa methods and tests. [#5010](https://github.com/sqlfluff/sqlfluff/pull/5010) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* AM06 to ignore aggregate ORDER BY clauses [#5008](https://github.com/sqlfluff/sqlfluff/pull/5008) [@tunetheweb](https://github.com/tunetheweb)
+* Bugfix: Treat Function name properly in grants [#5006](https://github.com/sqlfluff/sqlfluff/pull/5006) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Redshift: Add Qualify Clause [#5002](https://github.com/sqlfluff/sqlfluff/pull/5002) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Clickhouse Dialect - Support Dollar Quoted Literals [#5003](https://github.com/sqlfluff/sqlfluff/pull/5003) [@kaiyannameighu](https://github.com/kaiyannameighu)
+
+
+## New Contributors
+* [@kaiyannameighu](https://github.com/kaiyannameighu) made their first contribution in [#5003](https://github.com/sqlfluff/sqlfluff/pull/5003)
+* [@joaostorrer](https://github.com/joaostorrer) made their first contribution in [#4999](https://github.com/sqlfluff/sqlfluff/pull/4999)
+* [@aglebov](https://github.com/aglebov) made their first contribution in [#5026](https://github.com/sqlfluff/sqlfluff/pull/5026)
+* [@josef-v](https://github.com/josef-v) made their first contribution in [#5007](https://github.com/sqlfluff/sqlfluff/pull/5007)
+
 ## [2.1.4] - 2023-07-25
 
 ## Highlights
 
 This release brings some meaningful performance improvements to the parsing of
 complex SQL statements. In files with deeply nested expressions, we have seen
 up to a 50% reduction on time spent in the parsing phase. These changes are all
```

### Comparing `sqlfluff-2.1.4/LICENSE.md` & `sqlfluff-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/PKG-INFO` & `sqlfluff-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.4
+Version: 2.2.0
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.4/README.md` & `sqlfluff-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/setup.cfg` & `sqlfluff-2.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.1.4
+version = 2.2.0
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -72,14 +72,15 @@
 	appdirs
 	backports.cached-property; python_version < '3.8'
 	chardet
 	click
 	colorama>=0.3
 	diff-cover>=2.5.0
 	importlib_metadata>=1.0.0; python_version < '3.8'
+	importlib_resources; python_version < '3.9'
 	Jinja2
 	pathspec
 	pytest
 	pyyaml>=5.1
 	regex
 	tblib
 	toml; python_version < '3.11'
@@ -110,13 +111,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.1.4
+stable_version = 2.2.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/api/simple.py` & `sqlfluff-2.2.0/src/sqlfluff/api/simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,33 +57,37 @@
 
 
 def lint(
     sql: str,
     dialect: str = "ansi",
     rules: Optional[List[str]] = None,
     exclude_rules: Optional[List[str]] = None,
+    config: Optional[FluffConfig] = None,
     config_path: Optional[str] = None,
 ) -> List[Dict[str, Any]]:
     """Lint a SQL string.
 
     Args:
         sql (:obj:`str`): The SQL to be linted.
         dialect (:obj:`str`, optional): A reference to the dialect of the SQL
             to be linted. Defaults to `ansi`.
         rules (:obj:`Optional[List[str]`, optional): A list of rule
             references to lint for. Defaults to None.
         exclude_rules (:obj:`Optional[List[str]`, optional): A list of rule
             references to avoid linting for. Defaults to None.
-        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config.
+        config (:obj:`Optional[FluffConfig]`, optional): A configuration object
+            to use for the operation. Defaults to None.
+        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config,
+            which is only used if a `config` is not already provided.
             Defaults to None.
 
     Returns:
         :obj:`List[Dict[str, Any]]` for each violation found.
     """
-    cfg = get_simple_config(
+    cfg = config or get_simple_config(
         dialect=dialect,
         rules=rules,
         exclude_rules=exclude_rules,
         config_path=config_path,
     )
     linter = Linter(config=cfg)
 
@@ -94,34 +98,38 @@
 
 
 def fix(
     sql: str,
     dialect: str = "ansi",
     rules: Optional[List[str]] = None,
     exclude_rules: Optional[List[str]] = None,
+    config: Optional[FluffConfig] = None,
     config_path: Optional[str] = None,
     fix_even_unparsable: Optional[bool] = None,
 ) -> str:
     """Fix a SQL string.
 
     Args:
         sql (:obj:`str`): The SQL to be fixed.
         dialect (:obj:`str`, optional): A reference to the dialect of the SQL
             to be fixed. Defaults to `ansi`.
         rules (:obj:`Optional[List[str]`, optional): A subset of rule
             references to fix for. Defaults to None.
         exclude_rules (:obj:`Optional[List[str]`, optional): A subset of rule
             references to avoid fixing for. Defaults to None.
-        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config.
+        config (:obj:`Optional[FluffConfig]`, optional): A configuration object
+            to use for the operation. Defaults to None.
+        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config,
+            which is only used if a `config` is not already provided.
             Defaults to None.
 
     Returns:
         :obj:`str` for the fixed SQL if possible.
     """
-    cfg = get_simple_config(
+    cfg = config or get_simple_config(
         dialect=dialect,
         rules=rules,
         exclude_rules=exclude_rules,
         config_path=config_path,
     )
     linter = Linter(config=cfg)
 
@@ -139,35 +147,41 @@
         sql = result.paths[0].files[0].fix_string()[0]
     return sql
 
 
 def parse(
     sql: str,
     dialect: str = "ansi",
+    config: Optional[FluffConfig] = None,
     config_path: Optional[str] = None,
 ) -> Dict[str, Any]:
     """Parse a SQL string.
 
     Args:
         sql (:obj:`str`): The SQL to be parsed.
         dialect (:obj:`str`, optional): A reference to the dialect of the SQL
             to be parsed. Defaults to `ansi`.
-        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config.
+        config (:obj:`Optional[FluffConfig]`, optional): A configuration object
+            to use for the operation. Defaults to None.
+        config_path (:obj:`Optional[str]`, optional): A path to a .sqlfluff config,
+            which is only used if a `config` is not already provided.
             Defaults to None.
 
     Returns:
         :obj:`Dict[str, Any]` JSON containing the parsed structure.
     """
-    cfg = get_simple_config(
+    cfg = config or get_simple_config(
         dialect=dialect,
         config_path=config_path,
     )
     linter = Linter(config=cfg)
 
     parsed = linter.parse_string(sql)
     # If we encounter any parsing errors, raise them in a combined issue.
     if parsed.violations:
         raise APIParsingError(parsed.violations)
     # Return a JSON representation of the parse tree.
     if parsed.tree is None:  # pragma: no cover
         return {}
-    return parsed.tree.as_record(show_raw=True)
+    record = parsed.tree.as_record(show_raw=True)
+    assert record
+    return record
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/autocomplete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """autocompletion commands."""
 
 from sqlfluff import list_dialects
+from typing import List
 
 # Older versions of click don't have shell completion
 # so handle for now, as version 8 still fairly recent
 # See: https://github.com/sqlfluff/sqlfluff/issues/2543
 shell_completion_enabled = True
 try:
     from click import shell_completion as completion
 except ImportError:  # pragma: no cover
     shell_completion_enabled = False
 
 
-def dialect_shell_complete(ctx, param, incomplete):
+def dialect_shell_complete(ctx, param, incomplete) -> List[completion.CompletionItem]:
     """Shell completion for possible dialect names.
 
     We use this over click.Choice as we want to internally
     handle error messages and codes for incorrect/outdated dialects.
     """
     dialect_names = [e.label for e in list_dialects()]
     return [
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     The parser code is unlikely to undergo significant revisions.
 
     Hopefully will be removed when
       * https://github.com/pallets/click/issues/2263
     is finished.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         self.deprecated = kwargs.pop("deprecated", ())
         self.preferred = args[0][-1]
 
         super().__init__(*args, **kwargs)
 
 
 class DeprecatedOptionsCommand(click.Command):
@@ -88,14 +88,15 @@
 
             frame = inspect.currentframe()
             try:
                 opt = frame.f_back.f_locals.get("opt")  # type: ignore
             finally:
                 del frame
 
+            assert deprecated
             if opt in deprecated:
                 msg = (
                     f"DeprecationWarning: The option {opt!r} is deprecated, "
                     f"use {preferred!r}."
                 )
                 echo(style(msg, fg="red"), err=True)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/commands.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from itertools import chain
 import os
 import sys
 import json
 import logging
 import time
 from logging import LogRecord
-from typing import Callable, Tuple, Optional, cast
+from typing import Callable, Tuple, Optional
 
 import yaml
 
 import click
 
 # For the profiler
 import pstats
@@ -27,15 +27,15 @@
     DeprecatedOption,
     DeprecatedOptionsCommand,
 )
 from sqlfluff.cli.formatters import (
     format_linting_result_header,
     OutputStreamFormatter,
 )
-from sqlfluff.cli.helpers import get_package_version
+from sqlfluff.cli.helpers import get_package_version, LazySequence
 from sqlfluff.cli.outputstream import make_output_stream, OutputStream
 
 # Import from sqlfluff core.
 from sqlfluff.core import (
     Linter,
     FluffConfig,
     SQLLintError,
@@ -134,21 +134,21 @@
         fluff_logger.setLevel(logging.DEBUG)
         parser_logger.setLevel(logging.DEBUG)
 
 
 class PathAndUserErrorHandler:
     """Make an API call but with error handling for the CLI."""
 
-    def __init__(self, formatter):
+    def __init__(self, formatter) -> None:
         self.formatter = formatter
 
-    def __enter__(self):
+    def __enter__(self) -> "PathAndUserErrorHandler":
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         if exc_type is SQLFluffUserError:
             click.echo(
                 "\nUser Error: "
                 + self.formatter.colorize(
                     str(exc_val),
                     Color.red,
                 )
@@ -209,20 +209,23 @@
         )(f)
     f = click.option(
         "-t",
         "--templater",
         default=None,
         help="The templater to use (default=jinja)",
         type=click.Choice(
-            [
-                templater.name
-                for templater in chain.from_iterable(
-                    get_plugin_manager().hook.get_templaters()
-                )
-            ]
+            # Use LazySequence so that we don't load templaters until required.
+            LazySequence(
+                lambda: [
+                    templater.name
+                    for templater in chain.from_iterable(
+                        get_plugin_manager().hook.get_templaters()
+                    )
+                ]
+            )
         ),
     )(f)
     f = click.option(
         "-r",
         "--rules",
         default=None,
         help=(
@@ -352,14 +355,20 @@
         help=(
             "A filename to persist the timing information for a linting run to "
             "in csv format for external analysis. NOTE: This feature should be "
             "treated as beta, and the format of the csv file may change in "
             "future releases without warning."
         ),
     )(f)
+    f = click.option(
+        "--warn-unused-ignores",
+        is_flag=True,
+        default=False,
+        help="Warn about unneeded '-- noqa:' comments.",
+    )(f)
     return f
 
 
 def get_config(
     extra_config_path: Optional[str] = None,
     ignore_local_config: bool = False,
     **kwargs,
@@ -385,18 +394,26 @@
                 OutputStreamFormatter.colorize_helper(
                     plain_output,
                     f"Error: Unknown dialect '{kwargs['dialect']}'",
                     color=Color.red,
                 )
             )
             sys.exit(EXIT_ERROR)
+
     from_root_kwargs = {}
     if "require_dialect" in kwargs:
         from_root_kwargs["require_dialect"] = kwargs.pop("require_dialect")
+
     library_path = kwargs.pop("library_path", None)
+
+    if not kwargs.get("warn_unused_ignores", True):
+        # If it's present AND True, then keep it, otherwise remove this so
+        # that we default to the root config.
+        del kwargs["warn_unused_ignores"]
+
     # Instantiate a config object (filtering out the nulls)
     overrides = {k: kwargs[k] for k in kwargs if kwargs[k] is not None}
     if library_path is not None:
         # Check for a null value
         if library_path.lower() == "none":
             library_path = None  # Set an explicit None value.
         # Set the global override
@@ -447,15 +464,15 @@
   sqlfluff lint --dialect postgres .\n
   sqlfluff lint --dialect postgres --rules ST05 .\n
   sqlfluff fix --dialect sqlite --rules LT10,ST05 src/queries\n
   sqlfluff parse --dialect sqlite --templater jinja src/queries/common.sql
 """,
 )
 @click.version_option()
-def cli():
+def cli() -> None:
     """SQLFluff is a modular SQL linter for humans."""  # noqa D403
 
 
 @cli.command()
 @common_options
 def version(**kwargs) -> None:
     """Show the version of sqlfluff."""
@@ -497,15 +514,15 @@
 def dialects(**kwargs) -> None:
     """Show the current dialects available."""
     c = get_config(**kwargs, require_dialect=False)
     _, formatter = get_linter_and_formatter(c)
     click.echo(formatter.format_dialects(dialect_readout), color=c.get("color"))
 
 
-def dump_file_payload(filename: Optional[str], payload: str):
+def dump_file_payload(filename: Optional[str], payload: str) -> None:
     """Write the output file content to stdout or file."""
     # If there's a file specified to write to, write to it.
     if filename:
         with open(filename, "w") as out_file:
             out_file.write(payload)
     # Otherwise write to stdout
     else:
@@ -681,15 +698,15 @@
                     line += f" [{violation['name']}]"
 
                 github_result_native.append(line)
 
         file_output = "\n".join(github_result_native)
 
     if file_output:
-        dump_file_payload(write_output, cast(str, file_output))
+        dump_file_payload(write_output, file_output)
 
     if persist_timing:
         result.persist_timing_records(persist_timing)
 
     output_stream.close()
     if bench:
         click.echo("==== overall timings ====")
@@ -709,15 +726,15 @@
         sys.exit(EXIT_SUCCESS)
 
 
 def do_fixes(
     result: LintingResult,
     formatter: Optional[OutputStreamFormatter] = None,
     fixed_file_suffix: str = "",
-):
+) -> bool:
     """Actually do the fixes."""
     if formatter and formatter.verbosity >= 0:
         click.echo("Persisting Changes...")
     res = result.persist_changes(
         formatter=formatter, fixed_file_suffix=fixed_file_suffix
     )
     if all(res.values()):
@@ -730,15 +747,15 @@
     )  # pragma: no cover
     click.echo(
         "Some errors cannot be fixed or there is another error blocking it."
     )  # pragma: no cover
     return False  # pragma: no cover
 
 
-def _stdin_fix(linter: Linter, formatter, fix_even_unparsable):
+def _stdin_fix(linter: Linter, formatter, fix_even_unparsable: bool) -> None:
     """Handle fixing from stdin."""
     exit_code = EXIT_SUCCESS
     stdin = sys.stdin.read()
 
     result = linter.lint_string_wrapped(stdin, fname="stdin", fix=True)
     templater_error = result.num_violations(types=SQLTemplaterError) > 0
     unfixable_error = result.num_violations(types=SQLLintError, fixable=False) > 0
@@ -784,15 +801,15 @@
     fix_even_unparsable,
     force,
     fixed_suffix,
     bench,
     show_lint_violations,
     warn_force: bool = True,
     persist_timing: Optional[str] = None,
-):
+) -> None:
     """Handle fixing from paths."""
     # Lint the paths (not with the fix argument at this stage), outputting as we go.
     if formatter.verbosity >= 0:
         click.echo("==== finding fixable violations ====")
     exit_code = EXIT_SUCCESS
 
     if force and warn_force and formatter.verbosity >= 0:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             str_buff = token
     # If we have left over buff, add it in
     if str_buff:
         line_buff.append(str_buff)
     return line_buff
 
 
-def format_linting_result_header():
+def format_linting_result_header() -> str:
     """Format the header of a linting result output."""
     text_buffer = StringIO()
     text_buffer.write("==== readout ====\n")
     return text_buffer.getvalue()
 
 
 class OutputStreamFormatter:
@@ -143,15 +143,15 @@
                 text_buffer.write(self.format_config_vals(linter.config.iter_vals()))
         return text_buffer.getvalue()
 
     def dispatch_config(self, linter: Linter) -> None:
         """Dispatch configuration output appropriately."""
         self._dispatch(self._format_config(linter))
 
-    def dispatch_persist_filename(self, filename, result):
+    def dispatch_persist_filename(self, filename: str, result: str) -> None:
         """Dispatch filenames during a persist operation."""
         # Only show the skip records at higher levels of verbosity
         if self.verbosity >= 2 or result != "SKIP":
             self._dispatch(self.format_filename(filename=filename, success=result))
 
     def _format_path(self, path: str) -> str:
         """Format paths."""
@@ -190,15 +190,15 @@
         if self.verbosity > 1:
             self._dispatch(
                 self.format_filename(
                     filename=fname, success=f"LINTING ({', '.join(rules)})"
                 )
             )
 
-    def dispatch_compilation_header(self, templater, message):
+    def dispatch_compilation_header(self, templater: str, message: str) -> None:
         """Dispatch the header displayed before linting."""
         self._dispatch(
             f"=== [{self.colorize(templater, Color.lightgrey)}] {message}"
         )  # pragma: no cover
 
     def dispatch_processing_header(self, processes: int) -> None:
         """Dispatch the header displayed before linting."""
@@ -246,23 +246,29 @@
         str_buffer = text_buffer.getvalue()
         # Remove the trailing newline if there is one
         if len(str_buffer) > 0 and str_buffer[-1] == "\n":
             str_buffer = str_buffer[:-1]
         return str_buffer
 
     def dispatch_file_violations(
-        self, fname: str, linted_file: LintedFile, only_fixable: bool
+        self,
+        fname: str,
+        linted_file: LintedFile,
+        only_fixable: bool,
+        warn_unused_ignores: bool,
     ) -> None:
         """Dispatch any violations found in a file."""
         if self.verbosity < 0:
             return
         s = self._format_file_violations(
             fname,
             linted_file.get_violations(
-                fixable=True if only_fixable else None, filter_warning=False
+                fixable=True if only_fixable else None,
+                filter_warning=False,
+                warn_unused_ignores=warn_unused_ignores,
             ),
         )
         self._dispatch(s)
 
     def colorize(self, s: str, color: Optional[Color] = None) -> str:
         """Optionally use ANSI colour codes to colour a string."""
         return self.colorize_helper(self.plain_output, s, color)
@@ -454,15 +460,15 @@
                         "| ",
                         section_color,
                     )
                 )
             out_buff += line
         return out_buff
 
-    def format_linting_stats(self, result, verbose=0):
+    def format_linting_stats(self, result, verbose=0) -> str:
         """Format a set of stats given a `LintingResult`."""
         text_buffer = StringIO()
         all_stats = result.stats()
         text_buffer.write("==== summary ====\n")
         if verbose >= 2:
             output_fields = [
                 "files",
@@ -487,15 +493,15 @@
             )
             for key in output_fields
         ]
         # Render it all as a table
         text_buffer.write(self.cli_table(summary_content, max_label_width=14))
         return text_buffer.getvalue()
 
-    def format_config_vals(self, config_vals):
+    def format_config_vals(self, config_vals) -> str:
         """Format an iterable of config values from a config object."""
         text_buffer = StringIO()
         for i, k, v in config_vals:
             val = "" if v is None else str(v)
             text_buffer.write(
                 ("    " * i)
                 + self.colorize(
@@ -542,15 +548,15 @@
                 cols=1,
                 label_color=Color.blue,
                 val_align="left",
             )
         )
         return text_buffer.getvalue()
 
-    def format_dialects(self, dialect_readout, verbose=0):
+    def format_dialects(self, dialect_readout, verbose=0) -> str:
         """Format the dialects yielded by `dialect_readout`."""
         text_buffer = StringIO()
         text_buffer.write("==== sqlfluff - dialects ====\n")
         readouts = [
             (
                 dialect.label,
                 f"{dialect.name} dialect [inherits from '{dialect.inherits_from}']",
@@ -564,15 +570,15 @@
                 cols=1,
                 label_color=Color.blue,
                 val_align="right",
             )
         )
         return text_buffer.getvalue()
 
-    def format_dialect_warning(self, dialect):
+    def format_dialect_warning(self, dialect) -> str:
         """Output a warning for parsing errors."""
         return self.colorize(
             (
                 "WARNING: Parsing errors found and dialect is set to "
                 f"'{dialect}'. Have you configured your dialect correctly?"
             ),
             Color.lightgrey,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """CLI helper utilities."""
 
 import sys
 import textwrap
-from typing import Dict, List
+from typing import Callable, List, Dict, Any
+from collections import abc
 
 from sqlfluff import __version__ as pkg_version
+from sqlfluff.core.cached_property import cached_property
 
 
 def get_python_version() -> str:
     """Get the current python version as a string."""
     return "{0[0]}.{0[1]}.{0[2]}".format(sys.version_info)
 
 
@@ -28,15 +30,15 @@
 def wrap_elem(s: str, width: int) -> List[str]:
     """Wrap a string into a list of strings all less than <width>."""
     return textwrap.wrap(s, width=width)
 
 
 def wrap_field(
     label: str, val: str, width: int, max_label_width: int = 10, sep_char: str = ": "
-) -> Dict:
+) -> Dict[str, Any]:
     """Wrap a field (label, val).
 
     Returns:
         A dict of {label_list, val_list, sep_char, lines}
 
     """
     if len(label) > max_label_width:
@@ -68,7 +70,29 @@
         return s
     elif align == "left":
         return s + (" " * gap)
     elif align == "right":
         return (" " * gap) + s
     else:
         raise ValueError(f"Unknown alignment: {align}")  # pragma: no cover
+
+
+class LazySequence(abc.Sequence):
+    """A Sequence which only populates on the first access.
+
+    This is useful for being able to define sequences within
+    the click cli decorators, but that don't trigger their
+    contents until first called.
+    """
+
+    def __init__(self, getter=Callable[[], abc.Sequence]):
+        self._getter = getter
+
+    @cached_property
+    def _sequence(self) -> abc.Sequence:
+        return self._getter()
+
+    def __getitem__(self, key):
+        return self._sequence[key]
+
+    def __len__(self):
+        return len(self._sequence)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.2.0/src/sqlfluff/cli/outputstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,55 +9,55 @@
 from sqlfluff.core import FluffConfig
 from sqlfluff.core.enums import FormatType
 
 
 class OutputStream(abc.ABC):
     """Base class for linter output stream."""
 
-    def __init__(self, config: FluffConfig, context: Any = None):
+    def __init__(self, config: FluffConfig, context: Any = None) -> None:
         self.config = config
 
     def write(self, message: str) -> None:
         """Write message to output."""
         raise NotImplementedError  # pragma: no cover
 
-    def close(self):
+    def close(self) -> None:
         """Close output stream."""
         pass
 
 
 class TqdmOutput(OutputStream):
     """Outputs to stdout, coordinates to avoid conflict with tqdm.
 
     It may happen that progressbar conflicts with extra printing. Nothing very
     serious happens then, except that there is printed (not removed) progressbar
     line. The `external_write_mode` allows to disable tqdm for writing time.
     """
 
-    def __init__(self, config: FluffConfig):
+    def __init__(self, config: FluffConfig) -> None:
         super().__init__(config)
 
     def write(self, message: str) -> None:
         """Write message to stdout."""
         with tqdm.external_write_mode():
             click.echo(message=message, color=self.config.get("color"))
 
 
 class FileOutput(OutputStream):
     """Outputs to a specified file."""
 
-    def __init__(self, config: FluffConfig, output_path: str):
+    def __init__(self, config: FluffConfig, output_path: str) -> None:
         super().__init__(config)
         self.file = open(output_path, "w")
 
     def write(self, message: str) -> None:
         """Write message to output_path."""
         print(message, file=self.file)
 
-    def close(self):
+    def close(self) -> None:
         """Close output file."""
         self.file.close()
 
 
 def make_output_stream(
     config: FluffConfig,
     format: Optional[str] = None,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/config.py` & `sqlfluff-2.2.0/src/sqlfluff/core/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,47 @@
 """Module for loading config."""
 
+try:
+    from importlib.resources import files
+except ImportError:  # pragma: no cover
+    # fallback for python <=3.8
+    from importlib_resources import files  # type: ignore
+
 import logging
 import os
 import os.path
 import configparser
 import sys
 from dataclasses import dataclass
 
 import pluggy
 from itertools import chain
-from typing import Dict, Iterator, List, Tuple, Any, Optional, Union, Iterable, Callable
+from typing import (
+    TYPE_CHECKING,
+    Dict,
+    Iterator,
+    List,
+    Set,
+    Tuple,
+    Any,
+    Optional,
+    Type,
+    Union,
+    Iterable,
+    Callable,
+)
 from pathlib import Path
 from sqlfluff.core.plugin.host import get_plugin_manager
 from sqlfluff.core.errors import SQLFluffUserError
 
 import appdirs
 
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.templaters.base import RawTemplater
+
 if sys.version_info >= (3, 11):
     import tomllib
 else:  # pragma: no cover
     import toml as tomllib
 
 # Instantiate the config logger
 config_logger = logging.getLogger("sqlfluff.config")
@@ -180,15 +202,15 @@
             elif cleaned_val in ["none"]:
                 v = None
             else:
                 v = val
     return v
 
 
-def nested_combine(*dicts: dict) -> dict:
+def nested_combine(*dicts: Dict[str, Any]) -> Dict[str, Any]:
     """Combine an iterable of dictionaries.
 
     Each dictionary is combined into a result dictionary. For
     each key in the first dictionary, it will be overwritten
     by any same-named key in any later dictionaries in the
     iterable. If the element at that key is a dictionary, rather
     than just overwriting we use the same function to combine
@@ -204,15 +226,15 @@
     >>> nested_combine({"a": {"b": "c"}}, {"a": {"d": "e"}})
     {'a': {'b': 'c', 'd': 'e'}}
 
     Keys overwrite left to right:
     >>> nested_combine({"a": {"b": "c"}}, {"a": {"b": "e"}})
     {'a': {'b': 'e'}}
     """
-    r: dict = {}
+    r: Dict[str, Any] = {}
     for d in dicts:
         for k in d:
             if k in r and isinstance(r[k], dict):
                 if isinstance(d[k], dict):
                     r[k] = nested_combine(r[k], d[k])
                 else:  # pragma: no cover
                     raise ValueError(
@@ -220,16 +242,18 @@
                         "{!r}".format(k, d[k])
                     )
             else:
                 r[k] = d[k]
     return r
 
 
-def dict_diff(left: dict, right: dict, ignore: Optional[List[str]] = None) -> dict:
-    """Work out the difference between to dictionaries.
+def dict_diff(
+    left: Dict[str, Any], right: Dict[str, Any], ignore: Optional[List[str]] = None
+) -> Dict[str, Any]:
+    """Work out the difference between two dictionaries.
 
     Returns a dictionary which represents elements in the `left`
     dictionary which aren't in the `right` or are different to
     those in the `right`. If the element is a dictionary, we
     recursively look for differences in those dictionaries,
     likewise only returning the differing elements.
 
@@ -252,15 +276,15 @@
 
     Ignoring works on a key basis:
     >>> dict_diff({"a": "b"}, {"a": "c"})
     {'a': 'b'}
     >>> dict_diff({"a": "b"}, {"a": "c"}, ["a"])
     {}
     """
-    buff: dict = {}
+    buff: Dict[str, Any] = {}
     for k in left:
         if ignore and k in ignore:
             continue
         # Is the key there at all?
         if k not in right:
             buff[k] = left[k]
         # Is the content the same?
@@ -286,27 +310,53 @@
         return raw
     raise SQLFluffUserError(
         f"Expected list or comma separated string. Got {type(raw)}"
         f" instead for value {raw}."
     )
 
 
+def split_colon_separated_string(in_str: str) -> Tuple[Tuple[str, ...], str]:
+    """Converts a colon separated string.
+
+    NOTE: This also includes some provisions for values which may be
+    Windows paths containing colons and NOT stripping those.
+    """
+    config_path: List[str] = []
+    for element in in_str.split(":"):
+        # If the next element begins with a backslash, and the previous
+        # one had length == 1,  then this is probably a windows path.
+        # In which case, rejoin them together.
+        element = element.strip()
+        if (
+            element
+            and element[0] == "\\"
+            and config_path[-1]
+            and len(config_path[-1]) == 1
+        ):
+            config_path[-1] = config_path[-1] + ":" + element
+        else:
+            # Otherwise just add it to the path.
+            config_path.append(element)
+
+    return tuple(config_path[:-1]), config_path[-1]
+
+
 class ConfigLoader:
     """The class for loading config files.
 
     Note:
         Unlike most cfg file readers, sqlfluff is case-sensitive in how
         it reads config files. This is to ensure we support the case
         sensitivity of jinja.
 
     """
 
     def __init__(self) -> None:
         # TODO: check that this cache implementation is actually useful
-        self._config_cache: dict = {}
+        self._config_cache: Dict[str, Dict[str, Any]] = {}
 
     @classmethod
     def get_global(cls) -> "ConfigLoader":
         """Get the singleton loader."""
         global global_loader
         if not global_loader:
             global_loader = cls()
@@ -358,15 +408,17 @@
                 buff.extend(cls._walk_toml(v, key))
             else:
                 buff.append((key, v))
 
         return buff
 
     @classmethod
-    def _iter_config_elems_from_dict(cls, configs: dict) -> Iterator[ConfigElemType]:
+    def _iter_config_elems_from_dict(
+        cls, configs: Dict[str, Any]
+    ) -> Iterator[ConfigElemType]:
         """Walk a config dict and get config elements.
 
         >>> list(
         ...    ConfigLoader._iter_config_elems_from_dict(
         ...        {"foo":{"bar":{"baz": "a", "biz": "b"}}}
         ...    )
         ... )
@@ -376,29 +428,29 @@
             if isinstance(val, dict):
                 for partial_key, sub_val in cls._iter_config_elems_from_dict(val):
                     yield (key,) + partial_key, sub_val
             else:
                 yield (key,), val
 
     @classmethod
-    def _config_elems_to_dict(cls, configs: Iterable[ConfigElemType]) -> dict:
+    def _config_elems_to_dict(cls, configs: Iterable[ConfigElemType]) -> Dict[str, Any]:
         """Reconstruct config elements into a dict.
 
         >>> ConfigLoader._config_elems_to_dict(
         ...     [(("foo", "bar", "baz"), "a"), (("foo", "bar", "biz"), "b")]
         ... )
         {'foo': {'bar': {'baz': 'a', 'biz': 'b'}}}
         """
-        result: Dict[str, Union[dict, str]] = {}
+        result: Dict[str, Any] = {}
         for key, val in configs:
             ref = result
             for step in key[:-1]:
                 if step not in ref:
                     ref[step] = {}
-                ref = ref[step]  # type: ignore
+                ref = ref[step]
             ref[key[-1]] = val
         return result
 
     @classmethod
     def _get_config_elems_from_toml(cls, fpath: str) -> List[ConfigElemType]:
         """Load a config from a TOML file and return a list of tuples.
 
@@ -408,15 +460,17 @@
         with open(fpath, mode="r") as file:
             config = tomllib.loads(file.read())
         tool = config.get("tool", {}).get("sqlfluff", {})
 
         return cls._walk_toml(tool)
 
     @classmethod
-    def _get_config_elems_from_file(cls, fpath: str) -> List[ConfigElemType]:
+    def _get_config_elems_from_file(
+        cls, fpath: Optional[str] = None, config_string: Optional[str] = None
+    ) -> List[ConfigElemType]:
         """Load a config from a file and return a list of tuples.
 
         The return value is a list of tuples, were each tuple has two elements,
         the first is a tuple of paths, the second is the value at that path.
 
         Note:
             Unlike most cfg file readers, sqlfluff is case-sensitive in how
@@ -424,27 +478,35 @@
 
         Note:
             Any variable names ending with `_path` or `_dir`, will be attempted to be
             resolved as relative paths to this config file. If that fails the
             string value will remain.
 
         """
-        buff: List[Tuple[tuple, Any]] = []
+        assert fpath or config_string, "One of fpath or config_string is required."
+        buff: List[ConfigElemType] = []
         # Disable interpolation so we can load macros
-        kw: Dict = {}
+        kw: Dict[str, Any] = {}
         kw["interpolation"] = None
         config = configparser.ConfigParser(delimiters="=", **kw)
         # NB: We want to be case sensitive in how we read from files,
         # because jinja is also case sensitive. To do this we override
         # the optionxform attribute.
         config.optionxform = lambda option: option  # type: ignore
-        config.read(fpath)
+        if fpath:
+            config.read(fpath)
+        else:
+            assert config_string
+            config.read_string(config_string)
+            # Set the fpath to the current working directory
+            fpath = os.getcwd()
+
         for k in config.sections():
             if k == "sqlfluff":
-                key: Tuple = ("core",)
+                key: Tuple[str, ...] = ("core",)
             elif k.startswith("sqlfluff:"):
                 # Return a tuple of nested values
                 key = tuple(k[len("sqlfluff:") :].split(":"))
             else:  # pragma: no cover
                 # if it doesn't start with sqlfluff, then don't go
                 # further on this iteration
                 continue
@@ -466,23 +528,25 @@
                     # One path
                     v = cls._resolve_path(fpath, val)
                 # Add the name to the end of the key
                 buff.append((key + (name,), v))
         return buff
 
     @classmethod
-    def _resolve_path(cls, fpath, val):
+    def _resolve_path(cls, fpath: str, val: str) -> str:
         """Try to resolve a path."""
         # Make the referenced path.
         ref_path = os.path.join(os.path.dirname(fpath), val)
         # Check if it exists, and if it does, replace the value with the path.
         return ref_path if os.path.exists(ref_path) else val
 
     @staticmethod
-    def _incorporate_vals(ctx: dict, vals: List[ConfigElemType]) -> dict:
+    def _incorporate_vals(
+        ctx: Dict[str, Any], vals: List[ConfigElemType]
+    ) -> Dict[str, Any]:
         """Take a list of tuples and incorporate it into a dictionary.
 
         >>> ConfigLoader._incorporate_vals({}, [(("a", "b"), "c")])
         {'a': {'b': 'c'}}
         >>> ConfigLoader._incorporate_vals({"a": {"b": "c"}}, [(("a", "d"), "e")])
         {'a': {'b': 'c', 'd': 'e'}}
         """
@@ -505,15 +569,15 @@
                     r = r[dp]
             # Deal with the value itself
             r[n] = v
         return ctx
 
     @staticmethod
     def _validate_configs(
-        configs: Iterable[ConfigElemType], file_path
+        configs: Iterable[ConfigElemType], file_path: str
     ) -> List[ConfigElemType]:
         """Validate config elements.
 
         We validate in two ways:
         1. Are these config settings removed or deprecated.
         2. Are these config elements in the layout section _valid_.
         """
@@ -595,27 +659,55 @@
                         "See https://docs.sqlfluff.com/en/stable/layout.html"
                         "#configuring-layout for more details."
                     )
 
             validated_configs.append((k, v))
         return validated_configs
 
+    def load_config_resource(
+        self, package: str, file_name: str, configs: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """Load a config resource.
+
+        This is however more compatible with mypyc because it avoids
+        the use of the __file__ object to find the default config.
+
+        This is only tested extensively with the default config.
+
+        NOTE: This requires that the config file is built into
+        a package but should be more performant because it leverages
+        importlib.
+        https://docs.python.org/3/library/importlib.resources.html
+        """
+        config_string = files(package).joinpath(file_name).read_text()
+        elems = self._get_config_elems_from_file(config_string=config_string)
+        elems = self._validate_configs(elems, package + "." + file_name)
+        return self._incorporate_vals(configs or {}, elems)
+
     def load_config_file(
-        self, file_dir: str, file_name: str, configs: Optional[dict] = None
-    ) -> dict:
-        """Load the default config file."""
+        self, file_dir: str, file_name: str, configs: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """Load a config file."""
         file_path = os.path.join(file_dir, file_name)
         if file_name == "pyproject.toml":
             elems = self._get_config_elems_from_toml(file_path)
         else:
             elems = self._get_config_elems_from_file(file_path)
         elems = self._validate_configs(elems, file_path)
         return self._incorporate_vals(configs or {}, elems)
 
-    def load_config_at_path(self, path: str) -> dict:
+    def load_config_string(
+        self, config_string: str, configs: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """Load a config from the string in cfg format."""
+        elems = self._get_config_elems_from_file(config_string=config_string)
+        elems = self._validate_configs(elems, "<config string>")
+        return self._incorporate_vals(configs or {}, elems)
+
+    def load_config_at_path(self, path: str) -> Dict[str, Any]:
         """Load config from a given path."""
         # First check the cache
         if str(path) in self._config_cache:
             return self._config_cache[str(path)]
 
         # The potential filenames we would look for at this path.
         # NB: later in this list overwrites earlier
@@ -623,15 +715,15 @@
             "setup.cfg",
             "tox.ini",
             "pep8.ini",
             ".sqlfluff",
             "pyproject.toml",
         ]
 
-        configs: dict = {}
+        configs: Dict[str, Any] = {}
 
         if os.path.isdir(path):
             p = path
         else:
             p = os.path.dirname(path)
 
         d = os.listdir(os.path.expanduser(p))
@@ -640,26 +732,26 @@
             if fname in d:
                 configs = self.load_config_file(p, fname, configs=configs)
 
         # Store in the cache
         self._config_cache[str(path)] = configs
         return configs
 
-    def load_extra_config(self, extra_config_path: str) -> dict:
+    def load_extra_config(self, extra_config_path: str) -> Dict[str, Any]:
         """Load specified extra config."""
         if not os.path.exists(extra_config_path):
             raise SQLFluffUserError(
                 f"Extra config '{extra_config_path}' does not exist."
             )
 
         # First check the cache
         if str(extra_config_path) in self._config_cache:
             return self._config_cache[str(extra_config_path)]
 
-        configs: dict = {}
+        configs: Dict[str, Any] = {}
         if extra_config_path.endswith("pyproject.toml"):
             elems = self._get_config_elems_from_toml(extra_config_path)
         else:
             elems = self._get_config_elems_from_file(extra_config_path)
         configs = self._incorporate_vals(configs, elems)
 
         # Store in the cache
@@ -680,33 +772,33 @@
             appdirs.system = "darwin"
 
         if not os.path.exists(user_config_dir_path):
             user_config_dir_path = appdirs.user_config_dir(appname, appauthor)
 
         return user_config_dir_path
 
-    def load_user_appdir_config(self) -> dict:
+    def load_user_appdir_config(self) -> Dict[str, Any]:
         """Load the config from the user's OS specific appdir config directory."""
         user_config_dir_path = self._get_user_config_dir_path()
         if os.path.exists(user_config_dir_path):
             return self.load_config_at_path(user_config_dir_path)
         else:
             return {}
 
-    def load_user_config(self) -> dict:
+    def load_user_config(self) -> Dict[str, Any]:
         """Load the config from the user's home directory."""
         user_home_path = os.path.expanduser("~")
         return self.load_config_at_path(user_home_path)
 
     def load_config_up_to_path(
         self,
         path: str,
         extra_config_path: Optional[str] = None,
         ignore_local_config: bool = False,
-    ) -> dict:
+    ) -> Dict[str, Any]:
         """Loads a selection of config files from both the path and its parent paths."""
         user_appdir_config = (
             self.load_user_appdir_config() if not ignore_local_config else {}
         )
         user_config = self.load_user_config() if not ignore_local_config else {}
         config_paths = (
             self.iter_config_locations_up_to_path(path)
@@ -723,31 +815,36 @@
         )
         return nested_combine(
             user_appdir_config, user_config, *config_stack, extra_config
         )
 
     @classmethod
     def find_ignore_config_files(
-        cls, path, working_path=Path.cwd(), ignore_file_name=".sqlfluffignore"
-    ):
+        cls,
+        path: str,
+        working_path: Union[str, Path] = Path.cwd(),
+        ignore_file_name: str = ".sqlfluffignore",
+    ) -> Set[str]:
         """Finds sqlfluff ignore files from both the path and its parent paths."""
         return set(
             filter(
                 os.path.isfile,
                 map(
                     lambda x: os.path.join(x, ignore_file_name),
                     cls.iter_config_locations_up_to_path(
                         path=path, working_path=working_path
                     ),
                 ),
             )
         )
 
     @staticmethod
-    def iter_config_locations_up_to_path(path, working_path=Path.cwd()):
+    def iter_config_locations_up_to_path(
+        path: str, working_path: Union[str, Path] = Path.cwd()
+    ) -> Iterator[str]:
         """Finds config locations from both the path and its parent paths.
 
         The lowest priority is the user appdir, then home dir, then increasingly
         the configs closest to the file being directly linted.
         """
         given_path = Path(path).absolute()
         working_path = Path(working_path).absolute()
@@ -778,18 +875,18 @@
 class FluffConfig:
     """The class that actually gets passed around as a config object."""
 
     private_vals = "rule_denylist", "rule_allowlist", "dialect_obj", "templater_obj"
 
     def __init__(
         self,
-        configs: Optional[dict] = None,
+        configs: Optional[Dict[str, Any]] = None,
         extra_config_path: Optional[str] = None,
         ignore_local_config: bool = False,
-        overrides: Optional[dict] = None,
+        overrides: Optional[Dict[str, Any]] = None,
         plugin_manager: Optional[pluggy.PluginManager] = None,
         # Ideally a dialect should be set when config is read but sometimes
         # it might only be set in nested .sqlfluff config files, so allow it
         # to be not required.
         require_dialect: bool = True,
     ):
         self._extra_config_path = (
@@ -883,28 +980,28 @@
             raise SQLFluffUserError(
                 "No dialect was specified. You must configure a dialect or "
                 "specify one on the command line using --dialect after the "
                 "command. Available dialects:\n"
                 f"{', '.join([d.label for d in dialect_readout()])}"
             )
 
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, Any]:
         # Copy the object's state from self.__dict__ which contains
         # all our instance attributes. Always use the dict.copy()
         # method to avoid modifying the original state.
         state = self.__dict__.copy()
         # Remove the unpicklable entries.
         del state["_plugin_manager"]
         # The dbt templater doesn't pickle well, but isn't required
         # within threaded operations. If it was, it could easily be
         # rehydrated within the thread.
         state["_configs"]["core"].pop("templater_obj", None)
         return state
 
-    def __setstate__(self, state):  # pragma: no cover
+    def __setstate__(self, state: Dict[str, Any]) -> None:  # pragma: no cover
         # Restore instance attributes
         self.__dict__.update(state)
         # NB: We don't reinstate the plugin manager, but this should only
         # be happening between processes where the plugin manager should
         # probably be fresh in any case.
         # NOTE: This means that registering user plugins directly will only
         # work if those plugins are used in the main process (i.e. templaters).
@@ -918,16 +1015,16 @@
         # processes.
 
     @classmethod
     def from_root(
         cls,
         extra_config_path: Optional[str] = None,
         ignore_local_config: bool = False,
-        overrides: Optional[dict] = None,
-        **kw,
+        overrides: Optional[Dict[str, Any]] = None,
+        **kw: Any,
     ) -> "FluffConfig":
         """Loads a config object just based on the root directory."""
         loader = ConfigLoader.get_global()
         c = loader.load_config_up_to_path(
             path=".",
             extra_config_path=extra_config_path,
             ignore_local_config=ignore_local_config,
@@ -937,20 +1034,40 @@
             extra_config_path=extra_config_path,
             ignore_local_config=ignore_local_config,
             overrides=overrides,
             **kw,
         )
 
     @classmethod
+    def from_string(
+        cls,
+        config_string: str,
+        extra_config_path: Optional[str] = None,
+        ignore_local_config: bool = False,
+        overrides: Optional[Dict[str, Any]] = None,
+        plugin_manager: Optional[pluggy.PluginManager] = None,
+    ) -> "FluffConfig":
+        """Loads a config object given a particular path."""
+        loader = ConfigLoader.get_global()
+        c = loader.load_config_string(config_string)
+        return cls(
+            configs=c,
+            extra_config_path=extra_config_path,
+            ignore_local_config=ignore_local_config,
+            overrides=overrides,
+            plugin_manager=plugin_manager,
+        )
+
+    @classmethod
     def from_path(
         cls,
         path: str,
         extra_config_path: Optional[str] = None,
         ignore_local_config: bool = False,
-        overrides: Optional[dict] = None,
+        overrides: Optional[Dict[str, Any]] = None,
         plugin_manager: Optional[pluggy.PluginManager] = None,
     ) -> "FluffConfig":
         """Loads a config object given a particular path."""
         loader = ConfigLoader.get_global()
         c = loader.load_config_up_to_path(
             path=path,
             extra_config_path=extra_config_path,
@@ -995,17 +1112,19 @@
             overrides["rules"] = ",".join(rules)
         if exclude_rules:
             # Make a comma separated string to pass in as override
             overrides["exclude_rules"] = ",".join(exclude_rules)
 
         return cls(overrides=overrides, require_dialect=require_dialect)
 
-    def get_templater(self, templater_name="jinja", **kwargs):
+    def get_templater(
+        self, templater_name: str = "jinja", **kwargs: Any
+    ) -> "RawTemplater":
         """Fetch a templater by name."""
-        templater_lookup = {
+        templater_lookup: Dict[str, Type["RawTemplater"]] = {
             templater.name: templater
             for templater in chain.from_iterable(
                 self._plugin_manager.hook.get_templaters()
             )
         }
         try:
             cls = templater_lookup[templater_name]
@@ -1029,15 +1148,15 @@
             path,
             extra_config_path=self._extra_config_path,
             ignore_local_config=self._ignore_local_config,
             overrides=self._overrides,
             plugin_manager=self._plugin_manager,
         )
 
-    def diff_to(self, other: "FluffConfig") -> dict:
+    def diff_to(self, other: "FluffConfig") -> Dict[str, Any]:
         """Compare this config to another.
 
         Args:
             other (:obj:`FluffConfig`): Another config object to compare
                 against. We will return keys from *this* object that are
                 not in `other` or are different to those in `other`.
 
@@ -1048,15 +1167,15 @@
         """
         # We ignore some objects which are not meaningful in the comparison
         # e.g. dialect_obj, which is generated on the fly.
         return dict_diff(self._configs, other._configs, ignore=["dialect_obj"])
 
     def get(
         self, val: str, section: Union[str, Iterable[str]] = "core", default: Any = None
-    ):
+    ) -> Any:
         """Get a particular value from the config."""
         section_dict = self.get_section(section)
         if section_dict is None:
             return default
 
         return section_dict.get(val, default)
 
@@ -1081,36 +1200,38 @@
             buff = self._configs
             for sec in section:
                 buff = buff.get(sec, None)
                 if buff is None:
                     return None
             return buff
 
-    def set_value(self, config_path: Iterable[str], val: Any):
+    def set_value(self, config_path: Iterable[str], val: Any) -> None:
         """Set a value at a given path."""
         # Make the path a list so we can index on it
         config_path = list(config_path)
         # Coerce the value into something more useful.
         config_val = coerce_value(val)
         # Sort out core if not there
         if len(config_path) == 1:  # pragma: no cover TODO?
             config_path = ["core"] + config_path
         # Current section:
         dict_buff = [self._configs]
         for elem in config_path[:-1]:
-            dict_buff.append(dict_buff[-1][elem])
+            dict_buff.append(dict_buff[-1].get(elem, {}))
         # Set the value
         dict_buff[-1][config_path[-1]] = config_val
         # Rebuild the config
         for elem in reversed(config_path[:-1]):
             dict_elem = dict_buff.pop()
             dict_buff[-1][elem] = dict_elem
         self._configs = dict_buff[0]
 
-    def iter_vals(self, cfg: Optional[dict] = None) -> Iterable[tuple]:
+    def iter_vals(
+        self, cfg: Optional[Dict[str, Any]] = None
+    ) -> Iterable[Tuple[Any, ...]]:
         """Return an iterable of tuples representing keys.
 
         We show values before dicts, the tuple contains an indent
         value to know what level of the dict we're in. Dict labels
         will be returned as a blank value before their content.
         """
         cfg = cfg or self._configs
@@ -1131,38 +1252,38 @@
             if isinstance(cfg[k], dict):
                 # First yield the dict label
                 yield (0, k, "")
                 # Then yield its content
                 for idnt, key, val in self.iter_vals(cfg=cfg[k]):
                     yield (idnt + 1, key, val)
 
-    def process_inline_config(self, config_line: str, fname: str):
+    def process_inline_config(self, config_line: str, fname: str) -> None:
         """Process an inline config command and update self."""
         # Strip preceding comment marks
         if config_line.startswith("--"):
             config_line = config_line[2:].strip()
         # Strip preceding sqlfluff line.
         if not config_line.startswith("sqlfluff:"):  # pragma: no cover
             config_logger.warning(
                 "Unable to process inline config statement: %r", config_line
             )
             return
         config_line = config_line[9:].strip()
-        # Divide on colons
-        config_path = [elem.strip() for elem in config_line.split(":")]
-        config_val = (tuple(config_path[:-1]), config_path[-1])
+        config_val = split_colon_separated_string(config_line)
         # Validate the value
         ConfigLoader._validate_configs([config_val], fname)
         # Set the value
         self.set_value(*config_val)
-        # If the config is for dialect, initialise the dialect
-        if config_path[:-1] == ["dialect"]:
-            self._initialise_dialect(config_path[-1])
+        # If the config is for dialect, initialise the dialect.
+        # NOTE: Comparison with a 1-tuple is intentional here as
+        # the first element of config_val is a tuple.
+        if config_val[0] == ("dialect",):
+            self._initialise_dialect(config_val[1])
 
-    def process_raw_file_for_config(self, raw_str: str, fname: str):
+    def process_raw_file_for_config(self, raw_str: str, fname: str) -> None:
         """Process a full raw file for inline config and update self."""
         # Scan the raw file for config commands.
         for raw_line in raw_str.splitlines():
             # With or without a space.
             if raw_line.startswith(("-- sqlfluff", "--sqlfluff")):
                 # Found a in-file config command
                 self.process_inline_config(raw_line, fname)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.2.0/src/sqlfluff/core/default_config.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # Number of passes to run before admitting defeat
 runaway_limit = 10
 # Ignore errors by category (one or more of the following, separated by commas: lexing,linting,parsing,templating)
 ignore = None
 # Warn only for rule codes (one of more rule codes, seperated by commas: e.g. LT01,LT02)
 # Also works for templating and parsing errors by using TMP or PRS
 warnings = None
+# Whether to warn about unneeded '-- noqa:' comments.
+warn_unused_ignores = False
 # Ignore linting errors found within sections of code coming directly from
 # templated code (e.g. from within Jinja curly braces. Note that it does not
 # ignore errors from literal code found within template loops.
 ignore_templated_areas = True
 # can either be autodetect or a valid encoding e.g. utf-8, utf-8-sig
 encoding = autodetect
 # Ignore inline overrides (e.g. to test if still required)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.2.0/src/sqlfluff/core/dialects/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Defines the base dialect class."""
 
 import sys
-from typing import Set, Union, Type
+from typing import Set, Union, Type, Dict, Any, Optional, List
 
 from sqlfluff.core.parser import (
     KeywordSegment,
     SegmentGenerator,
     BaseSegment,
     StringParser,
 )
 from sqlfluff.core.parser.grammar.base import BaseGrammar
+from sqlfluff.core.parser.lexer import LexerType
 from sqlfluff.core.parser.matchable import Matchable
 
 DialectElementType = Union[Type[BaseSegment], Matchable, SegmentGenerator]
 # NOTE: Post expansion, no generators remain
 ExpandedDialectElementType = Union[Type[BaseSegment], Matchable]
 
 
@@ -25,30 +26,30 @@
         lexer_matchers (iterable of :obj:`StringLexer`): A structure defining
             the lexing config for this dialect.
 
     """
 
     def __init__(
         self,
-        name,
-        lexer_matchers=None,
+        name: str,
+        root_segment_name: str,
+        lexer_matchers: Optional[List[LexerType]] = None,
         library=None,
-        sets=None,
-        inherits_from=None,
-        root_segment_name=None,
-    ):
+        sets: Optional[Dict[str, Set[str]]] = None,
+        inherits_from: Optional[str] = None,
+    ) -> None:
         self._library = library or {}
         self.name = name
         self.lexer_matchers = lexer_matchers
         self.expanded = False
         self._sets = sets or {}
         self.inherits_from = inherits_from
         self.root_segment_name = root_segment_name
 
-    def __repr__(self):  # pragma: no cover
+    def __repr__(self) -> str:  # pragma: no cover
         return f"<Dialect: {self.name}>"
 
     def expand(self) -> "Dialect":
         """Expand any callable references to concrete ones.
 
         This must be called before using the dialect. But
         allows more flexible definitions to happen at runtime.
@@ -65,35 +66,34 @@
         # Are we already expanded?
         if self.expanded:  # pragma: no cover
             raise ValueError("Attempted to re-expand an already expanded dialect.")
 
         expanded_copy = self.copy_as(name=self.name)
         # Expand any callable elements of the dialect.
         for key in expanded_copy._library:
-            if isinstance(expanded_copy._library[key], SegmentGenerator):
+            seg_gen = expanded_copy._library[key]
+            if isinstance(seg_gen, SegmentGenerator):
                 # If the element is callable, call it passing the current
                 # dialect and store the result in its place.
                 # Use the .replace() method for its error handling.
-                expanded_copy.replace(
-                    **{key: expanded_copy._library[key].expand(expanded_copy)}
-                )
+                expanded_copy.replace(**{key: seg_gen.expand(expanded_copy)})
         # Expand any keyword sets.
         for keyword_set in [
             "unreserved_keywords",
             "reserved_keywords",
         ]:  # e.g. reserved_keywords, (JOIN, ...)
             # Make sure the values are available as KeywordSegments
             for kw in expanded_copy.sets(keyword_set):
                 n = kw.capitalize() + "KeywordSegment"
                 if n not in expanded_copy._library:
                     expanded_copy._library[n] = StringParser(kw.lower(), KeywordSegment)
         expanded_copy.expanded = True
         return expanded_copy
 
-    def sets(self, label) -> Set:
+    def sets(self, label: str) -> Set:
         """Allows access to sets belonging to this dialect.
 
         These sets belong to the dialect and are copied for sub
         dialects. These are used in combination with late-bound
         dialect objects to create some of the bulk-produced rules.
 
         """
@@ -105,15 +105,15 @@
         self, set_label: str, values: str
     ) -> None:
         """Special function to update a keywords set from a multi-line string."""
         self.sets(set_label).update(
             [n.strip().upper() for n in values.strip().split("\n")]
         )
 
-    def copy_as(self, name):
+    def copy_as(self, name: str) -> "Dialect":
         """Copy this dialect and create a new one with a different name.
 
         This is the primary method for inheritance, after which, the
         `replace` method can be used to override particular rules.
         """
         # Are we already expanded?
         if self.expanded:  # pragma: no cover
@@ -122,24 +122,26 @@
             raise ValueError("Attempted to copy an already expanded dialect.")
 
         # Copy sets if they are passed, so they can be mutated independently
         new_sets = {}
         for label in self._sets:
             new_sets[label] = self._sets[label].copy()
 
+        assert self.lexer_matchers
+
         return self.__class__(
             name=name,
             library=self._library.copy(),
             lexer_matchers=self.lexer_matchers.copy(),
             sets=new_sets,
             inherits_from=self.name,
             root_segment_name=self.root_segment_name,
         )
 
-    def add(self, **kwargs: DialectElementType):
+    def add(self, **kwargs: DialectElementType) -> None:
         """Add a segment to the dialect directly.
 
         This is the alternative to the decorator route, most useful for segments
         defined using `make`. Segments are passed in as kwargs.
 
         e.g.
         dialect.add(SomeSegment=StringParser("blah", KeywordSegment))
@@ -148,15 +150,15 @@
         will iterate through the kwargs
         """
         for n in kwargs:
             if n in self._library:  # pragma: no cover
                 raise ValueError(f"{n!r} is already registered in {self!r}")
             self._library[n] = kwargs[n]
 
-    def replace(self, **kwargs: DialectElementType):
+    def replace(self, **kwargs) -> None:
         """Override a segment on the dialect directly.
 
         Usage is very similar to add, but elements specified must already exist.
         """
         for n in kwargs:
             if n not in self._library:  # pragma: no cover
                 raise ValueError(f"{n!r} is not already registered in {self!r}")
@@ -172,14 +174,16 @@
 
             # To replace a segment, the replacement must either be a
             # subclass of the original, *or* it must have the same
             # public methods and/or fields as it.
             base_dir = set(dir(self._library[n]))
             subclass = False
             if isinstance(self._library[n], type) and isinstance(cls, type):
+                assert issubclass(self._library[n], BaseSegment)
+                assert issubclass(cls, BaseSegment)
                 subclass = issubclass(cls, self._library[n])
                 if not subclass:
                     if self._library[n].type != cls.type:
                         raise ValueError(  # pragma: no cover
                             f"Cannot replace {n!r} because 'type' property does not "
                             f"match: {cls.type} != {self._library[n].type}"
                         )
@@ -215,15 +219,15 @@
                             ):
                                 raise ValueError(
                                     f"Cannot replace {n!r} because it needs "
                                     f"to define '{grammar}'"
                                 )
             self._library[n] = cls
 
-    def add_update_segments(self, module_dct):
+    def add_update_segments(self, module_dct: Dict[str, Any]) -> None:
         """Scans module dictionary, adding or replacing segment definitions."""
         for k, v in module_dct.items():
             if isinstance(v, type) and issubclass(v, BaseSegment):
                 if k not in self._library:
                     self.add(**{k: v})
                 else:
                     self.replace(**{k: v})
@@ -232,47 +236,53 @@
         """Allow access to grammars pre-expansion.
 
         This is typically for dialect inheritance. This method
         also validates that the result is a grammar.
         """
         if name not in self._library:  # pragma: no cover
             raise ValueError(f"Element {name} not found in dialect.")
-        if not isinstance(self._library[name], BaseGrammar):  # pragma: no cover
+        grammar = self._library[name]
+        if not isinstance(grammar, BaseGrammar):  # pragma: no cover
             raise TypeError(
                 f"Attempted to fetch non grammar [{name}] with get_grammar."
             )
-        return self._library[name]
+        return grammar
 
     def get_segment(self, name: str) -> Type["BaseSegment"]:
         """Allow access to segments pre-expansion.
 
         This is typically for dialect inheritance. This method
         also validates that the result is a segment.
         """
         if name not in self._library:  # pragma: no cover
             raise ValueError(f"Element {name} not found in dialect.")
-        if not issubclass(self._library[name], BaseSegment):  # pragma: no cover
+        segment = self._library[name]
+
+        if issubclass(segment, BaseSegment):
+            return segment
+        else:  # pragma: no cover
             raise TypeError(
-                f"Attempted to fetch non segment [{name}] with get_segment."
+                f"Attempted to fetch non segment [{name}] "
+                f"with get_segment - type{type(segment)}"
             )
-        return self._library[name]
 
     def ref(self, name: str) -> ExpandedDialectElementType:
         """Return an object which acts as a late binding reference to the element named.
 
         NB: This requires the dialect to be expanded, and only returns Matchables
         as a result.
 
         """
         if not self.expanded:  # pragma: no cover
             raise RuntimeError("Dialect must be expanded before use.")
 
         if name in self._library:
             res = self._library[name]
             if res:
+                assert not isinstance(res, SegmentGenerator)
                 return res
             else:  # pragma: no cover
                 raise ValueError(
                     "Unexpected Null response while fetching {!r} from {}".format(
                         name, self.name
                     )
                 )
@@ -303,32 +313,32 @@
                     "Grammar refers to "
                     "{!r} which was not found in the {} dialect.".format(
                         name, self.name
                     )
                 )
             )
 
-    def set_lexer_matchers(self, lexer_matchers):
+    def set_lexer_matchers(self, lexer_matchers: List[LexerType]) -> None:
         """Set the lexer struct for the dialect.
 
         This is what is used for base dialects. For derived dialects
         (which don't exist yet) the assumption is that we'll introduce
         some kind of *patch* function which could be used to mutate
         an existing `lexer_matchers`.
         """
         self.lexer_matchers = lexer_matchers
 
-    def get_lexer_matchers(self):
+    def get_lexer_matchers(self) -> List[LexerType]:
         """Fetch the lexer struct for this dialect."""
         if self.lexer_matchers:
             return self.lexer_matchers
         else:  # pragma: no cover
             raise ValueError(f"Lexing struct has not been set for dialect {self}")
 
-    def patch_lexer_matchers(self, lexer_patch):
+    def patch_lexer_matchers(self, lexer_patch: List[LexerType]) -> None:
         """Patch an existing lexer struct.
 
         Used to edit the lexer of a sub-dialect.
         """
         buff = []
         if not self.lexer_matchers:  # pragma: no cover
             raise ValueError("Lexer struct must be defined before it can be patched!")
@@ -340,15 +350,15 @@
             if elem.name in patch_dict:
                 buff.append(patch_dict[elem.name])
             else:
                 buff.append(elem)
         # Overwrite with the buffer once we're done
         self.lexer_matchers = buff
 
-    def insert_lexer_matchers(self, lexer_patch, before):
+    def insert_lexer_matchers(self, lexer_patch: List[LexerType], before: str) -> None:
         """Insert new records into an existing lexer struct.
 
         Used to edit the lexer of a sub-dialect. The patch is
         inserted *before* whichever element is named in `before`.
         """
         buff = []
         found = False
@@ -367,10 +377,10 @@
         if not found:  # pragma: no cover
             raise ValueError(
                 f"Lexer struct insert before '{before}' failed because tag never found."
             )
         # Overwrite with the buffer once we're done
         self.lexer_matchers = buff
 
-    def get_root_segment(self):
+    def get_root_segment(self) -> Union[Type[BaseSegment], Matchable]:
         """Get the root segment of the dialect."""
         return self.ref(self.root_segment_name)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.2.0/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/enums.py` & `sqlfluff-2.2.0/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/errors.py` & `sqlfluff-2.2.0/src/sqlfluff/core/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-"""Errors - these are closely linked to what used to be called violations."""
-from typing import Optional, Tuple, Any, List
+"""Errors - these are closely linked to what used to be called violations.
+
+NOTE: The BaseException class, which ValueError inherits from, defines
+a custom __reduce__() method for picking and unpickling exceptions.
+For the SQLBaseError, and it's dependent classes, we define properties
+of these exceptions which don't work well with that method, which is
+why we redefine __reduce__() on each of these classes. Given the
+circumstances in which they are called, they don't show up on coverage
+tracking.
+
+https://stackoverflow.com/questions/49715881/how-to-pickle-inherited-exceptions
+"""
+from typing import Optional, Tuple, Any, List, Dict, Type, Union, TYPE_CHECKING
+
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.parser import PositionMarker, BaseSegment
+    from sqlfluff.core.rules import BaseRule, LintFix
 
 CheckTuple = Tuple[str, int, int]
 
 
 class SQLBaseError(ValueError):
     """Base Error Class for all violations."""
 
     _code: Optional[str] = None
     _identifier = "base"
+    _warning = False  # The default value for `warning`
 
     def __init__(
         self,
-        *args,
-        pos=None,
-        line_no=0,
-        line_pos=0,
-        ignore=False,
-        fatal=False,
-        warning=False,
-        **kwargs
-    ):
+        description: Optional[str] = None,
+        pos: Optional["PositionMarker"] = None,
+        line_no: int = 0,
+        line_pos: int = 0,
+        ignore: bool = False,
+        fatal: bool = False,
+        warning: Optional[bool] = None,
+    ) -> None:
         self.fatal = fatal
         self.ignore = ignore
-        self.warning = warning
+        self.warning: bool = warning if warning is not None else self._warning
+        self.description = description
         if pos:
             self.line_no, self.line_pos = pos.source_position()
         else:
             self.line_no = line_no
             self.line_pos = line_pos
-        super().__init__(*args, **kwargs)
+        super().__init__(self.desc())
+
+    def __reduce__(
+        self,
+    ) -> Tuple[Type["SQLBaseError"], Tuple[Any, ...]]:  # pragma: no cover
+        """Prepare the SQLBaseError for pickling."""
+        return type(self), (
+            self.description,
+            None,
+            self.line_no,
+            self.line_pos,
+            self.ignore,
+            self.fatal,
+            self.warning,
+        )
 
     @property
-    def fixable(self):
+    def fixable(self) -> bool:
         """Should this error be considered fixable?"""
         return False
 
     def rule_code(self) -> str:
-        """Fetch the code of the rule which cause this error.
-
-        NB: This only returns a real code for some subclasses of
-        error, (the ones with a `rule` attribute), but otherwise
-        returns a placeholder value which can be used instead.
-        """
-        if hasattr(self, "rule"):
-            return getattr(self, "rule").code
-
+        """Fetch the code of the rule which cause this error."""
         return self._code or "????"
 
     def desc(self) -> str:
-        """Fetch a description of this violation.
-
-        NB: For violations which don't directly implement a rule
-        this attempts to return the error message linked to whatever
-        caused the violation. Optionally some errors may have their
-        description set directly.
-        """
-        if hasattr(self, "description") and getattr(self, "description", None):
-            # This can only override if it's present AND
-            # if it's non-null.
-            return getattr(self, "description")
-
-        if hasattr(self, "rule"):
-            return getattr(self, "rule").description
-
-        # Return the first element - probably a string message
-        if len(self.args) > 1 and isinstance(self.args, str):  # pragma: no cover TODO?
-            return self.args
-
-        if len(self.args) == 1:
-            return self.args[0]
+        """Fetch a description of this violation."""
+        if self.description:
+            return self.description
 
         return self.__class__.__name__  # pragma: no cover
 
-    def get_info_dict(self):
+    def get_info_dict(self) -> Dict[str, Union[str, int]]:
         """Return a dict of properties.
 
         This is useful in the API for outputting violations.
         """
         return {
             "line_no": self.line_no,
             "line_pos": self.line_pos,
@@ -94,20 +98,20 @@
             self.line_pos,
         )
 
     def source_signature(self) -> Tuple[Any, ...]:
         """Return hashable source signature for deduplication."""
         return (self.check_tuple(), self.desc())
 
-    def ignore_if_in(self, ignore_iterable: List[str]):
+    def ignore_if_in(self, ignore_iterable: List[str]) -> None:
         """Ignore this violation if it matches the iterable."""
         if self._identifier in ignore_iterable:
             self.ignore = True
 
-    def warning_if_in(self, warning_iterable: List[str]):
+    def warning_if_in(self, warning_iterable: List[str]) -> None:
         """Warning only for this violation if it matches the iterable.
 
         Designed for rule codes so works with L001, LL0X but also TMP or PRS
         for templating and parsing errors.
         """
         if self.rule_code() in warning_iterable:
             self.warning = True
@@ -155,20 +159,35 @@
             used for logging and for referencing position.
 
     """
 
     _code = "PRS"
     _identifier = "parsing"
 
-    def __init__(self, *args, segment=None, **kwargs):
+    def __init__(
+        self,
+        description: Optional[str] = None,
+        segment: Optional["BaseSegment"] = None,
+        line_no: int = 0,
+        line_pos: int = 0,
+    ) -> None:
         # Store the segment on creation - we might need it later
         self.segment = segment
-        if self.segment:
-            kwargs["pos"] = self.segment.pos_marker
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            description=description,
+            pos=segment.pos_marker if segment else None,
+            line_no=line_no,
+            line_pos=line_pos,
+        )
+
+    def __reduce__(
+        self,
+    ) -> Tuple[Type["SQLParseError"], Tuple[Any, ...]]:  # pragma: no cover
+        """Prepare the SQLParseError for pickling."""
+        return type(self), (self.description, self.segment, self.line_no, self.line_pos)
 
 
 class SQLLintError(SQLBaseError):
     """An error which occurred during linting.
 
     In particular we reference the rule here to do extended logging based on
     the rule in question which caused the fail.
@@ -180,32 +199,45 @@
             used for logging and for referencing position.
 
     """
 
     _identifier = "linting"
 
     def __init__(
-        self, *args, segment=None, rule=None, fixes=None, description=None, **kwargs
-    ):
+        self,
+        description: str,
+        segment: "BaseSegment",
+        rule: "BaseRule",
+        fixes: Optional[List["LintFix"]] = None,
+    ) -> None:
         # Something about position, message and fix?
         self.segment = segment
-        if self.segment:
-            kwargs["pos"] = self.segment.pos_marker
         self.rule = rule
         self.fixes = fixes or []
-        self.description = description
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            description=description, pos=segment.pos_marker if segment else None
+        )
+
+    def __reduce__(
+        self,
+    ) -> Tuple[Type["SQLLintError"], Tuple[Any, ...]]:  # pragma: no cover
+        """Prepare the SQLLintError for pickling."""
+        return type(self), (self.description, self.segment, self.rule, self.fixes)
 
     @property
-    def fixable(self):
+    def fixable(self) -> bool:
         """Should this error be considered fixable?"""
         if self.fixes:
             return True
         return False
 
+    def rule_code(self) -> str:
+        """Fetch the code of the rule which cause this error."""
+        return self.rule.code
+
     def source_signature(self) -> Tuple[Any, ...]:
         """Return hashable source signature for deduplication.
 
         For linting errors we need to dedupe on more than just location and
         description, we also need to check the edits potentially made, both
         in the templated file but also in the source.
         """
@@ -214,18 +246,26 @@
         )
         source_fixes = tuple(
             tuple(tuple(e.source_fixes) for e in f.edit) if f.edit else None
             for f in self.fixes
         )
         return (self.check_tuple(), self.description, fix_raws, source_fixes)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<SQLLintError: rule {} pos:{!r}, #fixes: {}, description: {}>".format(
             self.rule_code(),
             (self.line_no, self.line_pos),
             len(self.fixes),
             self.description,
         )
 
 
+class SQLUnusedNoQaWarning(SQLBaseError):
+    """A warning about an unused noqa directive."""
+
+    _code = "NOQA"
+    _identifier = "noqa"
+    _warning = True
+
+
 class SQLFluffUserError(ValueError):
     """An error which should be fed back to the user."""
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import (
     List,
     NamedTuple,
     Optional,
     Tuple,
     Dict,
+    Any,
 )
 
 from sqlfluff.core.errors import SQLBaseError, SQLTemplaterError
 from sqlfluff.core.templaters import TemplatedFile
 from sqlfluff.core.config import FluffConfig
 from sqlfluff.core.parser.segments.base import BaseSegment
 
@@ -20,22 +21,14 @@
     code: str
     name: str
     description: str
     groups: Tuple[str, ...]
     aliases: Tuple[str, ...]
 
 
-class NoQaDirective(NamedTuple):
-    """Parsed version of a 'noqa' comment."""
-
-    line_no: int  # Source line number
-    rules: Optional[Tuple[str, ...]]  # Affected rule names
-    action: Optional[str]  # "enable", "disable", or "None"
-
-
 class RenderedFile(NamedTuple):
     """An object to store the result of a templated file/string.
 
     This is notable as it's the intermediate state between what happens
     in the main process and the child processes when running in parallel mode.
     """
 
@@ -61,12 +54,12 @@
             took in the process.
         `templated_file` is a :obj:`TemplatedFile` containing the details
             of the templated file.
     """
 
     tree: Optional[BaseSegment]
     violations: List[SQLBaseError]
-    time_dict: dict
+    time_dict: Dict[str, Any]
     templated_file: TemplatedFile
     config: FluffConfig
     fname: str
     source_str: str
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/linted_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     Any,
     Iterable,
     List,
     NamedTuple,
     Optional,
     Tuple,
     Union,
-    cast,
     Type,
     Dict,
 )
 
 from sqlfluff.core.errors import (
     SQLBaseError,
     SQLLintError,
@@ -33,15 +32,15 @@
     CheckTuple,
 )
 from sqlfluff.core.templaters import TemplatedFile, RawFileSlice
 
 # Classes needed only for type checking
 from sqlfluff.core.parser.segments import BaseSegment, FixPatch
 
-from sqlfluff.core.linter.common import NoQaDirective
+from sqlfluff.core.linter.noqa import IgnoreMask
 
 # Instantiate the linter logger
 linter_logger: logging.Logger = logging.getLogger("sqlfluff.linter")
 
 TMP_PRS_ERROR_TYPES = (SQLTemplaterError, SQLParseError)
 
 
@@ -72,19 +71,21 @@
 class LintedFile(NamedTuple):
     """A class to store the idea of a linted file."""
 
     path: str
     violations: List[SQLBaseError]
     timings: Optional[FileTimings]
     tree: Optional[BaseSegment]
-    ignore_mask: List[NoQaDirective]
+    ignore_mask: Optional[IgnoreMask]
     templated_file: TemplatedFile
     encoding: str
 
-    def check_tuples(self, raise_on_non_linting_violations=True) -> List[CheckTuple]:
+    def check_tuples(
+        self, raise_on_non_linting_violations: bool = True
+    ) -> List[CheckTuple]:
         """Make a list of check_tuples.
 
         This assumes that all the violations found are
         linting violations. If they don't then this function
         raises that error.
         """
         vs: List[CheckTuple] = []
@@ -123,14 +124,15 @@
 
     def get_violations(
         self,
         rules: Optional[Union[str, Tuple[str, ...]]] = None,
         types: Optional[Union[Type[SQLBaseError], Iterable[Type[SQLBaseError]]]] = None,
         filter_ignore: bool = True,
         filter_warning: bool = True,
+        warn_unused_ignores: bool = False,
         fixable: Optional[bool] = None,
     ) -> list:
         """Get a list of violations, respecting filters and ignore options.
 
         Optionally now with filters.
         """
         violations = self.violations
@@ -157,102 +159,21 @@
             # Fatal errors should always come through, regardless.
             violations = [v for v in violations if v.fixable is fixable or v.fatal]
         # Filter ignorable violations
         if filter_ignore:
             violations = [v for v in violations if not v.ignore]
             # Ignore any rules in the ignore mask
             if self.ignore_mask:
-                violations = self.ignore_masked_violations(violations, self.ignore_mask)
+                violations = self.ignore_mask.ignore_masked_violations(violations)
         # Filter warning violations
         if filter_warning:
             violations = [v for v in violations if not v.warning]
-        return violations
-
-    @staticmethod
-    def _ignore_masked_violations_single_line(
-        violations: List[SQLBaseError], ignore_mask: List[NoQaDirective]
-    ):
-        """Returns whether to ignore error for line-specific directives.
-
-        The "ignore" list is assumed to ONLY contain NoQaDirectives with
-        action=None.
-        """
-        for ignore in ignore_mask:
-            violations = [
-                v
-                for v in violations
-                if not (
-                    v.line_no == ignore.line_no
-                    and (ignore.rules is None or v.rule_code() in ignore.rules)
-                )
-            ]
-        return violations
-
-    @staticmethod
-    def _should_ignore_violation_line_range(
-        line_no: int, ignore_rule: List[NoQaDirective]
-    ):
-        """Returns whether to ignore a violation at line_no."""
-        # Loop through the NoQaDirectives to find the state of things at
-        # line_no. Assumptions about "ignore_rule":
-        # - Contains directives for only ONE RULE, i.e. the rule that was
-        #   violated at line_no
-        # - Sorted in ascending order by line number
-        disable = False
-        for ignore in ignore_rule:
-            if ignore.line_no > line_no:
-                break
-            disable = ignore.action == "disable"
-        return disable
-
-    @classmethod
-    def _ignore_masked_violations_line_range(
-        cls, violations: List[SQLBaseError], ignore_mask: List[NoQaDirective]
-    ):
-        """Returns whether to ignore error for line-range directives.
-
-        The "ignore" list is assumed to ONLY contain NoQaDirectives where
-        action is "enable" or "disable".
-        """
-        result = []
-        for v in violations:
-            # Find the directives that affect the violated rule "v", either
-            # because they specifically reference it or because they don't
-            # specify a list of rules, thus affecting ALL rules.
-            ignore_rule = sorted(
-                (
-                    ignore
-                    for ignore in ignore_mask
-                    if not ignore.rules
-                    or (v.rule_code() in cast(Tuple[str, ...], ignore.rules))
-                ),
-                key=lambda ignore: ignore.line_no,
-            )
-            # Determine whether to ignore the violation, based on the relevant
-            # enable/disable directives.
-            if not cls._should_ignore_violation_line_range(v.line_no, ignore_rule):
-                result.append(v)
-        return result
-
-    @classmethod
-    def ignore_masked_violations(
-        cls, violations: List[SQLBaseError], ignore_mask: List[NoQaDirective]
-    ) -> List[SQLBaseError]:
-        """Remove any violations specified by ignore_mask.
-
-        This involves two steps:
-        1. Filter out violations affected by single-line "noqa" directives.
-        2. Filter out violations affected by disable/enable "noqa" directives.
-        """
-        ignore_specific = [ignore for ignore in ignore_mask if not ignore.action]
-        ignore_range = [ignore for ignore in ignore_mask if ignore.action]
-        violations = cls._ignore_masked_violations_single_line(
-            violations, ignore_specific
-        )
-        violations = cls._ignore_masked_violations_line_range(violations, ignore_range)
+        # Add warnings for unneeded noqa if applicable
+        if warn_unused_ignores and not filter_warning and self.ignore_mask:
+            violations += self.ignore_mask.generate_warnings_for_unused()
         return violations
 
     def num_violations(self, **kwargs) -> int:
         """Count the number of violations.
 
         Optionally now with filters.
         """
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/linter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Defines the linter class."""
 
-import fnmatch
 import os
 import time
 import logging
 from typing import (
     Any,
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
-    Dict,
     cast,
 )
 
 import pathspec
 import regex
 from tqdm import tqdm
 
@@ -26,32 +24,31 @@
     SQLBaseError,
     SQLLexError,
     SQLLintError,
     SQLParseError,
     SQLFluffSkipFile,
     SQLFluffUserError,
 )
-from sqlfluff.core.parser import Lexer, Parser, RegexLexer
+from sqlfluff.core.parser import Lexer, Parser
 from sqlfluff.core.file_helpers import get_encoding
 from sqlfluff.core.templaters import TemplatedFile
 from sqlfluff.core.rules import get_ruleset
 from sqlfluff.core.config import FluffConfig, ConfigLoader, progress_bar_configuration
 
 # Classes needed only for type checking
 from sqlfluff.core.parser.segments.base import BaseSegment, SourceFix
 from sqlfluff.core.parser.segments.meta import MetaSegment
-from sqlfluff.core.parser.segments.raw import RawSegment
 from sqlfluff.core.rules import BaseRule, RulePack
 
 from sqlfluff.core.linter.common import (
     RuleTuple,
     ParsedString,
-    NoQaDirective,
     RenderedFile,
 )
+from sqlfluff.core.linter.noqa import IgnoreMask
 from sqlfluff.core.linter.linted_file import (
     LintedFile,
     FileTimings,
     TMP_PRS_ERROR_TYPES,
 )
 from sqlfluff.core.linter.linted_dir import LintedDir
 from sqlfluff.core.linter.linting_result import LintingResult
@@ -226,155 +223,85 @@
         parse_statistics: bool = False,
     ) -> Tuple[Optional[BaseSegment], List[SQLParseError]]:
         parser = Parser(config=config)
         violations = []
         # Parse the file and log any problems
         try:
             parsed: Optional[BaseSegment] = parser.parse(
-                tokens,
+                # Regardless of how the sequence was passed in, we should
+                # coerce it to a tuple here, before we head deeper into
+                # the parsing process.
+                tuple(tokens),
                 recurse=recurse,
                 fname=fname,
                 parse_statistics=parse_statistics,
             )
         except SQLParseError as err:
             linter_logger.info("PARSING FAILED! : %s", err)
             violations.append(err)
             return None, violations
 
-        if parsed:
-            linter_logger.info("\n###\n#\n# {}\n#\n###".format("Parsed Tree:"))
-            linter_logger.info("\n" + parsed.stringify())
-            # We may succeed parsing, but still have unparsable segments. Extract them
-            # here.
-            for unparsable in parsed.iter_unparsables():
-                # No exception has been raised explicitly, but we still create one here
-                # so that we can use the common interface
-                violations.append(
-                    SQLParseError(
-                        "Line {0[0]}, Position {0[1]}: Found unparsable section: "
-                        "{1!r}".format(
-                            unparsable.pos_marker.working_loc,
-                            unparsable.raw
-                            if len(unparsable.raw) < 40
-                            else unparsable.raw[:40] + "...",
-                        ),
-                        segment=unparsable,
-                    )
+        if parsed is None:  # pragma: no cover
+            return None, violations
+
+        linter_logger.info("\n###\n#\n# {}\n#\n###".format("Parsed Tree:"))
+        linter_logger.info("\n" + parsed.stringify())
+        # We may succeed parsing, but still have unparsable segments. Extract them
+        # here.
+        for unparsable in parsed.iter_unparsables():
+            # No exception has been raised explicitly, but we still create one here
+            # so that we can use the common interface
+            assert unparsable.pos_marker
+            violations.append(
+                SQLParseError(
+                    "Line {0[0]}, Position {0[1]}: Found unparsable section: "
+                    "{1!r}".format(
+                        unparsable.pos_marker.working_loc,
+                        unparsable.raw
+                        if len(unparsable.raw) < 40
+                        else unparsable.raw[:40] + "...",
+                    ),
+                    segment=unparsable,
                 )
-                linter_logger.info("Found unparsable segment...")
-                linter_logger.info(unparsable.stringify())
+            )
+            linter_logger.info("Found unparsable segment...")
+            linter_logger.info(unparsable.stringify())
         return parsed, violations
 
     @staticmethod
-    def parse_noqa(
-        comment: str,
-        line_no: int,
-        reference_map: Dict[str, Set[str]],
-    ):
-        """Extract ignore mask entries from a comment string."""
-        # Also trim any whitespace afterward
-
-        # Comment lines can also have noqa e.g.
-        # --dafhsdkfwdiruweksdkjdaffldfsdlfjksd -- noqa: LT05
-        # Therefore extract last possible inline ignore.
-        comment = [c.strip() for c in comment.split("--")][-1]
-
-        if comment.startswith("noqa"):
-            # This is an ignore identifier
-            comment_remainder = comment[4:]
-            if comment_remainder:
-                if not comment_remainder.startswith(":"):
-                    return SQLParseError(
-                        "Malformed 'noqa' section. Expected 'noqa: <rule>[,...]",
-                        line_no=line_no,
-                    )
-                comment_remainder = comment_remainder[1:].strip()
-                if comment_remainder:
-                    action: Optional[str]
-                    if "=" in comment_remainder:
-                        action, rule_part = comment_remainder.split("=", 1)
-                        if action not in {"disable", "enable"}:  # pragma: no cover
-                            return SQLParseError(
-                                "Malformed 'noqa' section. "
-                                "Expected 'noqa: enable=<rule>[,...] | all' "
-                                "or 'noqa: disable=<rule>[,...] | all",
-                                line_no=line_no,
-                            )
-                    else:
-                        action = None
-                        rule_part = comment_remainder
-                        if rule_part in {"disable", "enable"}:
-                            return SQLParseError(
-                                "Malformed 'noqa' section. "
-                                "Expected 'noqa: enable=<rule>[,...] | all' "
-                                "or 'noqa: disable=<rule>[,...] | all",
-                                line_no=line_no,
-                            )
-                    rules: Optional[Tuple[str, ...]]
-                    if rule_part != "all":
-                        # Rules can be globs therefore we compare to the rule_set to
-                        # expand the globs.
-                        unexpanded_rules = tuple(
-                            r.strip() for r in rule_part.split(",")
-                        )
-                        # We use a set to do natural deduplication.
-                        expanded_rules: Set[str] = set()
-                        for r in unexpanded_rules:
-                            matched = False
-                            for expanded in (
-                                reference_map[x]
-                                for x in fnmatch.filter(reference_map.keys(), r)
-                            ):
-                                expanded_rules |= expanded
-                                matched = True
-
-                            if not matched:
-                                # We were unable to expand the glob.
-                                # Therefore assume the user is referencing
-                                # a special error type (e.g. PRS, LXR, or TMP)
-                                # and add this to the list of rules to ignore.
-                                expanded_rules.add(r)
-                        # Sort for consistency
-                        rules = tuple(sorted(expanded_rules))
-                    else:
-                        rules = None
-                    return NoQaDirective(line_no, rules, action)
-            return NoQaDirective(line_no, None, None)
-        return None
-
-    @staticmethod
     def remove_templated_errors(
         linting_errors: List[SQLBaseError],
     ) -> List[SQLBaseError]:
         """Filter a list of lint errors, removing those from the templated slices."""
         # Filter out any linting errors in templated sections if relevant.
         result: List[SQLBaseError] = []
         for e in linting_errors:
             if isinstance(e, SQLLintError):
+                assert e.segment.pos_marker
                 if (
                     # Is it in a literal section?
                     e.segment.pos_marker.is_literal()
                     # Is it a rule that is designed to work on templated sections?
                     or e.rule.targets_templated
                 ):
                     result.append(e)
             else:
                 # If it's another type, just keep it. (E.g. SQLParseError from
                 # malformed "noqa" comment).
                 result.append(e)
         return result
 
     @staticmethod
-    def _report_conflicting_fixes_same_anchor(message: str):  # pragma: no cover
+    def _report_conflicting_fixes_same_anchor(message: str) -> None:  # pragma: no cover
         # This function exists primarily in order to let us monkeypatch it at
         # runtime (replacing it with a function that raises an exception).
         linter_logger.critical(message)
 
     @staticmethod
-    def _warn_unfixable(code: str):
+    def _warn_unfixable(code: str) -> None:
         linter_logger.warning(
             f"One fix for {code} not applied, it would re-cause the same error."
         )
 
     # ### Class Methods
     # These compose the base static methods into useful recipes.
 
@@ -424,87 +351,24 @@
             rendered.templated_file,
             rendered.config,
             rendered.fname,
             rendered.source_str,
         )
 
     @classmethod
-    def extract_ignore_from_comment(
-        cls,
-        comment: RawSegment,
-        reference_map: Dict[str, Set[str]],
-    ):
-        """Extract ignore mask entries from a comment segment."""
-        # Also trim any whitespace afterward
-        comment_content = comment.raw_trimmed().strip()
-        comment_line, _ = comment.pos_marker.source_position()
-        result = cls.parse_noqa(comment_content, comment_line, reference_map)
-        if isinstance(result, SQLParseError):
-            result.segment = comment
-        return result
-
-    @classmethod
-    def extract_ignore_mask_tree(
-        cls,
-        tree: BaseSegment,
-        reference_map: Dict[str, Set[str]],
-    ) -> Tuple[List[NoQaDirective], List[SQLBaseError]]:
-        """Look for inline ignore comments and return NoQaDirectives."""
-        ignore_buff: List[NoQaDirective] = []
-        violations: List[SQLBaseError] = []
-        for comment in tree.recursive_crawl("comment"):
-            if comment.is_type("inline_comment"):
-                ignore_entry = cls.extract_ignore_from_comment(comment, reference_map)
-                if isinstance(ignore_entry, SQLParseError):
-                    violations.append(ignore_entry)
-                elif ignore_entry:
-                    ignore_buff.append(ignore_entry)
-        if ignore_buff:
-            linter_logger.info("Parsed noqa directives from file: %r", ignore_buff)
-        return ignore_buff, violations
-
-    @classmethod
-    def extract_ignore_mask_source(
-        cls,
-        source: str,
-        inline_comment_regex: RegexLexer,
-        reference_map: Dict[str, Set[str]],
-    ) -> Tuple[List[NoQaDirective], List[SQLBaseError]]:
-        """Look for inline ignore comments and return NoQaDirectives.
-
-        Very similar to extract_ignore_mask_tree(), but can be run on raw source
-        (i.e. does not require the code to have parsed successfully).
-        """
-        ignore_buff: List[NoQaDirective] = []
-        violations: List[SQLBaseError] = []
-        for idx, line in enumerate(source.split("\n")):
-            match = inline_comment_regex.search(line) if line else None
-            if match:
-                ignore_entry = cls.parse_noqa(
-                    line[match[0] : match[1]], idx + 1, reference_map
-                )
-                if isinstance(ignore_entry, SQLParseError):
-                    violations.append(ignore_entry)  # pragma: no cover
-                elif ignore_entry:
-                    ignore_buff.append(ignore_entry)
-        if ignore_buff:
-            linter_logger.info("Parsed noqa directives from file: %r", ignore_buff)
-        return ignore_buff, violations
-
-    @classmethod
     def lint_fix_parsed(
         cls,
         tree: BaseSegment,
         config: FluffConfig,
         rule_pack: RulePack,
         fix: bool = False,
         fname: Optional[str] = None,
         templated_file: Optional[TemplatedFile] = None,
         formatter: Any = None,
-    ) -> Tuple[BaseSegment, List[SQLBaseError], List[NoQaDirective], RuleTimingsType]:
+    ) -> Tuple[BaseSegment, List[SQLBaseError], Optional[IgnoreMask], RuleTimingsType]:
         """Lint and optionally fix a tree object."""
         # Keep track of the linting errors on the very first linter pass. The
         # list of issues output by "lint" and "fix" only includes issues present
         # in the initial SQL code, EXCLUDING any issues that may be created by
         # the fixes themselves.
         initial_linting_errors = []
         # A placeholder for the fixes we had on the previous loop
@@ -520,20 +384,18 @@
 
         # Dispatch the output for the lint header
         if formatter:
             formatter.dispatch_lint_header(fname, sorted(rule_pack.codes()))
 
         # Look for comment segments which might indicate lines to ignore.
         if not config.get("disable_noqa"):
-            ignore_buff, ivs = cls.extract_ignore_mask_tree(
-                tree, rule_pack.reference_map
-            )
+            ignore_mask, ivs = IgnoreMask.from_tree(tree, rule_pack.reference_map)
             initial_linting_errors += ivs
         else:
-            ignore_buff = []
+            ignore_mask = None
 
         save_tree = tree
         # There are two phases of rule running.
         # 1. The main loop is for most rules. These rules are assumed to
         # interact and cause a cascade of fixes requiring multiple passes.
         # These are run the `runaway_limit` number of times (default 10).
         # 2. The post loop is for post-processing rules, not expected to trigger
@@ -548,15 +410,15 @@
                 rules_this_phase = [
                     rule for rule in rule_pack.rules if rule.lint_phase == phase
                 ]
             else:
                 rules_this_phase = rule_pack.rules
             for loop in range(loop_limit if phase == "main" else 2):
 
-                def is_first_linter_pass():
+                def is_first_linter_pass() -> bool:
                     return phase == phases[0] and loop == 0
 
                 # Additional newlines are to assist in scanning linting loops
                 # during debugging.
                 linter_logger.info(
                     f"\n\nEntering linter phase {phase}, loop {loop+1}/{loop_limit}\n"
                 )
@@ -595,15 +457,15 @@
                     # the "anchor", the segment to look for either to edit or to
                     # insert BEFORE. The second is the element to insert or create.
                     linting_errors, _, fixes, _ = crawler.crawl(
                         tree,
                         dialect=config.get("dialect_obj"),
                         fix=fix,
                         templated_file=templated_file,
-                        ignore_mask=ignore_buff,
+                        ignore_mask=ignore_mask,
                         fname=fname,
                         config=config,
                     )
                     if is_first_linter_pass():
                         initial_linting_errors += linting_errors
 
                     if fix and fixes:
@@ -618,16 +480,16 @@
                                 "fixes with the same anchor. This is only "
                                 "supported for create_before+create_after, so "
                                 "the fixes will not be applied. "
                             )
                             for uuid, info in anchor_info.items():
                                 if not info.is_valid:
                                     message += f"\n{uuid}:"
-                                    for fix in info.fixes:
-                                        message += f"\n    {fix}"
+                                    for _fix in info.fixes:
+                                        message += f"\n    {_fix}"
                             cls._report_conflicting_fixes_same_anchor(message)
                             for lint_result in linting_errors:
                                 lint_result.fixes = []
                         elif fixes == last_fixes:  # pragma: no cover
                             # If we generate the same fixes two times in a row,
                             # that means we're in a loop, and we want to stop.
                             # (Fixes should address issues, hence different
@@ -696,44 +558,44 @@
                         if isinstance(violation, SQLLintError):
                             violation.fixes = []
 
                     # Return the original parse tree, before any fixes were applied.
                     # Reason: When the linter hits the loop limit, the file is often
                     # messy, e.g. some of the fixes were applied repeatedly, possibly
                     # other weird things. We don't want the user to see this junk!
-                    return save_tree, initial_linting_errors, ignore_buff, rule_timings
+                    return save_tree, initial_linting_errors, ignore_mask, rule_timings
 
         if config.get("ignore_templated_areas", default=True):
             initial_linting_errors = cls.remove_templated_errors(initial_linting_errors)
 
         linter_logger.info("\n###\n#\n# {}\n#\n###".format("Fixed Tree:"))
         linter_logger.info("\n" + tree.stringify())
 
-        return tree, initial_linting_errors, ignore_buff, rule_timings
+        return tree, initial_linting_errors, ignore_mask, rule_timings
 
     @classmethod
     def lint_parsed(
         cls,
         parsed: ParsedString,
         rule_pack: RulePack,
         fix: bool = False,
         formatter: Any = None,
         encoding: str = "utf8",
-    ):
+    ) -> LintedFile:
         """Lint a ParsedString and return a LintedFile."""
         violations = parsed.violations
         time_dict = parsed.time_dict
         tree: Optional[BaseSegment]
         if parsed.tree:
             t0 = time.monotonic()
             linter_logger.info("LINTING (%s)", parsed.fname)
             (
                 tree,
                 initial_linting_errors,
-                ignore_buff,
+                ignore_mask,
                 rule_timings,
             ) = cls.lint_fix_parsed(
                 parsed.tree,
                 config=parsed.config,
                 rule_pack=rule_pack,
                 fix=fix,
                 fname=parsed.fname,
@@ -745,22 +607,22 @@
 
             # We're only going to return the *initial* errors, rather
             # than any generated during the fixing cycle.
             violations += initial_linting_errors
         else:
             # If no parsed tree, set to None
             tree = None
-            ignore_buff = []
+            ignore_mask = None
             rule_timings = []
             if not parsed.config.get("disable_noqa"):
                 # Templating and/or parsing have failed. Look for "noqa"
                 # comments (the normal path for identifying these comments
                 # requires access to the parse tree, and because of the failure,
                 # we don't have a parse tree).
-                ignore_buff, ignore_violations = cls.extract_ignore_mask_source(
+                ignore_mask, ignore_violations = IgnoreMask.from_source(
                     parsed.source_str,
                     [
                         lm
                         for lm in parsed.config.get("dialect_obj").lexer_matchers
                         if lm.name == "inline_comment"
                     ][0],
                     rule_pack.reference_map,
@@ -774,23 +636,26 @@
 
         linted_file = LintedFile(
             parsed.fname,
             # Deduplicate violations
             LintedFile.deduplicate_in_source_space(violations),
             FileTimings(time_dict, rule_timings),
             tree,
-            ignore_mask=ignore_buff,
+            ignore_mask=ignore_mask,
             templated_file=parsed.templated_file,
             encoding=encoding,
         )
 
         # This is the main command line output from linting.
         if formatter:
             formatter.dispatch_file_violations(
-                parsed.fname, linted_file, only_fixable=fix
+                parsed.fname,
+                linted_file,
+                only_fixable=fix,
+                warn_unused_ignores=parsed.config.get("warn_unused_ignores"),
             )
 
         # Safety flag for unset dialects
         if linted_file.get_violations(
             fixable=True if fix else None, types=SQLParseError
         ):
             if formatter:  # pragma: no cover TODO?
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/linting_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,26 @@
     @staticmethod
     def sum_dicts(d1: Dict[str, Any], d2: Dict[str, Any]) -> Dict[str, Any]:
         """Take the keys of two dictionaries and add them."""
         keys = set(d1.keys()) | set(d2.keys())
         return {key: d1.get(key, 0) + d2.get(key, 0) for key in keys}
 
     @staticmethod
-    def combine_dicts(*d: dict) -> dict:
+    def combine_dicts(*d: Dict[str, Any]) -> Dict[str, Any]:
         """Take any set of dictionaries and combine them."""
         dict_buffer: dict = {}
         for dct in d:
             dict_buffer.update(dct)
         return dict_buffer
 
     def add(self, path: LintedDir) -> None:
         """Add a new `LintedDir` to this result."""
         self.paths.append(path)
 
-    def stop_timer(self):
+    def stop_timer(self) -> None:
         """Stop the linting timer."""
         self.total_time = time.monotonic() - self._start_time
 
     @overload
     def check_tuples(
         self, by_path: Literal[False]
     ) -> List[CheckTuple]:  # pragma: no cover
@@ -103,22 +103,22 @@
                 tuple_buffer += path.check_tuples()
             return tuple_buffer
 
     def num_violations(self, **kwargs) -> int:
         """Count the number of violations in the result."""
         return sum(path.num_violations(**kwargs) for path in self.paths)
 
-    def get_violations(self, **kwargs):
+    def get_violations(self, **kwargs) -> list:
         """Return a list of violations in the result."""
         buff = []
         for path in self.paths:
             buff += path.get_violations(**kwargs)
         return buff
 
-    def violation_dict(self, **kwargs):
+    def violation_dict(self, **kwargs) -> dict:
         """Return a dict of paths and violations."""
         return self.combine_dicts(
             *(path.violation_dict(**kwargs) for path in self.paths)
         )
 
     def stats(self) -> Dict[str, Any]:
         """Return a stats dictionary of this result."""
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.2.0/src/sqlfluff/core/linter/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 import sys
 import traceback
 from typing import Callable, List, Tuple, Iterator
 
 from sqlfluff.core import FluffConfig, Linter
 from sqlfluff.core.errors import SQLFluffSkipFile
 from sqlfluff.core.linter import LintedFile, RenderedFile
+from sqlfluff.core.plugin.host import is_main_process
 
 linter_logger: logging.Logger = logging.getLogger("sqlfluff.linter")
 
 
 class BaseRunner(ABC):
     """Base runner class."""
 
     def __init__(
         self,
-        linter,
-        config,
-    ):
+        linter: Linter,
+        config: FluffConfig,
+    ) -> None:
         self.linter = linter
         self.config = config
 
     pass_formatter = True
 
     def iter_rendered(self, fnames: List[str]) -> Iterator[Tuple[str, RenderedFile]]:
         """Iterate through rendered files ready for linting."""
@@ -73,24 +74,24 @@
             )
 
     def run(self, fnames: List[str], fix: bool):
         """Run linting on the specified list of files."""
         raise NotImplementedError  # pragma: no cover
 
     @classmethod
-    def _init_global(cls, config):
+    def _init_global(cls, config) -> None:
         """Initializes any global state.
 
         May be overridden by subclasses to apply global configuration, initialize
         logger state in child processes, etc.
         """
         pass
 
     @staticmethod
-    def _handle_lint_path_exception(fname, e):
+    def _handle_lint_path_exception(fname, e) -> None:
         if isinstance(e, IOError):
             # IOErrors are caught in commands.py, so propagate it
             raise (e)  # pragma: no cover
         linter_logger.warning(
             f"""Unable to lint {fname} due to an internal error. \
 Please report this as an issue with your query's contents and stacktrace below!
 To hide this warning, add the failing file to .sqlfluffignore
@@ -117,15 +118,15 @@
 
     POOL_TYPE: Callable
     MAP_FUNCTION_NAME: str
     # Don't pass the formatter in a parallel world, they
     # don't pickle well.
     pass_formatter = False
 
-    def __init__(self, linter, config, processes):
+    def __init__(self, linter, config, processes) -> None:
         super().__init__(linter, config)
         self.processes = processes
 
     def run(self, fnames: List[str], fix: bool):
         """Parallel implementation.
 
         Note that the partials are generated one at a time then
@@ -149,15 +150,20 @@
                             lint_result.reraise()
                         except Exception as e:
                             self._handle_lint_path_exception(lint_result.fname, e)
                     else:
                         # It's a LintedDir.
                         if self.linter.formatter:
                             self.linter.formatter.dispatch_file_violations(
-                                lint_result.path, lint_result, only_fixable=fix
+                                lint_result.path,
+                                lint_result,
+                                only_fixable=fix,
+                                warn_unused_ignores=self.linter.config.get(
+                                    "warn_unused_ignores"
+                                ),
                             )
                         yield lint_result
             except KeyboardInterrupt:  # pragma: no cover
                 # On keyboard interrupt (Ctrl-C), terminate the workers.
                 # Notify the user we've received the signal and are cleaning up,
                 # in case it takes awhile.
                 print("Received keyboard interrupt. Cleaning up and shutting down...")
@@ -172,14 +178,20 @@
             return partial()
         # Capture any exceptions and return as delayed exception to handle
         # in the main thread.
         except Exception as e:
             return DelayedException(e, fname=fname)
 
     @classmethod
+    def _init_global(cls, config) -> None:  # pragma: no cover
+        """For the parallel runners indicate that we're not in the main thread."""
+        is_main_process.set(False)
+        super()._init_global(config)
+
+    @classmethod
     def _create_pool(cls, *args, **kwargs):
         return cls.POOL_TYPE(*args, **kwargs)
 
     @classmethod
     def _map(cls, pool, *args, **kwargs):
         """Runs a class-appropriate version of the general map() function."""
         return getattr(pool, cls.MAP_FUNCTION_NAME)(*args, **kwargs)
@@ -188,15 +200,15 @@
 class MultiProcessRunner(ParallelRunner):
     """Runner that does parallel processing using multiple processes."""
 
     POOL_TYPE = multiprocessing.Pool
     MAP_FUNCTION_NAME = "imap_unordered"
 
     @classmethod
-    def _init_global(cls, config):  # pragma: no cover
+    def _init_global(cls, config) -> None:  # pragma: no cover
         super()._init_global(config)
 
         # Disable signal handling in the child processes to let the parent
         # control all KeyboardInterrupt handling (Control C). This is
         # necessary in order for keyboard interrupts to exit quickly and
         # cleanly. Adapted from this post:
         # https://stackoverflow.com/questions/11312525/catch-ctrlc-sigint-and-exit-multiprocesses-gracefully-in-python
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,63 +5,92 @@
 
 The context acts as a way of keeping track of state, references
 to common configuration and dialects, logging and also the parse
 and match depth of the current operation.
 """
 
 from collections import defaultdict
+from contextlib import contextmanager
 import logging
 import uuid
-from typing import Optional, TYPE_CHECKING, Dict
+from typing import Iterator, Optional, TYPE_CHECKING, Dict, Any, Tuple, Sequence
 
 if TYPE_CHECKING:  # pragma: no cover
     from sqlfluff.core.parser.match_result import MatchResult
+    from sqlfluff.core.dialects.base import Dialect, ExpandedDialectElementType
+    from sqlfluff.core.config import FluffConfig
 
 # Get the parser logger
 parser_logger = logging.getLogger("sqlfluff.parser")
 
 
-class RootParseContext:
+class ParseContext:
     """Object to handle the context at hand during parsing.
 
-    The root context holds the persistent config which stays
-    consistent through a parsing operation. It also produces
-    the individual contexts that are used at different layers.
+    Holds two tiers of references.
+    1. Persistent config, like references to the dialect or
+       the current verbosity and logger.
+    2. Stack config, like the parse and match depth.
+
+    The manipulation of the stack config is done using a context
+    manager and layered config objects inside the context.
+
+    NOTE: We use context managers here to avoid _copying_
+    the context, just to mutate it safely. This is significantly
+    more performant than the copy operation, but does require some
+    care to use properly.
 
-    Each ParseContext maintains a reference to the RootParseContext
-    which created it so that it can refer to config within it.
+    When fetching elements from the context, we first look
+    at the top level stack config object and the persistent
+    config values (stored as attributes of the ParseContext
+    itself).
     """
 
-    def __init__(self, dialect, indentation_config=None, recurse=True):
-        """Store persistent config objects."""
+    def __init__(
+        self,
+        dialect: "Dialect",
+        indentation_config: Optional[Dict[str, Any]] = None,
+        recurse: bool = True,
+    ) -> None:
         self.dialect = dialect
         self.recurse = recurse
         # Indentation config is used by Indent and Dedent and used to control
         # the intended indentation of certain features. Specifically it is
         # used in the Conditional grammar.
         self.indentation_config = indentation_config or {}
-        # Initialise the denylist
-        self.denylist = ParseDenylist()
         # This is the logger that child objects will latch onto.
         self.logger = parser_logger
         # A uuid for this parse context to enable cache invalidation
         self.uuid = uuid.uuid4()
         # A dict for parse caching. This is reset for each file,
         # but persists for the duration of an individual file parse.
-        self._parse_cache = {}
+        self._parse_cache: Dict[Tuple[Any, ...], "MatchResult"] = {}
         # A dictionary for keeping track of some statistics on parsing
         # for performance optimisation.
         # Focused around BaseGrammar._longest_trimmed_match().
         # Initialise only with "next_counts", the rest will be int
         # and are dealt with in .increment().
-        self.parse_stats = {"next_counts": defaultdict(int)}
+        self.parse_stats: Dict[str, Any] = {"next_counts": defaultdict(int)}
+        # The following attributes are only accessible via a copy
+        # and not in the init method.
+        self.match_segment: Optional[str] = None
+        self.match_depth = 0
+        self.parse_depth = 0
+        # self.terminators is a tuple to afford some level of isolation
+        # and protection from edits to outside the context. This introduces
+        # a little more overhead than a list, but we manage this by only
+        # copying it when necessary.
+        # NOTE: Includes inherited parent terminators.
+        self.terminators: Tuple["ExpandedDialectElementType", ...] = ()
 
     @classmethod
-    def from_config(cls, config, **overrides: Dict[str, bool]) -> "RootParseContext":
-        """Construct a `RootParseContext` from a `FluffConfig`."""
+    def from_config(
+        cls, config: "FluffConfig", **overrides: Dict[str, bool]
+    ) -> "ParseContext":
+        """Construct a `ParseContext` from a `FluffConfig`."""
         indentation_config = config.get_section("indentation") or {}
         try:
             indentation_config = {k: bool(v) for k, v in indentation_config.items()}
         except TypeError:  # pragma: no cover
             raise TypeError(
                 "One of the configuration keys in the `indentation` section is not "
                 "True or False: {!r}".format(indentation_config)
@@ -73,191 +102,125 @@
         )
         # Set any overrides in the creation
         for key in overrides:
             if overrides[key] is not None:
                 setattr(ctx, key, overrides[key])
         return ctx
 
-    def __enter__(self):
-        """Enter into the context.
-
-        Here we return a basic ParseContext with initial values,
-        initialising just the recurse value.
-
-        Note: The RootParseContext is usually entered at the beginning
-        of the parse operation as follows::
-
-            with RootParseContext.from_config(...) as ctx:
-                parsed = file_segment.parse(parse_context=ctx)
-        """
-        return ParseContext(root_ctx=self, recurse=self.recurse)
-
-    def __exit__(self, type, value, traceback):
-        """Clear up the context."""
-        pass
-
-
-class ParseContext:
-    """Object to handle the context at hand during parsing.
-
-    Holds two tiers of references.
-    1. Persistent config, like references to the dialect or
-       the current verbosity and logger.
-    2. Stack config, like the parse and match depth.
-
-    The manipulation of the stack config is done using a context
-    manager and layered config objects inside the context.
-
-    When fetching elements from the context, we first look
-    at the top level stack config object and the persistent
-    config values (stored as attributes of the ParseContext
-    itself).
-    """
-
-    # We create and destroy many ParseContexts, so we limit the slots
-    # to improve performance.
-    __slots__ = [
-        "match_depth",
-        "parse_depth",
-        "match_segment",
-        "recurse",
-        "terminators",
-        "_root_ctx",
-    ]
-
-    def __init__(self, root_ctx, recurse=True):
-        self._root_ctx = root_ctx
-        self.recurse = recurse
-        # The following attributes are only accessible via a copy
-        # and not in the init method.
-        self.match_segment = None
-        self.match_depth = 0
-        self.parse_depth = 0
-        self.terminators = []  # NOTE: Includes inherited parent terminators.
-
-    def __getattr__(self, name):
-        """If the attribute doesn't exist on this, revert to the root."""
+    def _set_terminators(
+        self,
+        clear_terminators: bool = False,
+        push_terminators: Optional[Sequence["ExpandedDialectElementType"]] = None,
+    ) -> Tuple[int, Tuple["ExpandedDialectElementType", ...]]:
+        _appended = 0
+        # Retain a reference to the original terminators.
+        _terminators = self.terminators
+        # Note: only need to reset if clear _and not already clear_.
+        if clear_terminators and self.terminators:
+            # NOTE: It's really important that we .copy() on the way in, because
+            # we don't know what else has a reference to the input list, and
+            # we rely a lot in this code on having full control over the
+            # list of terminators.
+            self.terminators = tuple(push_terminators) if push_terminators else ()
+        elif push_terminators:
+            # Yes, inefficient for now.
+            for terminator in push_terminators:
+                if terminator not in self.terminators:
+                    self.terminators += (terminator,)
+                    _appended += 1
+        return _appended, _terminators
+
+    def _reset_terminators(
+        self,
+        appended: int,
+        terminators: Tuple["ExpandedDialectElementType", ...],
+        clear_terminators: bool = False,
+    ) -> None:
+        # If we totally reset them, just reinstate the old object.
+        if clear_terminators:
+            self.terminators = terminators
+        # If we didn't, then trim any added ones.
+        # NOTE: Because we dedupe, just because we had push_terminators
+        # doesn't mean any of them actually got added here - we only trim
+        # the number that actually got appended.
+        elif appended:
+            # Trim back to original length.
+            self.terminators = self.terminators[:-appended]
+
+    @contextmanager
+    def deeper_match(
+        self,
+        clear_terminators: bool = False,
+        push_terminators: Optional[Sequence["ExpandedDialectElementType"]] = None,
+    ) -> Iterator["ParseContext"]:
+        """Increment match depth."""
+        self.match_depth += 1
+        _append, _terms = self._set_terminators(clear_terminators, push_terminators)
         try:
-            return getattr(self._root_ctx, name)
-        except AttributeError:  # pragma: no cover
-            raise AttributeError(
-                "Attribute {!r} not found in {!r} or {!r}".format(
-                    name, type(self).__name__, type(self._root_ctx).__name__
-                )
+            yield self
+        finally:
+            self._reset_terminators(
+                _append, _terms, clear_terminators=clear_terminators
             )
+            self.match_depth -= 1
 
-    def _copy(self):
-        """Mimic the copy.copy() method but restrict only to local vars."""
-        ctx = self.__class__(root_ctx=self._root_ctx)
-        for key in self.__slots__:
-            if key == "terminators":
-                # For terminators, make sure we actually copy the list.
-                # This makes sure we don't keep a reference to the parent list.
-                setattr(ctx, key, getattr(self, key).copy())
-            else:
-                setattr(ctx, key, getattr(self, key))
-        return ctx
-
-    def __enter__(self):
-        """Enter into the context.
-
-        For the ParseContext, this just returns itself, because
-        we already have the right kind of object.
-        """
-        return self
-
-    def __exit__(self, type, value, traceback):
-        """Clear up the context."""
-        pass
-
-    def deeper_match(self):
-        """Return a copy with an incremented match depth."""
-        ctx = self._copy()
-        ctx.match_depth += 1
-        return ctx
-
-    def deeper_parse(self):
-        """Return a copy with an incremented parse depth."""
-        ctx = self._copy()
-        if not isinstance(ctx.recurse, bool):  # pragma: no cover TODO?
-            ctx.recurse -= 1
-        ctx.parse_depth += 1
-        ctx.match_depth = 0
-        # Clear terminators here. Inner parsing shouldn't inherit terminators.
-        ctx.clear_terminators()
-        return ctx
+    @contextmanager
+    def deeper_parse(self) -> Iterator["ParseContext"]:
+        """Increment parse depth."""
+        _match_depth = self.match_depth
+        self.parse_depth += 1
+        self.match_depth = 0
+        _append, _terms = self._set_terminators(clear_terminators=True)
+        if not isinstance(self.recurse, bool):  # pragma: no cover TODO?
+            self.recurse -= 1
+        try:
+            yield self
+        finally:
+            self.parse_depth -= 1
+            self.match_depth = _match_depth
+            if not isinstance(self.recurse, bool):  # pragma: no cover TODO?
+                self.recurse += 1
+            self._reset_terminators(_append, _terms, clear_terminators=True)
 
-    def may_recurse(self):
+    def may_recurse(self) -> bool:
         """Return True if allowed to recurse."""
         return self.recurse > 1 or self.recurse is True
 
-    def matching_segment(self, name):
+    @contextmanager
+    def matching_segment(
+        self,
+        name: str,
+        clear_terminators: bool = False,
+        push_terminators: Optional[Sequence["ExpandedDialectElementType"]] = None,
+    ) -> Iterator["ParseContext"]:
         """Set the name of the current matching segment.
 
         NB: We don't reset the match depth here.
         """
-        ctx = self._copy()
-        ctx.match_segment = name
-        return ctx
+        old_name = self.match_segment
+        self.match_segment = name
+        _append, _terms = self._set_terminators(clear_terminators, push_terminators)
+        try:
+            yield self
+        finally:
+            self._reset_terminators(_append, _terms, clear_terminators)
+            # Reset back to old name
+            self.match_segment = old_name
 
     def check_parse_cache(
-        self, loc_key: tuple, matcher_key: str
+        self, loc_key: Tuple[Any, ...], matcher_key: str
     ) -> Optional["MatchResult"]:
         """Check against the parse cache for a pre-existing match.
 
         If no match is found in the cache, this returns None.
         """
-        return self._root_ctx._parse_cache.get((loc_key, matcher_key))
+        return self._parse_cache.get((loc_key, matcher_key))
 
-    def put_parse_cache(self, loc_key: tuple, matcher_key: str, match: "MatchResult"):
+    def put_parse_cache(
+        self, loc_key: Tuple[Any, ...], matcher_key: str, match: "MatchResult"
+    ) -> None:
         """Store a match in the cache for later retrieval."""
-        self._root_ctx._parse_cache[(loc_key, matcher_key)] = match
+        self._parse_cache[(loc_key, matcher_key)] = match
 
     def increment(self, key: str, default: int = 0) -> None:
         """Increment one of the parse stats by name."""
-        self._root_ctx.parse_stats[key] = self._root_ctx.parse_stats.get(key, 0) + 1
-
-    def push_terminators(self, new_terminators: list) -> None:
-        """Push any new terminators onto the stack."""
-        # Yes, inefficient for now.
-        for term in new_terminators:
-            if term not in self.terminators:
-                self.terminators.append(term)
-
-    def clear_terminators(self) -> None:
-        """Clear any inherited terminators from this context."""
-        self.terminators = []
-
-
-class ParseDenylist:
-    """Acts as a cache to stop unnecessary matching."""
-
-    def __init__(self):
-        self._denylist_struct = {}
-
-    def _hashed_version(self):  # pragma: no cover TODO?
-        return {
-            k: {hash(e) for e in self._denylist_struct[k]}
-            for k in self._denylist_struct
-        }
-
-    def check(self, seg_name, seg_tuple):
-        """Check this seg_tuple against this seg_name.
-
-        Has this seg_tuple already been matched
-        unsuccessfully against this segment name.
-        """
-        if seg_name in self._denylist_struct:  # pragma: no cover TODO?
-            if seg_tuple in self._denylist_struct[seg_name]:
-                return True
-        return False
-
-    def mark(self, seg_name, seg_tuple):
-        """Mark this seg_tuple as not a match with this seg_name."""
-        if seg_name in self._denylist_struct:
-            self._denylist_struct[seg_name].add(seg_tuple)
-        else:
-            self._denylist_struct[seg_name] = {seg_tuple}
-
-    def clear(self):
-        """Clear the denylist struct."""
-        self._denylist_struct = {}
+        self.parse_stats[key] = self.parse_stats.get(key, 0) + 1
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """AnyNumberOf and OneOf."""
 
 from typing import List, Optional, Tuple, Set
 
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.parser.grammar.base import (
     BaseGrammar,
-    MatchableType,
     cached_method_for_parse_context,
+    MatchableType,
 )
+from sqlfluff.core.parser.grammar.types import SimpleHintType
 from sqlfluff.core.parser.grammar.sequence import Sequence, Bracketed
 from sqlfluff.core.parser.helpers import trim_non_code_segments
 from sqlfluff.core.parser.match_logging import parse_match_logging
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.segments import BaseSegment, allow_ephemeral
 
 
 class AnyNumberOf(BaseGrammar):
     """A more configurable version of OneOf."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         self.max_times = kwargs.pop("max_times", None)
         self.min_times = kwargs.pop("min_times", 0)
         self.max_times_per_element = kwargs.pop("max_times_per_element", None)
         # Any patterns to _prevent_ a match.
         self.exclude = kwargs.pop("exclude", None)
         # The intent here is that if we match something, and then the _next_
         # item is one of these, we can safely conclude it's a "total" match.
         # In those cases, we return early without considering more options.
         self.terminators = kwargs.pop("terminators", None)
         self.reset_terminators = kwargs.pop("reset_terminators", False)
         super().__init__(*args, **kwargs)
 
     @cached_method_for_parse_context
-    def simple(self, parse_context: ParseContext, crumbs: Optional[List[str]] = None):
+    def simple(
+        self, parse_context: ParseContext, crumbs: Optional[List[str]] = None
+    ) -> SimpleHintType:
         """Does this matcher support a uppercase hash matching route?
 
         AnyNumberOf does provide this, as long as *all* the elements *also* do.
         """
         simple_buff = [
             opt.simple(parse_context=parse_context, crumbs=crumbs)
             for opt in self._elements
@@ -157,19 +160,17 @@
         # the raw segments within it.
         available_options = self._prune_options(segments, parse_context=parse_context)
 
         # If we've pruned all the options, return unmatched (with some logging).
         if not available_options:
             return MatchResult.from_unmatched(segments), None
 
-        with parse_context.deeper_match() as ctx:
-            if self.reset_terminators:
-                ctx.clear_terminators()
-            if self.terminators:
-                ctx.push_terminators(self.terminators)
+        with parse_context.deeper_match(
+            clear_terminators=self.reset_terminators, push_terminators=self.terminators
+        ) as ctx:
             match, matched_option = self._longest_trimmed_match(
                 segments,
                 available_options,
                 parse_context=ctx,
                 trim_noncode=False,
             )
 
@@ -264,32 +265,32 @@
 class OneOf(AnyNumberOf):
     """Match any of the elements given once.
 
     If it matches multiple, it returns the longest, and if any are the same
     length it returns the first (unless we explicitly just match first).
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, max_times=1, min_times=1, **kwargs)
 
 
 class OptionallyBracketed(OneOf):
     """Hybrid of Bracketed and Sequence: allows brackets but they aren't required.
 
     NOTE: This class is greedy on brackets so if they *can* be claimed, then
     they will be.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(
             Bracketed(*args),
             # In the case that there is only one argument, no sequence is required.
             args[0] if len(args) == 1 else Sequence(*args),
             **kwargs,
         )
 
 
 class AnySetOf(AnyNumberOf):
     """Match any number of the elements but each element can only be matched once."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, max_times_per_element=1, **kwargs)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """Base grammar, Ref, Anything and Nothing."""
 
 import copy
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Optional, Union, Type, Tuple, Any, cast
+from typing import (
+    TYPE_CHECKING,
+    List,
+    Optional,
+    Union,
+    Type,
+    Tuple,
+    Any,
+    cast,
+)
 from uuid import uuid4
 
 from sqlfluff.core.errors import SQLParseError
+from sqlfluff.core.parser.grammar.types import SimpleHintType
 from sqlfluff.core.string_helpers import curtail_string
 
 from sqlfluff.core.parser.segments import BaseSegment, BracketedSegment, allow_ephemeral
 from sqlfluff.core.parser.helpers import trim_non_code_segments
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_logging import (
     parse_match_logging,
@@ -17,21 +27,22 @@
 )
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.matchable import Matchable
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.parser.parsers import BaseParser
 
 # Either a Matchable (a grammar or parser) or a Segment CLASS
+
 MatchableType = Union[Matchable, Type[BaseSegment]]
 
 if TYPE_CHECKING:
     from sqlfluff.core.dialects.base import Dialect  # pragma: no cover
 
 
-def first_trimmed_raw(seg):
+def first_trimmed_raw(seg: BaseSegment) -> str:
     """Trim whitespace off a whole element raw.
 
     Used as a helper function in BaseGrammar._look_ahead_match.
 
     For existing compound segments, we should assume that within
     that segment, things are internally consistent, that means
     rather than enumerating all the individual segments of a longer
@@ -56,15 +67,15 @@
     This is used in BaseGrammar._bracket_sensitive_look_ahead_match but
     defined here for type checking.
     """
 
     bracket: BaseSegment
     segments: Tuple[BaseSegment, ...]
 
-    def to_segment(self, end_bracket):
+    def to_segment(self, end_bracket) -> BracketedSegment:
         """Turn the contained segments into a bracketed segment."""
         return BracketedSegment(
             segments=self.segments,
             start_bracket=(self.bracket,),
             end_bracket=end_bracket,
         )
 
@@ -82,15 +93,15 @@
     def wrapped_method(self, parse_context: ParseContext, **kwargs):
         """Cache the output of the method against a given parse context.
 
         Note: kwargs are not taken into account in the caching, but
         for the current use case of dependency loop debugging that's
         ok.
         """
-        cache_tuple: Tuple = self.__dict__.get(cache_key, (None, None))
+        cache_tuple: tuple = self.__dict__.get(cache_key, (None, None))
         # Do we currently have a cached value?
         if cache_tuple[0] == parse_context.uuid:
             return cache_tuple[1]
         # Generate a new value, cache it and return
         result = func(self, parse_context=parse_context, **kwargs)
         self.__dict__[cache_key] = (parse_context.uuid, result)
         return result
@@ -139,15 +150,15 @@
 
     def __init__(
         self,
         *args: Union[MatchableType, str],
         allow_gaps=True,
         optional=False,
         ephemeral_name=None,
-    ):
+    ) -> None:
         """Deal with kwargs common to all grammars.
 
         Args:
             *args: Any number of elements which because the subjects
                 of this grammar. Optionally these elements may also be
                 string references to elements rather than the Matchable
                 elements themselves.
@@ -175,15 +186,15 @@
             for elem in args:
                 self._elements.append(self._resolve_ref(elem))
         else:
             self._elements = list(args)
 
         # Now we deal with the standard kwargs
         self.allow_gaps = allow_gaps
-        self.optional = optional
+        self.optional: bool = optional
         # ephemeral_name is a flag to indicate whether we need to make an
         # EphemeralSegment class. This is effectively syntactic sugar
         # to allow us to avoid specifying a EphemeralSegment directly in a dialect.
         # If this is the case, the actual segment construction happens in the
         # match_wrapper.
         self.ephemeral_name = ephemeral_name
         # Generate a cache key
@@ -192,46 +203,50 @@
     def cache_key(self) -> str:
         """Get the cache key for this grammar.
 
         For grammars these are unique per-instance.
         """
         return self._cache_key
 
-    def is_optional(self):
+    def is_optional(self) -> bool:
         """Return whether this segment is optional.
 
         The optional attribute is set in the __init__ method.
         """
         return self.optional
 
     @match_wrapper()
     @allow_ephemeral
-    def match(self, segments: Tuple[BaseSegment, ...], parse_context: ParseContext):
+    def match(
+        self, segments: Tuple[BaseSegment, ...], parse_context: ParseContext
+    ) -> MatchResult:
         """Match a list of segments against this segment.
 
         Matching can be done from either the raw or the segments.
         This raw function can be overridden, or a grammar defined
         on the underlying class.
         """
         raise NotImplementedError(
             f"{self.__class__.__name__} has no match function implemented"
         )  # pragma: no cover
 
     @cached_method_for_parse_context
-    def simple(self, parse_context: ParseContext, crumbs=None):
+    def simple(
+        self, parse_context: ParseContext, crumbs: Optional[List[str]] = None
+    ) -> SimpleHintType:
         """Does this matcher support a lowercase hash matching route?"""
         return None
 
     @classmethod
     def _longest_trimmed_match(
         cls,
         segments: Tuple[BaseSegment, ...],
         matchers: List[MatchableType],
         parse_context: ParseContext,
-        trim_noncode=True,
+        trim_noncode: bool = True,
     ) -> Tuple[MatchResult, Optional[MatchableType]]:
         """Return longest match from a selection of matchers.
 
         Prioritise the first match, and if multiple match at the same point the longest.
         If two matches of the same length match at the same time, then it's the first in
         the iterable of matchers.
 
@@ -247,15 +262,15 @@
         # NOTE: The use of terminators is only available via the context.
         # They are set in that way to allow appropriate inheritance rather
         # than only being used in a per-grammar basis.
         if parse_context.terminators:
             parse_context.increment("ltm_calls_w_ctx_terms")
             terminators = parse_context.terminators
         else:
-            terminators = []
+            terminators = ()
 
         # Have we been passed an empty list?
         if len(segments) == 0:  # pragma: no cover
             return MatchResult.from_empty(), None
 
         # If gaps are allowed, trim the ends.
         if trim_noncode:
@@ -288,15 +303,15 @@
                     "HIT",
                     parse_context=parse_context,
                     cache_hit=matcher.__class__.__name__,
                     cache_key=matcher_key,
                 )
             else:
                 # Match fresh if no cache hit
-                res_match = matcher.match(segments, parse_context=parse_context)
+                res_match = matcher.match(segments, parse_context)
                 # Cache it for later to for performance.
                 parse_context.put_parse_cache(loc_key, matcher_key, res_match)
 
             # By here we know that it's a MatchResult
             res_match = cast(MatchResult, res_match)
 
             if res_match.is_complete():
@@ -328,15 +343,15 @@
                         break
                     elif terminators:
                         _, segs, _ = trim_non_code_segments(
                             best_match[0].unmatched_segments
                         )
                         for terminator in terminators:
                             terminator_match: MatchResult = terminator.match(
-                                segs, parse_context=parse_context
+                                segs, parse_context
                             )
 
                             if terminator_match.matched_segments:
                                 terminated = True
                                 break
 
             if terminated:
@@ -722,27 +737,27 @@
             # - We reached the end with no open brackets.
             # - No match while outside a bracket stack.
             # - We found an unexpected end bracket before matching something
             # interesting. We return with the mutated segments so we can reuse any
             # bracket matching.
             return ((), MatchResult.from_unmatched(pre_seg_buff + seg_buff), None)
 
-    def __str__(self):  # pragma: no cover TODO?
+    def __str__(self) -> str:  # pragma: no cover TODO?
         return repr(self)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<{}: [{}]>".format(
             self.__class__.__name__,
             curtail_string(
                 ", ".join(curtail_string(repr(elem), 40) for elem in self._elements),
                 100,
             ),
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """Two grammars are equal if their elements and types are equal.
 
         NOTE: We use the equality_kwargs tuple on the class to define
         other kwargs which should also be checked so that things like
         "optional" is also taken into account in considering equality.
         """
         return (
@@ -830,29 +845,31 @@
 class Ref(BaseGrammar):
     """A kind of meta-grammar that references other grammars by name at runtime."""
 
     # We can't allow keyword refs here, because it doesn't make sense
     # and it also causes infinite recursion.
     allow_keyword_string_refs = False
 
-    def __init__(self, *args: str, **kwargs):
+    def __init__(self, *args: str, **kwargs) -> None:
         # Any patterns to _prevent_ a match.
         self.exclude = kwargs.pop("exclude", None)
         # The intent here is that if we match something, and then the _next_
         # item is one of these, we can safely conclude it's a "total" match.
         # In those cases, we return early without considering more options.
         # Terminators don't take effect directly within this grammar, but
         # the Ref grammar is an effective place to manage the terminators
         # inherited via the context.
         self.terminators = kwargs.pop("terminators", None)
         self.reset_terminators = kwargs.pop("reset_terminators", False)
         super().__init__(*args, **kwargs)
 
     @cached_method_for_parse_context
-    def simple(self, parse_context: ParseContext, crumbs: Optional[Tuple[str]] = None):
+    def simple(
+        self, parse_context: ParseContext, crumbs: Optional[Tuple[str]] = None
+    ) -> SimpleHintType:
         """Does this matcher support a uppercase hash matching route?
 
         A ref is simple, if the thing it references is simple.
         """
         ref = self._get_ref()
         if crumbs and ref in crumbs:  # pragma: no cover
             loop = " -> ".join(crumbs)
@@ -900,65 +917,40 @@
         self, segments: Tuple[BaseSegment, ...], parse_context: ParseContext
     ) -> "MatchResult":
         """Match a list of segments against this segment.
 
         Matching can be done from either the raw or the segments.
         This raw function can be overridden, or a grammar defined
         on the underlying class.
-
-        The match element of Ref, also implements the caching
-        using the parse_context `denylist` methods.
         """
         elem = self._get_elem(dialect=parse_context.dialect)
 
         # First if we have an *exclude* option, we should check that
         # which would prevent the rest of this grammar from matching.
         if self.exclude:
-            with parse_context.deeper_match() as ctx:
-                # NOTE: Not covered because `exclude` and `teminators` aren't
-                # currently used together in any dialect.
-                if self.reset_terminators:  # pragma: no cover
-                    ctx.clear_terminators()
-                if self.terminators:  # pragma: no cover
-                    ctx.push_terminators(self.terminators)
+            with parse_context.deeper_match(
+                clear_terminators=self.reset_terminators,
+                push_terminators=self.terminators,
+            ) as ctx:
                 if self.exclude.match(segments, parse_context=ctx):
                     return MatchResult.from_unmatched(segments)
 
-        # First check against the efficiency Cache.
-        # We rely on segments not being mutated within a given
-        # match cycle and so the ids should continue to refer to unchanged
-        # objects.
-        seg_tuple = (id(seg) for seg in segments)
-        self_name = self._get_ref()
-        if parse_context.denylist.check(self_name, seg_tuple):  # pragma: no cover TODO?
-            # This has been tried before.
-            parse_match_logging(
-                self.__class__.__name__,
-                "match",
-                "SKIP",
-                parse_context=parse_context,
-                v_level=3,
-                self_name=self_name,
-            )
-            return MatchResult.from_unmatched(segments)
-
         # Match against that. NB We're not incrementing the match_depth here.
         # References shouldn't really count as a depth of match.
-        with parse_context.matching_segment(self._get_ref()) as ctx:
-            if self.reset_terminators:
-                ctx.clear_terminators()
-            if self.terminators:
-                ctx.push_terminators(self.terminators)
-            resp = elem.match(segments=segments, parse_context=ctx)
-        if not resp:
-            parse_context.denylist.mark(self_name, seg_tuple)
+        with parse_context.matching_segment(
+            self._get_ref(),
+            clear_terminators=self.reset_terminators,
+            push_terminators=self.terminators,
+        ) as ctx:
+            resp = elem.match(segments, ctx)
+
         return resp
 
     @classmethod
-    def keyword(cls, keyword, **kwargs):
+    def keyword(cls, keyword: str, **kwargs) -> BaseGrammar:
         """Generate a reference to a keyword by name.
 
         This function is entirely syntactic sugar, and designed
         for more readable dialects.
 
         Ref.keyword('select') == Ref('SelectKeywordSegment')
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             )
         if not rules:  # pragma: no cover
             raise ValueError("Conditional requires rules to be set.")
         self._config_type = config_type
         self._config_rules = rules
         super().__init__(*args)
 
-    def is_enabled(self, parse_context):
+    def is_enabled(self, parse_context) -> bool:
         """Evaluate conditionals and return whether enabled."""
         # NOTE: Because only "indentation" is the only current config_type
         # supported, this code is much simpler that would be required in
         # future if multiple options are available.
         if self._config_type != "indentation":  # pragma: no cover
             raise ValueError(
                 "Only 'indentation' is supported as a Conditional config_type."
@@ -78,15 +78,15 @@
             conf_val = config_section.get(rule, False)
             # Coerce to boolean.
             if val != bool(conf_val):
                 return False
         return True
 
     @match_wrapper()
-    def match(self, segments, parse_context):
+    def match(self, segments, parse_context) -> MatchResult:
         """Evaluate conditionals and return content."""
         if not self.is_enabled(parse_context):  # pragma: no cover TODO?
             return MatchResult.from_unmatched(segments)
 
         # Instantiate the new element and return
         new_seg = self._elements[0]()
         return MatchResult((new_seg,), segments)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self,
         *args,
         delimiter=Ref("CommaSegment"),
         allow_trailing=False,
         terminator=None,
         min_delimiters=None,
         **kwargs,
-    ):
+    ) -> None:
         if delimiter is None:  # pragma: no cover
             raise ValueError("Delimited grammars require a `delimiter`")
         self.bracket_pairs_set = kwargs.pop("bracket_pairs_set", "bracket_pairs")
         self.delimiter = self._resolve_ref(delimiter)
         self.allow_trailing = allow_trailing
         self.terminator = self._resolve_ref(terminator)
         # Setting min delimiters means we have to match at least this number
@@ -146,17 +146,20 @@
                     if match:
                         terminated = True
                         unmatched_segments = (
                             pre_non_code + match.all_segments() + post_non_code
                         )
                         break
 
-                with parse_context.deeper_match() as ctx:
-                    if delimiter_matchers and elements != delimiter_matchers:
-                        ctx.push_terminators(delimiter_matchers)
+                _push_terminators = []
+                if delimiter_matchers and elements != delimiter_matchers:
+                    _push_terminators = delimiter_matchers
+                with parse_context.deeper_match(
+                    push_terminators=_push_terminators
+                ) as ctx:
                     match, _ = self._longest_trimmed_match(
                         segments=seg_content,
                         matchers=elements,
                         parse_context=ctx,
                         # We've already trimmed
                         trim_noncode=False,
                     )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.parser.segments import allow_ephemeral
 
 from sqlfluff.core.parser.grammar.base import (
     BaseGrammar,
+    BaseSegment,
     cached_method_for_parse_context,
 )
+from typing import Tuple
 
 
 class GreedyUntil(BaseGrammar):
     """Matching for GreedyUntil works just how you'd expect.
 
     Args:
         enforce_whitespace_preceding (:obj:`bool`): Should the GreedyUntil
             match only match the content if it's preceded by whitespace?
             (defaults to False). This is useful for some keywords which may
             have false alarms on some array accessors.
 
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         self.enforce_whitespace_preceding_terminator = kwargs.pop(
             "enforce_whitespace_preceding_terminator", False
         )
         super().__init__(*args, **kwargs)
         if not self.allow_gaps:  # pragma: no cover
             raise NotImplementedError(
                 f"{self.__class__} does not support allow_gaps=False."
             )
 
     @match_wrapper()
     @allow_ephemeral
-    def match(self, segments, parse_context):
+    def match(self, segments, parse_context) -> MatchResult:
         """Matching for GreedyUntil works just how you'd expect."""
         return self.greedy_match(
             segments,
             parse_context,
             matchers=self._elements,
             enforce_whitespace_preceding_terminator=(
                 self.enforce_whitespace_preceding_terminator
@@ -51,18 +53,18 @@
     def greedy_match(
         cls,
         segments,
         parse_context,
         matchers,
         enforce_whitespace_preceding_terminator,
         include_terminator=False,
-    ):
+    ) -> MatchResult:
         """Matching for GreedyUntil works just how you'd expect."""
         seg_buff = segments
-        seg_bank = ()  # Empty tuple
+        seg_bank: Tuple[BaseSegment, ...] = ()  # Empty tuple
         # If no terminators then just return the whole thing.
         # Shouldn't really happen as GreedyMatch is everything
         # and StartsWith has mandatory terminator
         if matchers == [None]:  # pragma: no cover
             return MatchResult.from_matched(segments)
 
         while True:
@@ -153,15 +155,15 @@
 
 class StartsWith(GreedyUntil):
     """Match if this sequence starts with a match.
 
     This also has configurable whitespace and comment handling.
     """
 
-    def __init__(self, target, *args, **kwargs):
+    def __init__(self, target, *args, **kwargs) -> None:
         self.target = self._resolve_ref(target)
         self.terminator = self._resolve_ref(kwargs.pop("terminator", None))
         self.include_terminator = kwargs.pop("include_terminator", False)
 
         # StartsWith should only be used with a terminator
         assert self.terminator
 
@@ -172,15 +174,17 @@
         """Does this matcher support a uppercase hash matching route?
 
         `StartsWith` is simple, if the thing it starts with is also simple.
         """
         return self.target.simple(parse_context=parse_context, crumbs=crumbs)
 
     @match_wrapper()
-    def match(self, segments, parse_context):
+    def match(
+        self, segments: Tuple[BaseSegment, ...], parse_context: ParseContext
+    ) -> MatchResult:
         """Match if this sequence starts with a match."""
         first_code_idx = None
         # Work through to find the first code segment...
         for idx, seg in enumerate(segments):
             if seg.is_code:
                 first_code_idx = idx
                 break
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 terminator or similar alongside other matchers.
 """
 
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.matchable import Matchable
 from sqlfluff.core.parser.context import ParseContext
+from sqlfluff.core.parser.grammar.types import SimpleHintType
+from typing import Tuple, Optional
 
 
 class NonCodeMatcher(Matchable):
     """An object which behaves like a matcher to match non-code."""
 
-    def simple(self, parse_context: ParseContext, crumbs=None):
+    def simple(
+        self, parse_context: ParseContext, crumbs: Optional[Tuple[str, ...]] = None
+    ) -> SimpleHintType:
         """This element doesn't work with simple."""
         return None
 
-    def is_optional(self):  # pragma: no cover TODO?
+    def is_optional(self) -> bool:  # pragma: no cover TODO?
         """Not optional."""
         return False
 
     def cache_key(self) -> str:
         """Get the cache key for the matcher.
 
         NOTE: In this case, this class is a bit of a singleton
         and so we don't need a unique UUID in the same way as
         other classes.
         """
         return "non-code-matcher"
 
     @match_wrapper(v_level=4)
-    def match(self, segments, parse_context):
+    def match(self, segments, parse_context: ParseContext) -> MatchResult:
         """Match any starting non-code segments."""
         if not isinstance(segments, tuple):  # pragma: no cover
             raise TypeError("NonCodeMatcher expects a tuple.")
         idx = 0
         while idx < len(segments) and not segments[idx].is_code:
             idx += 1
         return MatchResult(segments[:idx], segments[idx:])
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from sqlfluff.core.parser.helpers import trim_non_code_segments, check_still_complete
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.matchable import Matchable
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.parser.grammar.base import (
     BaseGrammar,
-    MatchableType,
     cached_method_for_parse_context,
+    MatchableType,
 )
+from sqlfluff.core.parser.grammar.types import SimpleHintType
 from sqlfluff.core.parser.grammar.conditional import Conditional
 from os import getenv
 
 
 def _all_remaining_metas(
     remaining_elements: _Sequence[MatchableType], parse_context: ParseContext
-) -> Optional[Tuple[BaseSegment, ...]]:
+) -> Optional[Tuple[MetaSegment, ...]]:
     """Check the remaining elements, instantiate them if they're metas.
 
     Helper function in `Sequence.match()`.
     """
     # Are all the remaining elements metas?
     if not all(
         e.is_optional()
@@ -43,39 +44,41 @@
         for e in remaining_elements
     ):
         # No? Return Nothing.
         return None
 
     # Yes, so we shortcut back early because we don't want
     # to claim any more whitespace.
-    return_segments: Tuple[BaseSegment, ...] = tuple()
+    return_segments: Tuple[MetaSegment, ...] = tuple()
     # Instantiate all the metas
     for e in remaining_elements:
         # If it's meta, instantiate it.
         if e.is_optional():
             continue
         elif isinstance(e, Conditional):
             if e.is_enabled(parse_context):
                 meta_match = e.match(tuple(), parse_context)
                 if meta_match:
-                    return_segments += meta_match.matched_segments
+                    return_segments += cast(
+                        Tuple[MetaSegment, ...], meta_match.matched_segments
+                    )
             continue
         elif not isinstance(e, Matchable) and e.is_meta:
             indent_seg = cast(Type[MetaSegment], e)
             return_segments += (indent_seg(),)
     return return_segments
 
 
 class Sequence(BaseGrammar):
     """Match a specific sequence of elements."""
 
     test_env = getenv("SQLFLUFF_TESTENV", "")
 
     @cached_method_for_parse_context
-    def simple(self, parse_context: ParseContext, crumbs=None):
+    def simple(self, parse_context: ParseContext, crumbs=None) -> SimpleHintType:
         """Does this matcher support a uppercase hash matching route?
 
         Sequence does provide this, as long as the *first* non-optional
         element does, *AND* and optional elements which preceded it also do.
         """
         simple_raws = set()
         simple_types = set()
@@ -90,25 +93,22 @@
                 # We found our first non-optional element!
                 return frozenset(simple_raws), frozenset(simple_types)
         # If *all* elements are optional AND simple, I guess it's also simple.
         return frozenset(simple_raws), frozenset(simple_types)
 
     @match_wrapper()
     @allow_ephemeral
-    def match(self, segments, parse_context):
+    def match(self, segments, parse_context: ParseContext) -> MatchResult:
         """Match a specific sequence of elements."""
-        if isinstance(segments, BaseSegment):
-            segments = tuple(segments)  # pragma: no cover TODO?
-
         matched_segments = MatchResult.from_empty()
         unmatched_segments = segments
 
         # Buffers of uninstantiated meta segments.
-        meta_pre_nc = ()
-        meta_post_nc = ()
+        meta_pre_nc: Tuple[MetaSegment, ...] = ()
+        meta_post_nc: Tuple[MetaSegment, ...] = ()
         early_break = False
 
         for idx, elem in enumerate(self._elements):
             # Check for an early break.
             if early_break:
                 break
 
@@ -128,32 +128,34 @@
                     else:
                         # No, there's more left to match.
                         # That means we've haven't matched the whole
                         # sequence.
                         return MatchResult.from_unmatched(segments)
 
                 # Then handle any metas mid-sequence.
-                new_metas = ()
+                new_metas: Tuple[MetaSegment, ...] = ()
                 # Is it a raw meta?
                 if elem.is_meta:
                     new_metas = (elem(),)
                 elif isinstance(elem, Conditional):
                     if not elem.is_enabled(parse_context):
                         # If it's not active, skip it.
                         break
                     # Then if it _is_ active. Match against it.
                     with parse_context.deeper_match() as ctx:
-                        meta_match = elem.match(unmatched_segments, parse_context=ctx)
+                        meta_match = elem.match(unmatched_segments, ctx)
                     # Did it match and leave the unmatched portion the same?
                     if (
                         meta_match
                         and meta_match.unmatched_segments == unmatched_segments
                     ):
                         # If it did, it's just returned a new meta, keep it.
-                        new_metas = meta_match.matched_segments
+                        new_metas = cast(
+                            Tuple[MetaSegment, ...], meta_match.matched_segments
+                        )
 
                 # Do we have a new meta?
                 if new_metas:
                     # Elements with a negative indent value come AFTER
                     # the whitespace. Positive or neutral come BEFORE.
                     # HOWEVER: If one is already there, we must preserve
                     # the order. This forced ordering is fine if there's
@@ -256,15 +258,15 @@
       grammar.
     - Post 0.1.0: Bracketed was separate from sequence, and the content
       of the expression were treated as options (like OneOf).
     - Pre 0.1.0: Bracketed inherited from Sequence and simply added
       brackets to that sequence.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         # Store the bracket type. NB: This is only
         # hydrated into segments at runtime.
         self.bracket_type = kwargs.pop("bracket_type", "round")
         self.bracket_pairs_set = kwargs.pop("bracket_pairs_set", "bracket_pairs")
         # Allow optional override for special bracket-like things
         self.start_bracket = kwargs.pop("start_bracket", None)
         self.end_bracket = kwargs.pop("end_bracket", None)
@@ -275,15 +277,15 @@
         """Does this matcher support a uppercase hash matching route?
 
         Bracketed does this easily, we just look for the bracket.
         """
         start_bracket, _, _ = self.get_bracket_from_dialect(parse_context)
         return start_bracket.simple(parse_context=parse_context, crumbs=crumbs)
 
-    def get_bracket_from_dialect(self, parse_context):
+    def get_bracket_from_dialect(self, parse_context: ParseContext):
         """Rehydrate the bracket segments in question."""
         for bracket_type, start_ref, end_ref, persists in parse_context.dialect.sets(
             self.bracket_pairs_set
         ):
             if bracket_type == self.bracket_type:
                 start_bracket = parse_context.dialect.ref(start_ref)
                 end_bracket = parse_context.dialect.ref(end_ref)
@@ -350,18 +352,17 @@
                 start_match = start_bracket.match(seg_buff, parse_context=ctx)
             if start_match:
                 seg_buff = start_match.unmatched_segments
             else:
                 # Can't find the opening bracket. No Match.
                 return MatchResult.from_unmatched(segments)
 
-            # Look for the closing bracket
-            with parse_context.deeper_match() as ctx:
-                # Within the brackets, clear any inherited terminators.
-                ctx.clear_terminators()
+            # Look for the closing bracket.
+            # Within the brackets, clear any inherited terminators.
+            with parse_context.deeper_match(clear_terminators=True) as ctx:
                 content_segs, end_match, _ = self._bracket_sensitive_look_ahead_match(
                     segments=seg_buff,
                     matchers=[end_bracket],
                     parse_context=ctx,
                     start_bracket=start_bracket,
                     end_bracket=end_bracket,
                     bracket_pairs_set=self.bracket_pairs_set,
@@ -376,16 +377,16 @@
             # Construct a bracket segment
             bracket_segment = BracketedSegment(
                 segments=(
                     start_match.matched_segments
                     + content_segs
                     + end_match.matched_segments
                 ),
-                start_bracket=start_match.matched_segments,
-                end_bracket=end_match.matched_segments,
+                start_bracket=cast(Tuple[BaseSegment], start_match.matched_segments),
+                end_bracket=cast(Tuple[BaseSegment], end_match.matched_segments),
             )
             trailing_segments = end_match.unmatched_segments
 
         # Then trim whitespace and deal with the case of non-code content e.g. "(   )"
         if self.allow_gaps:
             pre_segs, content_segs, post_segs = trim_non_code_segments(content_segs)
         else:  # pragma: no cover TODO?
@@ -404,34 +405,30 @@
                     else bracket_segment.segments,
                     trailing_segments,
                 )
             else:
                 return MatchResult.from_unmatched(segments)
 
         # Match the content using super. Sequence will interpret the content of the
-        # elements.
-        with parse_context.deeper_match() as ctx:
-            # Within the brackets, clear any inherited terminators.
-            ctx.clear_terminators()
-            content_match = super().match(content_segs, parse_context=ctx)
+        # elements. Within the brackets, clear any inherited terminators.
+        with parse_context.deeper_match(clear_terminators=True) as ctx:
+            content_match = super().match(content_segs, ctx)
 
         # We require a complete match for the content (hopefully for obvious reasons)
         if content_match.is_complete():
             # Reconstruct the bracket segment post match.
             # We need to realign the meta segments so the pos markers are correct.
             # Have we already got indents?
             meta_idx = None
-            for idx, seg in enumerate(bracket_segment.segments):
-                if (
-                    seg.is_meta
-                    and cast(MetaSegment, seg).indent_val > 0
-                    and not cast(MetaSegment, seg).is_template
-                ):
-                    meta_idx = idx
-                    break
+            for idx, _seg in enumerate(bracket_segment.segments):
+                if _seg.is_meta:
+                    _meta_seg = cast(MetaSegment, _seg)
+                    if _meta_seg.indent_val > 0 and not _meta_seg.is_template:
+                        meta_idx = idx
+                        break
             # If we've already got indents, don't add more.
             if meta_idx:
                 bracket_segment.segments = BaseSegment._position_segments(
                     bracket_segment.start_bracket
                     + pre_segs
                     + content_match.all_segments()
                     + post_segs
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The code for the Lexer."""
 
 import logging
-from typing import Iterator, Optional, List, Tuple, Union, NamedTuple, Dict
+from typing import Iterator, Optional, List, Tuple, Union, NamedTuple, Dict, Type, Any
 from uuid import UUID, uuid4
 import regex
 
 from sqlfluff.core.parser.segments import (
     BaseSegment,
     RawSegment,
     Indent,
@@ -88,64 +88,69 @@
     """A LexedElement, bundled with it's position in the templated file."""
 
     raw: str
     template_slice: slice
     matcher: "StringLexer"
 
     @classmethod
-    def from_element(cls, element: LexedElement, template_slice: slice):
+    def from_element(
+        cls, element: LexedElement, template_slice: slice
+    ) -> "TemplateElement":
         """Make a TemplateElement from a LexedElement."""
         return cls(
             raw=element.raw, template_slice=template_slice, matcher=element.matcher
         )
 
-    def to_segment(self, pos_marker, subslice=None):
+    def to_segment(self, pos_marker: PositionMarker, subslice: Optional[slice] = None):
         """Create a segment from this lexed element."""
         return self.matcher.construct_segment(
             self.raw[subslice] if subslice else self.raw, pos_marker=pos_marker
         )
 
 
 class LexMatch(NamedTuple):
     """A class to hold matches from the Lexer."""
 
     forward_string: str
     elements: List[LexedElement]
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         """A LexMatch is truthy if it contains a non-zero number of matched elements."""
         return len(self.elements) > 0
 
 
+LexerType = Union["RegexLexer", "StringLexer"]
+
+
 class StringLexer:
     """This singleton matcher matches strings exactly.
 
     This is the simplest usable matcher, but it also defines some of the
     mechanisms for more complicated matchers, which may simply override the
     `_match` function rather than the public `match` function.  This acts as
     the base class for matchers.
     """
 
     def __init__(
         self,
-        name,
-        template,
-        segment_class,
-        subdivider=None,
-        trim_post_subdivide=None,
-        segment_kwargs=None,
-    ):
+        name: str,
+        template: str,
+        segment_class: Type[RawSegment],
+        subdivider: Optional[LexerType] = None,
+        trim_post_subdivide: Optional[LexerType] = None,
+        segment_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> None:
         self.name = name
         self.template = template
         self.segment_class = segment_class
         self.subdivider = subdivider
         self.trim_post_subdivide = trim_post_subdivide
         self.segment_kwargs = segment_kwargs or {}
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.name}>"
 
     def _match(self, forward_string: str) -> Optional[LexedElement]:
         """The private match function. Just look for a literal string."""
         if forward_string.startswith(self.template):
             return LexedElement(self.template, self)
         else:
@@ -269,15 +274,15 @@
         """Construct a segment using the given class a properties."""
         return self.segment_class(raw=raw, pos_marker=pos_marker, **self.segment_kwargs)
 
 
 class RegexLexer(StringLexer):
     """This RegexLexer matches based on regular expressions."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         # We might want to configure this at some point, but for now, newlines
         # do get matched by .
         flags = regex.DOTALL
         self._compiled_regex = regex.compile(self.template, flags)
 
     def _match(self, forward_string: str) -> Optional[LexedElement]:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/markers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implements the PositionMarker class.
 
 This class is a construct to keep track of positions within a file.
 """
 
 from dataclasses import dataclass
-from typing import Tuple, TYPE_CHECKING
+from typing import Optional, Tuple, TYPE_CHECKING
 
 from sqlfluff.core.slice_helpers import zero_slice
 
 if TYPE_CHECKING:
     from sqlfluff.core.templaters import TemplatedFile  # pragma: no cover
 
 
@@ -32,38 +32,38 @@
     source_slice: slice
     templated_slice: slice
     templated_file: "TemplatedFile"
     # If not set, these will be initialised in the post init.
     working_line_no: int = -1
     working_line_pos: int = -1
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         # If the working position has not been explicitly set
         # then infer it from the position in the templated file.
         # This is accurate up until the point that any fixes have
         # been applied.
         if self.working_line_no == -1 or self.working_line_pos == -1:
             line_no, line_pos = self.templated_position()
             # Use the base method because we're working with a frozen class
             object.__setattr__(self, "working_line_no", line_no)
             object.__setattr__(self, "working_line_pos", line_pos)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.to_source_string()
 
-    def __gt__(self, other):
+    def __gt__(self, other: "PositionMarker") -> bool:
         return self.working_loc > other.working_loc  # pragma: no cover TODO?
 
-    def __lt__(self, other):
+    def __lt__(self, other: "PositionMarker") -> bool:
         return self.working_loc < other.working_loc  # pragma: no cover TODO?
 
-    def __ge__(self, other):
+    def __ge__(self, other: "PositionMarker") -> bool:
         return self.working_loc >= other.working_loc  # pragma: no cover TODO?
 
-    def __le__(self, other):
+    def __le__(self, other: "PositionMarker") -> bool:
         return self.working_loc <= other.working_loc  # pragma: no cover TODO?
 
     @property
     def working_loc(self) -> Tuple[int, int]:
         """Location tuple for the working position."""
         return self.working_line_no, self.working_line_pos
 
@@ -77,30 +77,30 @@
 
     @classmethod
     def from_point(
         cls,
         source_point: int,
         templated_point: int,
         templated_file: "TemplatedFile",
-        **kwargs,
-    ):
+        **kwargs: int,  # kwargs can only contain working_line positions
+    ) -> "PositionMarker":
         """Convenience method for creating point markers."""
         return cls(
             zero_slice(source_point),
             zero_slice(templated_point),
             templated_file,
             **kwargs,
         )
 
     @classmethod
     def from_points(
         cls,
         start_point_marker: "PositionMarker",
         end_point_marker: "PositionMarker",
-    ):
+    ) -> "PositionMarker":
         """Construct a position marker from the section between two points."""
         return cls(
             slice(
                 start_point_marker.source_slice.start,
                 end_point_marker.source_slice.stop,
             ),
             slice(
@@ -114,25 +114,27 @@
             start_point_marker.templated_file,
             # Line position should be of the _start_ of the section.
             start_point_marker.working_line_no,
             start_point_marker.working_line_pos,
         )
 
     @classmethod
-    def from_child_markers(cls, *markers):
+    def from_child_markers(
+        cls, *markers: Optional["PositionMarker"]
+    ) -> "PositionMarker":
         """Create a parent marker from it's children."""
         source_slice = slice(
-            min(m.source_slice.start for m in markers),
-            max(m.source_slice.stop for m in markers),
+            min(m.source_slice.start for m in markers if m),
+            max(m.source_slice.stop for m in markers if m),
         )
         templated_slice = slice(
-            min(m.templated_slice.start for m in markers),
-            max(m.templated_slice.stop for m in markers),
+            min(m.templated_slice.start for m in markers if m),
+            max(m.templated_slice.stop for m in markers if m),
         )
-        templated_files = {m.templated_file for m in markers}
+        templated_files = {m.templated_file for m in markers if m}
         if len(templated_files) != 1:  # pragma: no cover
             raise ValueError("Attempted to make a parent marker from multiple files.")
         templated_file = templated_files.pop()
         return cls(source_slice, templated_slice, templated_file)
 
     def source_position(self) -> Tuple[int, int]:
         """Return the line and position of this marker in the source."""
@@ -177,17 +179,18 @@
         return self.__class__.from_point(
             self.source_slice.stop,
             self.templated_slice.stop,
             templated_file=self.templated_file,
         )
 
     @staticmethod
-    def slice_is_point(test_slice):
+    def slice_is_point(test_slice: slice) -> bool:
         """Is this slice a point."""
-        return test_slice.start == test_slice.stop
+        is_point: bool = test_slice.start == test_slice.stop
+        return is_point
 
     def is_point(self) -> bool:
         """A marker is a point if it has zero length in templated and source file."""
         return self.slice_is_point(self.source_slice) and self.slice_is_point(
             self.templated_slice
         )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/match_logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """Classes to help with match logging."""
 
+import logging
+from typing import Any, Tuple, TYPE_CHECKING
 from sqlfluff.core.parser.helpers import join_segments_raw_curtailed
 
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.parser.context import ParseContext
+    from sqlfluff.core.parser import BaseSegment
+
 
 class LateLoggingObject:
     """A basic late binding log object for parse_match_logging.
 
     This allows us to defer the string manipulation involved
     until actually required by the logger.
     """
 
     __slots__ = "v_level", "logger", "msg"
 
-    def __init__(self, logger, msg, v_level=3):
+    def __init__(self, logger: logging.Logger, msg: str, v_level: int = 3) -> None:
         self.v_level = v_level
         self.logger = logger
         self.msg = msg
 
-    def __str__(self):  # pragma: no cover TODO?
+    def __str__(self) -> str:  # pragma: no cover TODO?
         """Actually materialise the string."""
         return self.msg
 
-    def log(self):
+    def log(self) -> None:
         """Actually log this object."""
         # Otherwise carry on...
         if self.v_level == 3:
             self.logger.info(self)
         elif self.v_level == 4:
             self.logger.debug(self)
 
@@ -40,22 +46,30 @@
     __slots__ = [
         "context",
         "grammar",
         "func",
         "kwargs",
     ]
 
-    def __init__(self, parse_context, grammar, func, msg, v_level=3, **kwargs):
+    def __init__(
+        self,
+        parse_context: "ParseContext",
+        grammar: str,
+        func: str,
+        msg: str,
+        v_level: int = 3,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(v_level=v_level, logger=parse_context.logger, msg=msg)
         self.context = parse_context
         self.grammar = grammar
         self.func = func
         self.kwargs = kwargs
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Actually materialise the string."""
         symbol = self.kwargs.pop("symbol", "")
         s = "[PD:{:<2} MD:{:<2}]\t{:<50}\t{:<20}\t{:<4}".format(
             self.context.parse_depth,
             self.context.match_depth,
             ("." * self.context.match_depth) + str(self.context.match_segment),
             f"{self.grammar:.5}.{self.func} {self.msg}",
@@ -67,15 +81,22 @@
                     f"{k}={repr(v) if isinstance(v, str) else str(v)}"
                     for k, v in self.kwargs.items()
                 )
             )
         return s
 
 
-def parse_match_logging(grammar, func, msg, parse_context, v_level=3, **kwargs):
+def parse_match_logging(
+    grammar: str,
+    func: str,
+    msg: str,
+    parse_context: "ParseContext",
+    v_level: int = 3,
+    **kwargs: Any,
+) -> None:
     """Log in a particular consistent format for use while matching."""
     # Make a late bound log object so we only do the string manipulation when we need
     # to.
     ParseMatchLogObject(
         parse_context, grammar, func, msg, v_level=v_level, **kwargs
     ).log()
 
@@ -83,12 +104,12 @@
 class LateBoundJoinSegmentsCurtailed:
     """Object to delay `join_segments_raw_curtailed` until later.
 
     This allows us to defer the string manipulation involved
     until actually required by the logger.
     """
 
-    def __init__(self, segments):
+    def __init__(self, segments: Tuple["BaseSegment", ...]) -> None:
         self.segments = segments
 
-    def __str__(self):
+    def __str__(self) -> str:
         return repr(join_segments_raw_curtailed(self.segments))
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 """Defined the `match_wrapper` which adds validation and logging to match methods."""
 
+from typing import Any, Callable, Tuple, TYPE_CHECKING
+
 from sqlfluff.core.parser.match_logging import ParseMatchLogObject
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.helpers import join_segments_raw_curtailed
 
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.parser.context import ParseContext
+    from sqlfluff.core.parser import BaseSegment
+
+
+MatchFuncType = Callable[[Any, Tuple["BaseSegment", ...], "ParseContext"], MatchResult]
+
 
 class WrapParseMatchLogObject(ParseMatchLogObject):
     """A specialised version of ParseMatchLogObject.
 
     This defers some of the specialist handling to later.
     """
 
-    def __init__(self, match, segments, **kwargs):
+    def __init__(
+        self, match: MatchResult, segments: Tuple["BaseSegment", ...], **kwargs: Any
+    ) -> None:
         self.match = match
         self.segments = segments
         super().__init__(msg="OUT", match=match, **kwargs)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.match.is_complete():
             self.kwargs["symbol"] = "++"
         elif self.match:
             self.kwargs["symbol"] = "+"
         self.kwargs["seg"] = repr(join_segments_raw_curtailed(self.segments))
         return super().__str__()
 
 
-def match_wrapper(v_level=3):
+def match_wrapper(v_level: int = 3) -> Callable[[MatchFuncType], MatchFuncType]:
     """Wraps a .match() method to add validation and logging.
 
     This is designed to be used as follows:
 
         class SomeMatchableObject(object):
             @match_wrapper()
             def match(self, segments, parse_context):
                 ...
                 return m
 
     This applies a common logging framework to both Grammar and
     Segment based match routines.
     """
 
-    def inner_match_wrapper(func):
+    def inner_match_wrapper(func: MatchFuncType) -> MatchFuncType:
         """Decorate a match function."""
 
-        def wrapped_match_method(self_cls, segments: tuple, parse_context):
+        def wrapped_match_method(
+            self_cls: Any,
+            segments: Tuple["BaseSegment", ...],
+            parse_context: "ParseContext",
+        ) -> MatchResult:
             """A wrapper on the match function to do some basic validation."""
             # Do the match
-            m = func(self_cls, segments, parse_context=parse_context)
+            m = func(self_cls, segments, parse_context)
 
             name = getattr(self_cls, "__name__", self_cls.__class__.__name__)
 
             # Validate result
             if not isinstance(m, MatchResult):  # pragma: no cover
                 parse_context.logger.warning(
                     f"{name}.match, returned {type(m)} rather than MatchResult"
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/matchable.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     from sqlfluff.core.parser.context import ParseContext
     from sqlfluff.core.parser.match_result import MatchResult
 
 
 class Matchable(ABC):
     """A base object defining the matching interface."""
 
+    # Matchables are expected to have a type
+    type: Optional[str]
+
     @abstractmethod
     def is_optional(self) -> bool:
         """Return whether this element is optional."""
 
     @abstractmethod
     def simple(
         self, parse_context: "ParseContext", crumbs: Optional[Tuple[str, ...]] = None
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Defines the Parser class."""
 
-from typing import Optional, Sequence, TYPE_CHECKING
+from typing import Optional, Sequence, Type, TYPE_CHECKING
 
-from sqlfluff.core.parser.context import RootParseContext
+from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.config import FluffConfig
 
-if TYPE_CHECKING:
-    from sqlfluff.core.parser.segments import BaseSegment  # pragma: no cover
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.parser.segments import (
+        BaseSegment,
+        BaseFileSegment,
+    )
 
 
 class Parser:
     """Instantiates parsed queries from a sequence of lexed raw segments."""
 
     def __init__(
         self, config: Optional[FluffConfig] = None, dialect: Optional[str] = None
     ):
         # Allow optional config and dialect
         self.config = FluffConfig.from_kwargs(config=config, dialect=dialect)
-        self.RootSegment = self.config.get("dialect_obj").get_root_segment()
+        self.RootSegment: Type[BaseFileSegment] = self.config.get(
+            "dialect_obj"
+        ).get_root_segment()
 
     def parse(
         self,
         segments: Sequence["BaseSegment"],
         recurse=True,
         fname: Optional[str] = None,
         parse_statistics: bool = False,
@@ -32,33 +37,41 @@
             # be an end_of_file segment. It would probably only happen in
             # api use cases.
             return None
         # Instantiate the root segment
         root_segment = self.RootSegment(segments=segments, fname=fname)
         # Call .parse() on that segment
 
-        with RootParseContext.from_config(config=self.config, recurse=recurse) as ctx:
-            parsed = root_segment.parse(parse_context=ctx)
+        # NOTE: This is the only time we use the parse context not in the
+        # context of a context manager. That's because it's the initial
+        # instantiation.
+        ctx = ParseContext.from_config(config=self.config, recurse=recurse)
+        parsed = root_segment.parse(parse_context=ctx)
+
+        if parse_statistics:  # pragma: no cover
+            # NOTE: We use ctx.logger.warning here to output the statistics.
+            # It's not particularly beautiful, but for the users who do utilise
+            # this functionality, I don't think they mind. ¯\_(ツ)_/¯
+            # In the future, this clause might become unnecessary.
+            ctx.logger.warning("==== Parse Statistics ====")
+            for key in ctx.parse_stats:
+                if key == "next_counts":
+                    continue
+                ctx.logger.warning(f"{key}: {ctx.parse_stats[key]}")
+            ctx.logger.warning("## Tokens following un-terminated matches")
+            ctx.logger.warning(
+                "Adding terminator clauses to catch these may improve performance."
+            )
+            for key, val in sorted(
+                ctx.parse_stats["next_counts"].items(),
+                reverse=True,
+                key=lambda item: item[1],
+            ):
+                ctx.logger.warning(f"{val}: {key!r}")
+            ctx.logger.warning("==== End Parse Statistics ====")
 
-            if parse_statistics:  # pragma: no cover
-                # NOTE: We use ctx.logger.warning here to output the statistics.
-                # It's not particularly beautiful, but for the users who do utilise
-                # this functionality, I don't think they mind. ¯\_(ツ)_/¯
-                # In the future, this clause might become unnecessary.
-                ctx.logger.warning("==== Parse Statistics ====")
-                for key in ctx.parse_stats:
-                    if key == "next_counts":
-                        continue
-                    ctx.logger.warning(f"{key}: {ctx.parse_stats[key]}")
-                ctx.logger.warning("## Tokens following un-terminated matches")
-                ctx.logger.warning(
-                    "Adding terminator clauses to catch these may improve performance."
-                )
-                for key, val in sorted(
-                    ctx.parse_stats["next_counts"].items(),
-                    reverse=True,
-                    key=lambda item: item[1],
-                ):
-                    ctx.logger.warning(f"{val}: {key!r}")
-                ctx.logger.warning("==== End Parse Statistics ====")
-
-        return parsed
+        if not parsed:  # pragma: no cover
+            return None
+        elif len(parsed) == 1:
+            return parsed[0]
+        else:  # pragma: no cover
+            raise ValueError(f"Unexpected longer root parse result [{len(parsed)}].")
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from abc import abstractmethod
 from uuid import uuid4
 import regex
 from typing import Collection, Type, Optional, Tuple, Union
 
 from sqlfluff.core.parser.context import ParseContext
+from sqlfluff.core.parser.grammar.types import SimpleHintType
 from sqlfluff.core.parser.matchable import Matchable
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.segments import RawSegment, BaseSegment
 
 
 class BaseParser(Matchable):
     """An abstract class from which other Parsers should inherit."""
@@ -44,15 +45,15 @@
         return self._cache_key
 
     def is_optional(self) -> bool:
         """Return whether this element is optional."""
         return self.optional
 
     @abstractmethod
-    def _is_first_match(self, segment: BaseSegment):
+    def _is_first_match(self, segment: BaseSegment) -> bool:
         """Does the segment provided match according to the current rules."""
 
     def _make_match_from_segment(self, segment: BaseSegment):
         """Make a MatchResult from the first segment in the given list.
 
         This is a helper function for reuse by other parsers.
         """
@@ -107,35 +108,35 @@
     def __init__(
         self,
         template: str,
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         **segment_kwargs,
-    ):
+    ) -> None:
         # NB: the template in this case is the _target_ type.
         # The type kwarg is the eventual type.
         self.template = template
         super().__init__(
             raw_class=raw_class,
             # If no type specified we default to the template
             type=type or template,
             optional=optional,
             **segment_kwargs,
         )
 
-    def simple(cls, parse_context: ParseContext, crumbs=None):
+    def simple(cls, parse_context: ParseContext, crumbs=None) -> SimpleHintType:
         """Does this matcher support a uppercase hash matching route?
 
         TypedParser segment doesn't support matching against raw strings,
         but it does support it against types.
         """
         return frozenset(), frozenset((cls.template,))
 
-    def _is_first_match(self, segment: BaseSegment):
+    def _is_first_match(self, segment: BaseSegment) -> bool:
         """Return true if the type matches the target type."""
         return segment.is_type(self.template)
 
 
 class StringParser(BaseParser):
     """An object which matches and returns raw segments based on strings."""
 
@@ -153,23 +154,23 @@
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             **segment_kwargs,
         )
 
-    def simple(self, parse_context: "ParseContext", crumbs=None):
+    def simple(self, parse_context: "ParseContext", crumbs=None) -> SimpleHintType:
         """Return simple options for this matcher.
 
         Because string matchers are not case sensitive we can
         just return the template here.
         """
         return self._simple, frozenset()
 
-    def _is_first_match(self, segment: BaseSegment):
+    def _is_first_match(self, segment: BaseSegment) -> bool:
         """Does the segment provided match according to the current rules."""
         # Is the target a match and IS IT CODE.
         # The latter stops us accidentally matching comments.
         if self.template == segment.raw_upper and segment.is_code:
             return True
         return False
 
@@ -191,23 +192,23 @@
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             **segment_kwargs,
         )
 
-    def simple(self, parse_context: "ParseContext", crumbs=None):
+    def simple(self, parse_context: "ParseContext", crumbs=None) -> SimpleHintType:
         """Return simple options for this matcher.
 
         Because string matchers are not case sensitive we can
         just return the templates here.
         """
         return self._simple, frozenset()
 
-    def _is_first_match(self, segment: BaseSegment):
+    def _is_first_match(self, segment: BaseSegment) -> bool:
         """Does the segment provided match according to the current rules."""
         # Is the target a match and IS IT CODE.
         # The latter stops us accidentally matching comments.
         if segment.is_code and segment.raw_upper in self.templates:
             return True
         return False
 
@@ -233,22 +234,22 @@
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             **segment_kwargs,
         )
 
-    def simple(cls, parse_context: ParseContext, crumbs=None):
+    def simple(cls, parse_context: ParseContext, crumbs=None) -> None:
         """Does this matcher support a uppercase hash matching route?
 
         Regex segment does NOT for now. We might need to later for efficiency.
         """
         return None
 
-    def _is_first_match(self, segment: BaseSegment):
+    def _is_first_match(self, segment: BaseSegment) -> bool:
         """Does the segment provided match according to the current rules.
 
         RegexParser implements its own matching function where
         we assume that ._template is a r"" string, and is formatted
         for use directly as a regex. This only matches on a single segment.
         """
         if len(segment.raw) == 0:  # pragma: no cover TODO?
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from copy import deepcopy, copy
 from dataclasses import dataclass, field, replace
 from io import StringIO
 from itertools import chain
 from typing import (
     Any,
     Callable,
+    cast,
     ClassVar,
     Dict,
     Optional,
     List,
     Tuple,
     Iterator,
     Set,
@@ -34,30 +35,29 @@
 from sqlfluff.core.cached_property import cached_property
 from sqlfluff.core.config import progress_bar_configuration
 from sqlfluff.core.string_helpers import (
     frame_msg,
     curtail_string,
 )
 
-from sqlfluff.core.parser.context import RootParseContext
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_logging import parse_match_logging
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.helpers import (
     check_still_complete,
     trim_non_code_segments,
 )
 from sqlfluff.core.parser.matchable import Matchable
 from sqlfluff.core.parser.markers import PositionMarker
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.templaters.base import TemplatedFile
 
-if TYPE_CHECKING:
-    from sqlfluff.core.rules import LintFix  # pragma: no cover
-    from sqlfluff.core.parser.segments import RawSegment  # pragma: no cover
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.rules import LintFix
+    from sqlfluff.core.parser.segments import RawSegment
 
 # Instantiate the linter logger (only for use in methods involved with fixing.)
 linter_logger = logging.getLogger("sqlfluff.linter")
 
 
 @dataclass(frozen=True)
 class SourceFix:
@@ -68,15 +68,15 @@
     # TODO: It might be possible to refactor this to not require
     # a templated_slice (because in theory it's unnecessary).
     # However much of the fix handling code assumes we need
     # a position in the templated file to interpret it.
     # More work required to achieve that if desired.
     templated_slice: slice
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         # Only hash based on the source slice, not the
         # templated slice (which might change)
         return hash((self.edit, self.source_slice.start, self.source_slice.stop))
 
 
 @dataclass(frozen=True)
 class PathStep:
@@ -105,33 +105,33 @@
     # than for function. It allows traceability of *why* this patch was
     # generated. It has no significance for processing.
     patch_category: str
     source_slice: slice
     templated_str: str
     source_str: str
 
-    def dedupe_tuple(self):
+    def dedupe_tuple(self) -> Tuple[slice, str]:
         """Generate a tuple of this fix for deduping."""
         return (self.source_slice, self.fixed_raw)
 
 
 @dataclass
 class AnchorEditInfo:
     """For a given fix anchor, count of the fix edit types and fixes for it."""
 
     delete: int = field(default=0)
     replace: int = field(default=0)
     create_before: int = field(default=0)
     create_after: int = field(default=0)
-    fixes: List = field(default_factory=list)
-    source_fixes: List = field(default_factory=list)
+    fixes: List["LintFix"] = field(default_factory=list)
+    source_fixes: List[SourceFix] = field(default_factory=list)
     # First fix of edit_type "replace" in "fixes"
     _first_replace: Optional["LintFix"] = field(default=None)
 
-    def add(self, fix: "LintFix"):
+    def add(self, fix: "LintFix") -> None:
         """Adds the fix and updates stats.
 
         We also allow potentially multiple source fixes on the same
         anchor by condensing them together here.
         """
         if fix in self.fixes:
             # Deduplicate fixes in case it's already in there.
@@ -162,20 +162,20 @@
 
         self.fixes.append(fix)
         if fix.edit_type == "replace" and not self._first_replace:
             self._first_replace = fix
         setattr(self, fix.edit_type, getattr(self, fix.edit_type) + 1)
 
     @property
-    def total(self):
+    def total(self) -> int:
         """Returns total count of fixes."""
         return len(self.fixes)
 
     @property
-    def is_valid(self):
+    def is_valid(self) -> bool:
         """Returns True if valid combination of fixes for anchor.
 
         Cases:
         * 0-1 fixes of any type: Valid
         * 2 fixes: Valid if and only if types are create_before and create_after
         """
         if self.total <= 1:
@@ -262,56 +262,41 @@
     # NOTE: Cache key is generated by the SegmentMetaclass
     _cache_key: str
     # _preface_modifier used in ._preface()
     _preface_modifier: str = ""
 
     def __init__(
         self,
-        segments,
+        segments: Tuple["BaseSegment", ...],
         pos_marker: Optional[PositionMarker] = None,
         uuid: Optional[UUID] = None,
-    ):
-        # A cache variable for expandable
-        self._is_expandable: Optional[bool] = None
-
+    ) -> None:
         if len(segments) == 0:  # pragma: no cover
             raise RuntimeError(
                 "Setting {} with a zero length segment set. This shouldn't "
                 "happen.".format(self.__class__)
             )
 
-        if hasattr(segments, "matched_segments"):  # pragma: no cover TODO?
-            # Safely extract segments from a match
-            self.segments = segments.matched_segments
-        elif isinstance(segments, tuple):
-            self.segments = segments
-        elif isinstance(segments, list):
-            self.segments = tuple(segments)
-        else:  # pragma: no cover
-            raise TypeError(f"Unexpected type passed to BaseSegment: {type(segments)}")
-
         if not pos_marker:
-            # If no pos given, it's the pos of the first segment.
-            if isinstance(segments, (tuple, list)):
-                if all(seg.pos_marker for seg in segments):
-                    pos_marker = PositionMarker.from_child_markers(
-                        *(seg.pos_marker for seg in segments)
-                    )
-            else:  # pragma: no cover
-                raise TypeError(
-                    f"Unexpected type passed to BaseSegment: {type(segments)}"
+            # If no pos given, work it out from the children.
+            if all(seg.pos_marker for seg in segments):
+                pos_marker = PositionMarker.from_child_markers(
+                    *(seg.pos_marker for seg in segments)
                 )
 
         self.pos_marker = pos_marker
+        self.segments: Tuple["BaseSegment", ...] = segments
+        # A cache variable for expandable
+        self._is_expandable: Optional[bool] = None
         # Tracker for matching when things start moving.
         self.uuid = uuid or uuid4()
 
         self._recalculate_caches()
 
-    def __setattr__(self, key, value):
+    def __setattr__(self, key, value) -> None:
         try:
             if key == "segments":
                 self._recalculate_caches()
 
         except (AttributeError, KeyError):  # pragma: no cover
             pass
 
@@ -331,35 +316,35 @@
             # This is important for .apply_fixes().
             and (
                 self.pos_marker.start_point_marker()
                 == other.pos_marker.start_point_marker()
             )
         )
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(
             (
                 self.__class__.__name__,
                 self.raw,
                 self.pos_marker.source_position() if self.pos_marker else None,
             )
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: ({self.pos_marker})>"
 
     # ################ PRIVATE PROPERTIES
 
     @property
-    def _comments(self):
+    def _comments(self) -> List["BaseSegment"]:
         """Returns only the comment elements of this segment."""
         return [seg for seg in self.segments if seg.is_type("comment")]
 
     @property
-    def _non_comments(self):  # pragma: no cover TODO?
+    def _non_comments(self) -> List["BaseSegment"]:  # pragma: no cover TODO?
         """Returns only the non-comment elements of this segment."""
         return [seg for seg in self.segments if not seg.is_type("comment")]
 
     # ################ PUBLIC PROPERTIES
 
     @property
     def is_expandable(self) -> bool:
@@ -461,15 +446,15 @@
         """Returns a list of raw segments in this segment with the ancestors."""
         buffer = []
         code_idxs = tuple(idx for idx, seg in enumerate(self.segments) if seg.is_code)
         for idx, seg in enumerate(self.segments):
             # If it's a raw, yield it with this segment as the parent
             new_step = [PathStep(self, idx, len(self.segments), code_idxs)]
             if seg.is_type("raw"):
-                buffer.append((seg, new_step))
+                buffer.append((cast("RawSegment", seg), new_step))
             # If it's not, recurse - prepending self to the ancestor stack
             else:
                 buffer.extend(
                     [
                         (raw_seg, new_step + stack)
                         for raw_seg, stack in seg.raw_segments_with_ancestors
                     ]
@@ -510,19 +495,14 @@
         return (
             self.pos_marker.source_slice.start != self.pos_marker.source_slice.stop
             and not self.pos_marker.is_literal()
         )
 
     # ################ STATIC METHODS
 
-    @staticmethod
-    def segs_to_tuple(segs, **kwargs):  # pragma: no cover TODO?
-        """Return a tuple structure from an iterable of segments."""
-        return tuple(seg.to_tuple(**kwargs) for seg in segs)
-
     def _suffix(self) -> str:
         """Return any extra output required at the end when logging.
 
         NB Override this for specific subclasses if we want extra output.
         """
         return ""
 
@@ -569,20 +549,15 @@
                 )
             parse_depth_msg = "Parse Depth {}. Expanding: {}: {!r}".format(
                 parse_context.parse_depth,
                 stmt.__class__.__name__,
                 curtail_string(stmt.raw, length=40),
             )
             parse_context.logger.info(frame_msg(parse_depth_msg))
-            res = stmt.parse(parse_context=parse_context)
-            if isinstance(res, BaseSegment):
-                segs += (res,)
-            else:
-                # We might get back an iterable of segments
-                segs += tuple(res)
+            segs += stmt.parse(parse_context=parse_context)
 
         # Basic Validation
         check_still_complete(segments, segs, ())
         return segs
 
     @classmethod
     def _position_segments(
@@ -733,32 +708,32 @@
         """Return the cache key for this segment definition.
 
         NOTE: The key itself is generated on _definition_ by the metaclass.
         """
         return cls._cache_key
 
     @classmethod
-    def is_optional(cls):
+    def is_optional(cls) -> bool:
         """Return True if this segment is optional.
 
         This is used primarily in sequence matching, where optional
         segments can be skipped.
         """
         return cls.optional
 
     @classmethod
-    def class_is_type(cls, *seg_type):
+    def class_is_type(cls, *seg_type) -> bool:
         """Is this segment class (or its parent) of the given type."""
         # Use set intersection
         if cls._class_types.intersection(seg_type):
             return True
         return False
 
     @classmethod
-    def structural_simplify(cls, elem):
+    def structural_simplify(cls, elem) -> Optional[dict]:
         """Simplify the structure recursively so it serializes nicely in json/yaml."""
         if len(elem) == 0:
             return None
         elif isinstance(elem, tuple):
             # Does this look like an element?
             if len(elem) == 2 and isinstance(elem[0], str):
                 # This looks like a single element, make a dict
@@ -817,49 +792,33 @@
             return MatchResult((segments[0],), segments[1:])
 
         if cls.match_grammar:
             # Call the private method
             with parse_context.deeper_match() as ctx:
                 m = cls.match_grammar.match(segments=segments, parse_context=ctx)
 
-            # Calling unify here, allows the MatchResult class to do all the type
-            # checking.
-            if not isinstance(m, MatchResult):  # pragma: no cover
-                raise TypeError(
-                    "[PD:{} MD:{}] {}.match. Result is {}, not a MatchResult!".format(
-                        parse_context.parse_depth,
-                        parse_context.match_depth,
-                        cls.__name__,
-                        type(m),
-                    )
-                )
-            # Once unified we can deal with it just as a MatchResult
             if m.has_match():
-                try:
-                    return MatchResult(
-                        (cls(segments=m.matched_segments),), m.unmatched_segments
-                    )
-                except TypeError as err:  # pragma: no cover
-                    # This is an error to assist with debugging dialect design.
-                    # It's most likely that the match_grammar has been set on
-                    # a raw segment which shouldn't happen.
-                    raise TypeError(
-                        f"Error in instantiating {cls.__module__}.{cls.__name__}. Have "
-                        f"you defined a match_grammar on a RawSegment? : {str(err)}"
-                    )
+                return MatchResult(
+                    # Return result of the match_grammar match, wrapped in a new
+                    # instance of this segment. The matched portion of the
+                    # MatchResult from the match_grammar, becomes the children
+                    # (i.e. the `segments`) of that new segment.
+                    (cls(segments=m.matched_segments),),
+                    m.unmatched_segments,
+                )
             else:
                 return MatchResult.from_unmatched(segments)
         else:  # pragma: no cover
             raise NotImplementedError(
                 f"{cls.__name__} has no match function implemented"
             )
 
     # ################ PRIVATE INSTANCE METHODS
 
-    def _recalculate_caches(self):
+    def _recalculate_caches(self) -> None:
         for key in [
             "is_code",
             "is_comment",
             "is_whitespace",
             "raw",
             "raw_upper",
             "matched_length",
@@ -869,15 +828,15 @@
             "source_fixes",
             "full_type_set",
             "descendant_type_set ",
             "direct_descendant_type_set ",
         ]:
             self.__dict__.pop(key, None)
 
-    def _preface(self, ident, tabsize):
+    def _preface(self, ident, tabsize) -> str:
         """Returns the preamble to any logging."""
         padded_type = "{padding}{modifier}{type}".format(
             padding=" " * (ident * tabsize),
             modifier=self._preface_modifier,
             type=self.get_type() + ":",
         )
         preface = "{pos:20}|{padded_type:60}  {suffix}".format(
@@ -886,62 +845,66 @@
             suffix=self._suffix() or "",
         )
         # Trim unnecessary whitespace before returning
         return preface.rstrip()
 
     # ################ PUBLIC INSTANCE METHODS
 
-    def get_type(self):
+    def get_type(self) -> str:
         """Returns the type of this segment as a string."""
         return self.type
 
-    def count_segments(self, raw_only=False):
+    def count_segments(self, raw_only=False) -> int:
         """Returns the number of segments in this segment."""
         if self.segments:
             self_count = 0 if raw_only else 1
             return self_count + sum(
                 seg.count_segments(raw_only=raw_only) for seg in self.segments
             )
         else:
             return 1
 
-    def is_type(self, *seg_type):
+    def is_type(self, *seg_type) -> bool:
         """Is this segment (or its parent) of the given type."""
         return self.class_is_type(*seg_type)
 
-    def invalidate_caches(self):
+    def invalidate_caches(self) -> None:
         """Invalidate the cached properties.
 
         This should be called whenever the segments within this
         segment is mutated.
         """
         for seg in self.segments:
             seg.invalidate_caches()
 
         self._recalculate_caches()
 
-    def get_start_point_marker(self):  # pragma: no cover
+    def get_start_point_marker(self) -> PositionMarker:  # pragma: no cover
         """Get a point marker at the start of this segment."""
+        assert self.pos_marker
         return self.pos_marker.start_point_marker()
 
-    def get_end_point_marker(self):
+    def get_end_point_marker(self) -> PositionMarker:
         """Get a point marker at the end of this segment."""
+        assert self.pos_marker
         return self.pos_marker.end_point_marker()
 
-    def get_start_loc(self):
+    def get_start_loc(self) -> Tuple[int, int]:
         """Get a location tuple at the start of this segment."""
+        assert self.pos_marker
         return self.pos_marker.working_loc
 
-    def get_end_loc(self):
+    def get_end_loc(self) -> Tuple[int, int]:
         """Get a location tuple at the end of this segment."""
+        assert self.pos_marker
         return self.pos_marker.working_loc_after(
             self.raw,
         )
 
-    def stringify(self, ident=0, tabsize=4, code_only=False):
+    def stringify(self, ident=0, tabsize=4, code_only=False) -> str:
         """Use indentation to render this segment and its children as a string."""
         buff = StringIO()
         preface = self._preface(ident=ident, tabsize=tabsize)
         buff.write(preface + "\n")
         if not code_only and self.comment_separate and len(self._comments) > 0:
             if self._comments:  # pragma: no cover TODO?
                 buff.write((" " * ((ident + 1) * tabsize)) + "Comments:" + "\n")
@@ -1007,92 +970,87 @@
                     )
                     for seg in self.segments
                     if include_meta or not seg.is_meta
                 ),
             )
         return result
 
-    def copy(self):
+    def copy(self) -> "BaseSegment":
         """Copy the segment recursively, with appropriate copying of references."""
         new_seg = copy(self)
         # Position markers are immutable, and it's important that we keep
         # a reference to the same TemplatedFile, so keep the same position
         # marker.
         new_seg.pos_marker = self.pos_marker
         if self.segments:
             new_seg.segments = tuple(seg.copy() for seg in self.segments)
         return new_seg
 
-    def as_record(self, **kwargs):
+    def as_record(self, **kwargs) -> Optional[dict]:
         """Return the segment as a structurally simplified record.
 
         This is useful for serialization to yaml or json.
         kwargs passed to to_tuple
         """
         return self.structural_simplify(self.to_tuple(**kwargs))
 
-    def raw_list(self):  # pragma: no cover TODO?
-        """Return a list of raw elements, mostly for testing or searching."""
-        buff = []
-        for s in self.segments:
-            buff += s.raw_list()
-        return buff
-
-    def get_raw_segments(self):
+    def get_raw_segments(self) -> List["RawSegment"]:
         """Iterate raw segments, mostly for searching."""
         return [item for s in self.segments for item in s.raw_segments]
 
-    def iter_segments(self, expanding=None, pass_through=False):
+    def iter_segments(
+        self, expanding=None, pass_through=False
+    ) -> Iterator["BaseSegment"]:
         """Iterate segments, optionally expanding some children."""
         for s in self.segments:
             if expanding and s.is_type(*expanding):
                 yield from s.iter_segments(
                     expanding=expanding if pass_through else None
                 )
             else:
                 yield s
 
-    def iter_unparsables(self):
+    def iter_unparsables(self) -> Iterator["UnparsableSegment"]:
         """Iterate through any unparsables this segment may contain."""
         for s in self.segments:
             yield from s.iter_unparsables()
 
-    def type_set(self):
+    def type_set(self) -> Set[str]:
         """Return a set of the types contained, mostly for testing."""
         typs = {self.type}
         for s in self.segments:
             typs |= s.type_set()
         return typs
 
-    def is_raw(self):
+    def is_raw(self) -> bool:
         """Return True if this segment has no children."""
         return len(self.segments) == 0
 
     def get_child(self, *seg_type):
         """Retrieve the first of the children of this segment with matching type."""
         for seg in self.segments:
             if seg.is_type(*seg_type):
                 return seg
         return None
 
-    def get_children(self, *seg_type):
+    def get_children(self, *seg_type) -> list:
         """Retrieve the all of the children of this segment with matching type."""
         buff = []
         for seg in self.segments:
             if seg.is_type(*seg_type):
                 buff.append(seg)
         return buff
 
     def select_children(
         self,
         start_seg: Optional["BaseSegment"] = None,
         stop_seg: Optional["BaseSegment"] = None,
         select_if: Optional[Callable[["BaseSegment"], Any]] = None,
         loop_while: Optional[Callable[["BaseSegment"], Any]] = None,
-    ):
+    ) -> List["BaseSegment"]:
         """Retrieve subset of children based on range and filters.
 
         Often useful by linter rules when generating fixes, e.g. to find
         whitespace segments between two already known segments.
         """
         start_index = self.segments.index(start_seg) if start_seg else -1
         stop_index = self.segments.index(stop_seg) if stop_seg else len(self.segments)
@@ -1191,35 +1149,31 @@
         # Not found.
         return []  # pragma: no cover
 
     def parse(
         self,
         parse_context: ParseContext,
         parse_grammar: Optional[Matchable] = None,
-    ) -> "BaseSegment":
+    ) -> Tuple["BaseSegment", ...]:
         """Use the parse grammar to find subsegments within this segment.
 
         A large chunk of the logic around this can be found in the `expand` method.
 
         Use the parse setting in the context for testing, mostly to check how deep to
         go. True/False for yes or no, an integer allows a certain number of levels.
 
         Optionally, this method allows a custom parse grammar to be
         provided which will override any existing parse grammar
         on the segment.
         """
-        # Clear the denylist cache so avoid missteps
-        if parse_context:
-            parse_context.denylist.clear()
-
         # the parse_depth and recurse kwargs control how deep we will recurse for
         # testing.
         if not self.segments:  # pragma: no cover TODO?
             # This means we're a root segment, just return an unmutated self
-            return self
+            return (self,)
 
         # Check the Parse Grammar
         parse_grammar = parse_grammar or self.parse_grammar
         if parse_grammar is None:
             # No parse grammar, go straight to expansion
             parse_context.logger.debug(
                 "{}.parse: no grammar. Going straight to expansion".format(
@@ -1244,21 +1198,14 @@
                         f"{segments[idx_non_code].raw!r}.\n{segments!r}"
                     )
 
             # NOTE: No match_depth kwarg, because this is the start of the matching.
             with parse_context.matching_segment(self.__class__.__name__) as ctx:
                 m = parse_grammar.match(segments=segments, parse_context=ctx)
 
-            if not isinstance(m, MatchResult):  # pragma: no cover
-                raise TypeError(
-                    "[PD:{}] {}.match. Result is {}, not a MatchResult!".format(
-                        parse_context.parse_depth, self.__class__.__name__, type(m)
-                    )
-                )
-
             # Basic Validation, that we haven't dropped anything.
             check_still_complete(segments, m.matched_segments, m.unmatched_segments)
 
             if m.has_match():
                 if m.is_complete():
                     # Complete match, happy days!
                     self.segments = pre_nc + m.matched_segments + post_nc
@@ -1311,15 +1258,15 @@
             parse_context.logger.debug(parse_depth_msg)
             with parse_context.deeper_parse() as ctx:
                 self.segments = self.expand(
                     self.segments,
                     parse_context=ctx,
                 )
 
-        return self
+        return (self,)
 
     @staticmethod
     def _is_code_or_meta(segment: "BaseSegment") -> bool:
         return segment.is_code or segment.is_meta
 
     @classmethod
     def _find_start_or_end_non_code(cls, segments) -> Optional[int]:
@@ -1378,15 +1325,15 @@
                                 "Matched fix for %s against segment: %s -> %s",
                                 rule_code,
                                 f,
                                 seg,
                             )
                             if f.edit_type == "delete":
                                 # We're just getting rid of this segment.
-                                seg = None
+                                pass
                             elif f.edit_type in (
                                 "replace",
                                 "create_before",
                                 "create_after",
                             ):
                                 if (
                                     f.edit_type == "create_after"
@@ -1395,30 +1342,28 @@
                                     # in the case of a creation after that is not part
                                     # of a create_before/create_after pair, also add
                                     # this segment before the edit.
                                     seg_buffer.append(seg)
 
                                 # We're doing a replacement (it could be a single
                                 # segment or an iterable)
+                                assert f.edit, f"Edit {f.edit_type!r} requires `edit`."
                                 consumed_pos = False
-                                if isinstance(f.edit, BaseSegment):
-                                    seg_buffer.append(f.edit)  # pragma: no cover TODO?
-                                else:
-                                    for s in f.edit:
-                                        seg_buffer.append(s)
-                                        # If one of them has the same raw representation
-                                        # then the first that matches gets to take the
-                                        # original position marker.
-                                        if (
-                                            f.edit_type == "replace"
-                                            and s.raw == seg.raw
-                                            and not consumed_pos
-                                        ):
-                                            seg_buffer[-1].pos_marker = seg.pos_marker
-                                            consumed_pos = True
+                                for s in f.edit:
+                                    seg_buffer.append(s)
+                                    # If one of them has the same raw representation
+                                    # then the first that matches gets to take the
+                                    # original position marker.
+                                    if (
+                                        f.edit_type == "replace"
+                                        and s.raw == seg.raw
+                                        and not consumed_pos
+                                    ):
+                                        seg_buffer[-1].pos_marker = seg.pos_marker
+                                        consumed_pos = True
 
                                 if f.edit_type == "create_before":
                                     # in the case of a creation before, also add this
                                     # segment on the end
                                     seg_buffer.append(seg)
 
                             else:  # pragma: no cover
@@ -1498,39 +1443,38 @@
             # different segments may compare as equal.
             anchor_id = fix.anchor.uuid
             anchor_info[anchor_id].add(fix)
         return dict(anchor_info)
 
     def _validate_segment_after_fixes(self, rule_code, dialect, fixes_applied, segment):
         """Checks correctness of new segment against match or parse grammar."""
-        root_parse_context = RootParseContext(dialect=dialect)
-        with root_parse_context as parse_context:
-            try:
-                # :HACK: Calling parse() corrupts the segment 'r'
-                # in some cases, e.g. adding additional Dedent child
-                # segments. Here, we work around this by calling
-                # parse() on a "backup copy" of the segment.
-                r_copy = deepcopy(segment)
-                for seg in r_copy.segments:
-                    seg.pos_marker = replace(
-                        seg.pos_marker,
-                        templated_file=self.pos_marker.templated_file,
-                    )
-                r_copy.parse(parse_context)
-            except ValueError:  # pragma: no cover
-                self._log_apply_fixes_check_issue(
-                    "After %s fixes were applied, segment %r failed the "
-                    "parse() check. Fixes: %r",
-                    rule_code,
-                    r_copy,
-                    fixes_applied,
-                )
+        ctx = ParseContext(dialect=dialect)
+        try:
+            # :HACK: Calling parse() corrupts the segment 'r'
+            # in some cases, e.g. adding additional Dedent child
+            # segments. Here, we work around this by calling
+            # parse() on a "backup copy" of the segment.
+            r_copy = deepcopy(segment)
+            for seg in r_copy.segments:
+                seg.pos_marker = replace(
+                    seg.pos_marker,
+                    templated_file=self.pos_marker.templated_file,
+                )
+            r_copy.parse(ctx)
+        except ValueError:  # pragma: no cover
+            self._log_apply_fixes_check_issue(
+                "After %s fixes were applied, segment %r failed the "
+                "parse() check. Fixes: %r",
+                rule_code,
+                r_copy,
+                fixes_applied,
+            )
 
     @staticmethod
-    def _log_apply_fixes_check_issue(message, *args):  # pragma: no cover
+    def _log_apply_fixes_check_issue(message, *args) -> None:  # pragma: no cover
         linter_logger.critical(message, exc_info=True, *args)
 
     def _iter_source_fix_patches(
         self, templated_file: TemplatedFile
     ) -> Iterator[FixPatch]:
         """Yield any source patches as fixes now.
 
@@ -1608,16 +1552,18 @@
             while segments and segments[-1].is_type("end_of_file", "indent"):
                 segments = segments[:-1]
 
             # Iterate through the child segments
             source_idx = self.pos_marker.source_slice.start
             templated_idx = self.pos_marker.templated_slice.start
             insert_buff = ""
-            for seg_idx, segment in enumerate(segments):
+            for segment in segments:
                 # First check for insertions.
+                # At this stage, everything should have a position.
+                assert segment.pos_marker
                 # We know it's an insertion if it has length but not in the templated
                 # file.
                 if segment.raw and segment.pos_marker.is_point():
                     # Add it to the insertion buffer if it has length:
                     if segment.raw:
                         insert_buff += segment.raw
                         linter_logger.debug(
@@ -1714,16 +1660,16 @@
     def __init__(
         self,
         *args,
         # These are tuples of segments but we're expecting them to
         # be tuples of length 1. This is because we'll almost always
         # be doing tuple arithmetic with the results and constructing
         # 1-tuples on the fly is very easy to misread.
-        start_bracket: Optional[Tuple[BaseSegment]] = None,
-        end_bracket: Optional[Tuple[BaseSegment]] = None,
+        start_bracket: Tuple[BaseSegment],
+        end_bracket: Tuple[BaseSegment],
         **kwargs,
     ):
         """Stash the bracket segments for later."""
         if not start_bracket or not end_bracket:  # pragma: no cover
             raise ValueError(
                 "Attempted to construct Bracketed segment without specifying brackets."
             )
@@ -1737,15 +1683,15 @@
         start_brackets = [
             start_bracket
             for _, start_bracket, _, persistent in parse_context.dialect.sets(
                 "bracket_pairs"
             )
             if persistent
         ]
-        simple_raws = set()
+        simple_raws: Set[str] = set()
         for ref in start_brackets:
             bracket_simple = parse_context.dialect.ref(ref).simple(
                 parse_context, crumbs=crumbs
             )
             assert bracket_simple, "All bracket segments must support simple."
             assert bracket_simple[0], "All bracket segments must support raw simple."
             # NOTE: By making this assumption we don't have to handle the "typed"
@@ -1767,26 +1713,26 @@
     """This is a segment which can't be parsed. It indicates a error during parsing."""
 
     type = "unparsable"
     # From here down, comments are printed separately.
     comment_separate = True
     _expected = ""
 
-    def __init__(self, *args, expected="", **kwargs):
+    def __init__(self, *args, expected="", **kwargs) -> None:
         self._expected = expected
         super().__init__(*args, **kwargs)
 
-    def _suffix(self):
+    def _suffix(self) -> str:
         """Return any extra output required at the end when logging.
 
         NB Override this for specific subclasses if we want extra output.
         """
         return f"!! Expected: {self._expected!r}"
 
-    def iter_unparsables(self):
+    def iter_unparsables(self) -> Iterator["UnparsableSegment"]:
         """Iterate through any unparsables.
 
         As this is an unparsable, it should yield itself.
         """
         yield self
 
 
@@ -1810,19 +1756,19 @@
         pos_marker=None,
         fname: Optional[str] = None,
     ):
         self._file_path = fname
         super().__init__(segments, pos_marker=pos_marker)
 
     @property
-    def file_path(self):
+    def file_path(self) -> Optional[str]:
         """File path of a parsed SQL file."""
         return self._file_path
 
-    def get_table_references(self):
+    def get_table_references(self) -> set:
         """Use parsed tree to extract table references."""
         references = set()
         for stmt in self.get_children("statement"):
             references |= stmt.get_table_references()
         return references
 
 
@@ -1833,37 +1779,37 @@
     where different object instances may compare as equal.
 
     Copied from: https://stackoverflow.com/questions/16994307/identityset-in-python
     """
 
     key = id  # should return a hashable object
 
-    def __init__(self, iterable=()):
-        self.map = {}  # id -> object
+    def __init__(self, iterable=()) -> None:
+        self.map: dict = {}  # id -> object
         self |= iterable  # add elements from iterable to the set (union)
 
-    def __len__(self):  # Sized
+    def __len__(self) -> int:  # Sized
         return len(self.map)
 
     def __iter__(self):  # Iterable
         return self.map.values().__iter__()  # pragma: no cover
 
     def __contains__(self, x):  # Container
         return self.key(x) in self.map
 
     def add(self, value):  # MutableSet
         """Add an element."""
         self.map[self.key(value)] = value
 
-    def update(self, value):
+    def update(self, value) -> None:
         """Add elements in 'value'."""
         for v in value:
             self.add(v)
 
     def discard(self, value):  # MutableSet
         """Remove an element.  Do not raise an exception if absent."""
         self.map.pop(self.key(value), None)  # pragma: no cover
 
-    def __repr__(self):  # pragma: no cover
+    def __repr__(self) -> str:  # pragma: no cover
         if not self:
             return "%s()" % (self.__class__.__name__,)
         return "%s(%r)" % (self.__class__.__name__, list(self))
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 """Ephemeral segment definitions."""
 
 import copy
 import logging
+from typing import Optional, Tuple, TYPE_CHECKING
 
 from sqlfluff.core.parser.match_result import MatchResult
+from sqlfluff.core.parser.match_wrapper import MatchFuncType
 from sqlfluff.core.parser.segments.base import BaseSegment
 
+if TYPE_CHECKING:  # pragma: no cover
+    from sqlfluff.core.parser.context import ParseContext
+    from sqlfluff.core.parser.markers import PositionMarker
+    from sqlfluff.core.parser.matchable import Matchable
+    from sqlfluff.core.parser.grammar.base import BaseGrammar
+
 
 parser_logger = logging.getLogger("sqlfluff.parser")
 
 
 class EphemeralSegment(BaseSegment):
     """A segment which acts like a normal segment, but is ephemeral.
 
@@ -17,62 +25,79 @@
     a normal segment except that during the `parse` step, it returns its
     contents rather than itself. This means in the final parsed structure
     it no longer exists.
     """
 
     type = "ephemeral"
 
-    def __init__(self, segments, pos_marker, parse_grammar, ephemeral_name: str):
+    def __init__(
+        self,
+        segments: Tuple[BaseSegment, ...],
+        pos_marker: Optional["PositionMarker"],
+        parse_grammar: "Matchable",
+        ephemeral_name: str,
+    ):
         # Stash the parse grammar for now.
         self._parse_grammar = parse_grammar
         self.ephemeral_name = ephemeral_name
         super().__init__(segments, pos_marker=pos_marker)
 
     @property
     def expected_form(self) -> str:
         """What to return to the user when unparsable."""
         return self.ephemeral_name
 
     @property
-    def is_expandable(self):
+    def is_expandable(self) -> bool:
         """Ephemeral segments are always expandable.
 
         They should dissolve after expansion. So if it exists, it's expandable.
         We need to redefine this here because the usual introspection doesn't
         handle the custom parse_grammar properly.
         """
         return True
 
-    def parse(self, parse_context):
+    def parse(
+        self, parse_context: "ParseContext", parse_grammar: Optional["Matchable"] = None
+    ) -> Tuple[BaseSegment, ...]:
         """Use the parse grammar to find subsegments within this segment.
 
         Return the content of the result, rather than itself.
         """
         # Call the usual parse function, but overriding the parse grammar.
-        new_self = super().parse(parse_context, parse_grammar=self._parse_grammar)
+        parsed_segments = super().parse(
+            parse_context, parse_grammar=self._parse_grammar
+        )
+
+        # Check we only got a result of length 1.
+        assert len(parsed_segments) == 1
         # Return the content of that result rather than self
-        return new_self.segments
+        return parsed_segments[0].segments
 
 
-def allow_ephemeral(func):
+def allow_ephemeral(func: MatchFuncType) -> MatchFuncType:
     """Wraps a .match() method to the option of ephemeral matching for grammars.
 
     This is designed to be used as follows:
 
         class SomeMatchableObject(object):
             @match_wrapper()
             @allow_ephemeral
             def match(self, segments, parse_context):
                 ...
                 return m
 
     NOTE: This should come inside the match_wrapper.
     """
 
-    def wrapped_match_method(self, segments: tuple, parse_context):
+    def wrapped_match_method(
+        self: "BaseGrammar",
+        segments: Tuple[BaseSegment, ...],
+        parse_context: "ParseContext",
+    ) -> MatchResult:
         """A wrapper on the match function to do some basic validation."""
         # Use the ephemeral_segment if present. This should only
         # be the case for grammars where `ephemeral_name` is defined.
         if self.ephemeral_name:
             # We're going to return as though it's a full match, similar to Anything().
             new_grammar = copy.copy(self)
             # Reset the ephemeral name on the new version of the grammar otherwise
@@ -96,10 +121,10 @@
                             parse_grammar=new_grammar,
                             ephemeral_name=self.ephemeral_name,
                         ),
                     )
                 )
         else:
             # Otherwise carry on through with wrapping the function.
-            return func(self, segments, parse_context=parse_context)
+            return func(self, segments, parse_context)
 
     return wrapped_match_method
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     It returns a single dialect object on expansion.
 
     These are defined using a callable, which is only called
     once everything else is defined. Very useful for template
     inheritance.
     """
 
-    def __init__(self, func):
+    def __init__(self, func) -> None:
         self.func = func
 
     # For all functions, use the function call
     def expand(self, dialect):
         """Expand this object into its true dialect object.
 
         The inner function is passed an instance of the current dialect
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Indent and Dedent classes."""
 
 from uuid import UUID
 
 from sqlfluff.core.parser.markers import PositionMarker
+from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.match_wrapper import match_wrapper
 from sqlfluff.core.parser.segments.raw import RawSegment, SourceFix
 from sqlfluff.core.parser.context import ParseContext
 from typing import Optional, List
 
 from sqlfluff.core.templaters.base import TemplatedFile
 
@@ -42,33 +43,33 @@
                 template (e.g. the beginning and end of an if
                 statement).
         """
         super().__init__(*args, **kwargs)
         self.is_template = is_template
         self.block_uuid = block_uuid
 
-    def _suffix(self):
+    def _suffix(self) -> str:
         """Return any extra output required at the end when logging.
 
         Meta classes have not much to say here so just stay blank.
         """
         return ""
 
     @classmethod
     @match_wrapper()
-    def match(cls, segments, parse_context):  # pragma: no cover
+    def match(cls, segments, parse_context) -> MatchResult:  # pragma: no cover
         """This will never be called. If it is then we're using it wrong."""
         raise NotImplementedError(
             "{} has no match method, it should only be used in a Sequence!".format(
                 cls.__name__
             )
         )
 
     @classmethod
-    def simple(cls, parse_context: ParseContext, crumbs=None):
+    def simple(cls, parse_context: ParseContext, crumbs=None) -> None:
         """Does this matcher support an uppercase hash matching route?
 
         This should be true if the MATCH grammar is simple. Most more
         complicated segments will be assumed to overwrite this method
         if they wish to be considered simple.
         """
         return None
@@ -206,15 +207,15 @@
         return cls(
             pos_marker=pos_marker,
             source_str=templated_file.source_str[source_slice],
             block_type=block_type,
             block_uuid=block_uuid,
         )
 
-    def to_tuple(self, code_only=False, show_raw=False, include_meta=False):
+    def to_tuple(self, code_only=False, show_raw=False, include_meta=False) -> tuple:
         """Return a tuple structure from this segment.
 
         Unlike most segments, we return the _source_ content for placeholders
         if viewing metas is allowed. This allows verification of the content
         of those placeholders for inspection or debugging.
         """
         if include_meta:
@@ -223,15 +224,15 @@
             return (self.get_type(), self.raw)
 
     def edit(
         self,
         raw: Optional[str] = None,
         source_fixes: Optional[List[SourceFix]] = None,
         source_str: Optional[str] = None,
-    ):
+    ) -> MetaSegment:
         """Create a new segment, with exactly the same position but different content.
 
         Returns:
             A copy of this object with new contents.
 
         Used mostly by fixes.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.2.0/src/sqlfluff/core/parser/segments/raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Raw segment definitions.
 
 This is designed to be the root segment, without
 any children, and the output of the lexer.
 """
 
-from typing import List, Optional, Tuple, Set
+from typing import Any, List, Optional, Tuple, Set
 from uuid import UUID, uuid4
 
 from sqlfluff.core.parser.segments.base import BaseSegment, SourceFix
 from sqlfluff.core.parser.markers import PositionMarker
 
 
 class RawSegment(BaseSegment):
@@ -43,14 +43,16 @@
         else:
             self._raw = self._default_raw
         self._raw_upper = self._raw.upper()
         # pos marker is required here. We ignore the typing initially
         # because it might *initially* be unset, but it will be reset
         # later.
         self.pos_marker: PositionMarker = pos_marker  # type: ignore
+        # Set the segments attribute to be an empty tuple.
+        self.segments = ()
         # if a surrogate type is provided, store it for later.
         self._surrogate_type = type
         # What should we trim off the ends to get to content
         self.trim_start = trim_start
         self.trim_chars = trim_chars
         # A cache variable for expandable
         self._is_expandable = None
@@ -58,75 +60,67 @@
         self._source_fixes = source_fixes
         # UUID for matching
         self.uuid = uuid or uuid4()
         self.representation = "<{}: ({}) {!r}>".format(
             self.__class__.__name__, self.pos_marker, self.raw
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         # This is calculated at __init__, because all elements are immutable
         # and this was previously recalculating the pos marker,
         # and became very expensive
         return self.representation
 
-    def __setattr__(self, key, value):
+    def __setattr__(self, key: str, value: Any) -> None:
         """Overwrite BaseSegment's __setattr__ with BaseSegment's superclass."""
         super(BaseSegment, self).__setattr__(key, value)
 
     # ################ PUBLIC PROPERTIES
 
     @property
-    def matched_length(self):
+    def matched_length(self) -> int:
         """Return the length of the segment in characters."""
         return len(self._raw)
 
     @property
-    def is_expandable(self):
+    def is_expandable(self) -> bool:
         """Return true if it is meaningful to call `expand` on this segment."""
         return False
 
     @property
-    def is_code(self):
+    def is_code(self) -> bool:
         """Return True if this segment is code."""
         return self._is_code
 
     @property
-    def is_comment(self):
+    def is_comment(self) -> bool:
         """Return True if this segment is a comment."""
         return self._is_comment
 
     @property
-    def is_whitespace(self):
+    def is_whitespace(self) -> bool:
         """Return True if this segment is whitespace."""
         return self._is_whitespace
 
     @property
-    def raw(self):
+    def raw(self) -> str:
         """Returns the raw segment."""
         return self._raw
 
     @property
-    def raw_upper(self):
+    def raw_upper(self) -> str:
         """Returns the raw segment in uppercase."""
         return self._raw_upper
 
     @property
-    def raw_segments(self):
+    def raw_segments(self) -> List["RawSegment"]:
         """Returns self to be compatible with calls to its superclass."""
         return [self]
 
     @property
-    def segments(self):
-        """Return an empty list of child segments.
-
-        This is in case something tries to iterate on this segment.
-        """
-        return []
-
-    @property
     def class_types(self) -> Set[str]:
         """The set of full types for this segment, including inherited.
 
         Add the surrogate type for raw segments.
         """
         return (
             {self._surrogate_type} if self._surrogate_type else set()
@@ -135,33 +129,33 @@
     @property
     def source_fixes(self) -> List[SourceFix]:
         """Return any source fixes as list."""
         return self._source_fixes or []
 
     # ################ INSTANCE METHODS
 
-    def invalidate_caches(self):
+    def invalidate_caches(self) -> None:
         """Overwrite superclass functionality."""
         pass
 
-    def get_type(self):
+    def get_type(self) -> str:
         """Returns the type of this segment as a string."""
         return self._surrogate_type or self.type
 
-    def is_type(self, *seg_type):
+    def is_type(self, *seg_type) -> bool:
         """Extend the parent class method with the surrogate types."""
         if self._surrogate_type and self._surrogate_type in seg_type:
             return True
         return self.class_is_type(*seg_type)
 
-    def get_raw_segments(self):
+    def get_raw_segments(self) -> List["RawSegment"]:
         """Iterate raw segments, mostly for searching."""
         return [self]
 
-    def raw_trimmed(self):
+    def raw_trimmed(self) -> str:
         """Return a trimmed version of the raw content."""
         raw_buff = self.raw
         if self.trim_start:
             for seq in self.trim_start:
                 if raw_buff.startswith(seq):
                     raw_buff = raw_buff[len(seq) :]
         if self.trim_chars:
@@ -173,33 +167,31 @@
                     raw_buff = raw_buff[len(seq) :]
                 # trim end
                 while raw_buff.endswith(seq):
                     raw_buff = raw_buff[: -len(seq)]
             return raw_buff
         return raw_buff
 
-    def raw_list(self):  # pragma: no cover TODO?
-        """Return a list of the raw content of this segment."""
-        return [self.raw]
-
-    def stringify(self, ident=0, tabsize=4, code_only=False):
+    def stringify(
+        self, ident: int = 0, tabsize: int = 4, code_only: bool = False
+    ) -> str:
         """Use indentation to render this segment and its children as a string."""
         preface = self._preface(ident=ident, tabsize=tabsize)
         return preface + "\n"
 
-    def _suffix(self):
+    def _suffix(self) -> str:
         """Return any extra output required at the end when logging.
 
         NB Override this for specific subclasses if we want extra output.
         """
         return f"{self.raw!r}"
 
     def edit(
         self, raw: Optional[str] = None, source_fixes: Optional[List[SourceFix]] = None
-    ):
+    ) -> "RawSegment":
         """Create a new segment, with exactly the same position but different content.
 
         Returns:
             A copy of this object with new contents.
 
         Used mostly by fixes.
 
@@ -290,15 +282,17 @@
         super().__init__(
             raw=raw,
             pos_marker=pos_marker,
             type=type,
             source_fixes=source_fixes,
         )
 
-    def edit(self, raw=None, source_fixes=None):
+    def edit(
+        self, raw: Optional[str] = None, source_fixes: Optional[List[SourceFix]] = None
+    ) -> "KeywordSegment":
         """Create a new segment, with exactly the same position but different content.
 
         Returns:
             A copy of this object with new contents.
 
         Used mostly by fixes.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.2.0/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.2.0/src/sqlfluff/core/plugin/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Base implementation for the plugin."""
 
-import os.path
-
-from typing import List, Type
+from typing import List, Type, Dict, Any
 
 from sqlfluff.core.config import ConfigLoader
 from sqlfluff.core.plugin import hookimpl
 from sqlfluff.core.rules.config_info import STANDARD_CONFIG_INFO_DICT
 from sqlfluff.core.rules.loader import get_rules_from_path
 from sqlfluff.core.rules import BaseRule
 from sqlfluff.core.templaters import core_templaters, RawTemplater
@@ -22,23 +20,24 @@
     """
     return get_rules_from_path()
 
 
 @hookimpl
 def get_templaters() -> List[Type[RawTemplater]]:
     """Get templaters."""
-    return core_templaters()
+    templaters = list(t for t in core_templaters())
+    return templaters
 
 
 @hookimpl
-def load_default_config() -> dict:
+def load_default_config() -> Dict[str, Any]:
     """Loads the default configuration for the plugin."""
-    return ConfigLoader.get_global().load_config_file(
-        file_dir=os.path.join(os.path.dirname(os.path.dirname(__file__))),
+    return ConfigLoader.get_global().load_config_resource(
+        package="sqlfluff.core",
         file_name="default_config.cfg",
     )
 
 
 @hookimpl
-def get_configs_info() -> dict:
+def get_configs_info() -> Dict[str, Any]:
     """Get rule config validations and descriptions."""
     return STANDARD_CONFIG_INFO_DICT
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     EvalResultType,
 )
 from sqlfluff.core.rules.context import RuleContext
 from sqlfluff.core.rules.config_info import STANDARD_CONFIG_INFO_DICT
 from sqlfluff.core.plugin.host import get_plugin_manager
 
 
-def _load_standard_rules():
+def _load_standard_rules() -> RuleSet:
     """Initialise the standard ruleset.
 
     We do this on each call so that dynamic rules changes
     are possible.
     """
     std_rule_set = RuleSet(name="standard", config_info=STANDARD_CONFIG_INFO_DICT)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,25 @@
     Dict,
     Type,
     DefaultDict,
     Iterator,
 )
 from collections import namedtuple, defaultdict
 
-from sqlfluff.core.config import FluffConfig, split_comma_separated_string
+from sqlfluff.core.config import split_comma_separated_string
 
-from sqlfluff.core.linter import LintedFile, NoQaDirective
+from sqlfluff.core.linter import IgnoreMask
 from sqlfluff.core.parser import BaseSegment, PositionMarker, RawSegment
 from sqlfluff.core.dialects import Dialect
 from sqlfluff.core.errors import SQLLintError, SQLFluffUserError
 from sqlfluff.core.parser.segments.base import SourceFix
 from sqlfluff.core.rules.context import RuleContext
 from sqlfluff.core.rules.crawlers import BaseCrawler
 from sqlfluff.core.rules.config_info import get_config_info
+from sqlfluff.core.plugin.host import plugins_loaded, is_main_process
 from sqlfluff.core.templaters.base import RawFileSlice, TemplatedFile
 
 # The ghost of a rule (mostly used for testing)
 RuleGhost = namedtuple("RuleGhost", ["code", "name", "description"])
 
 # Instantiate the rules logger
 rules_logger = logging.getLogger("sqlfluff.rules")
@@ -204,28 +205,28 @@
                     )
                     seg.pos_marker = None
             # Once stripped, we shouldn't replace any markers because
             # later code may rely on them being accurate, which we
             # can't guarantee with edits.
         self.source = [seg for seg in source if seg.pos_marker] if source else []
 
-    def is_trivial(self):
+    def is_trivial(self) -> bool:
         """Return true if the fix is trivial.
 
         Trivial edits are:
         - Anything of zero length.
         - Any edits which result in themselves.
 
         Removing these makes the routines which process fixes much faster.
         """
         if self.edit_type in ("create_before", "create_after"):
             if isinstance(self.edit, BaseSegment):
                 if len(self.edit.raw) == 0:  # pragma: no cover TODO?
                     return True
-            elif all(len(elem.raw) == 0 for elem in self.edit):
+            elif self.edit and all(len(elem.raw) == 0 for elem in self.edit):
                 return True
         elif self.edit_type == "replace" and self.edit == self.anchor:
             return True  # pragma: no cover TODO?
         return False
 
     def is_just_source_edit(self) -> bool:
         """Return whether this a valid source only edit."""
@@ -255,15 +256,15 @@
         else:
             detail = ""  # pragma: no cover TODO?
         return (
             f"<LintFix: {self.edit_type} {self.anchor.get_type()}"
             f"@{self.anchor.pos_marker} {detail}>"
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """Compare equality with another fix.
 
         A fix is equal to another if is in the same place (position), with the
         same type and (if appropriate) the same edit values.
 
         """
         if not self.edit_type == other.edit_type:
@@ -497,15 +498,15 @@
         "(\\s{4}\\*\\*Anti-pattern\\*\\*|\\s{4}\\.\\. note::|"
         "\\s\\s{4}\\*\\*Configuration\\*\\*)",
         flags=re.MULTILINE,
     )
     _valid_classname_regex = regex.compile(r"Rule_?([A-Z]{1}[a-zA-Z]+)?_([A-Z0-9]{4})")
     _valid_rule_name_regex = regex.compile(r"[a-z][a-z\.\_]+")
 
-    def _populate_code_and_description(mcs, name, class_dict):
+    def _populate_code_and_description(mcs, name, class_dict) -> dict:
         """Extract and validate the rule code & description.
 
         We expect that rules are defined as classes with the name `Rule_XXXX`
         where `XXXX` is of the form `LLNN`, where L is a letter and N is a
         two digit number. For backward compatibility we also still support
         the legacy format of LNNN i.e. a single letter and three digit number.
 
@@ -567,15 +568,37 @@
         groups_docs = (
             ("    **Groups**: ``" + "``, ``".join(class_dict["groups"]) + "``\n\n")
             if class_dict.get("groups", [])
             else ""
         )
 
         config_docs = ""
-        if class_dict.get("config_keywords", []):
+
+        # NOTE: We should only validate and add config keywords
+        # into the docstring if the plugin loading methods have
+        # fully completed (i.e. plugins_loaded.get() is True).
+        if name == "BaseRule" or not is_main_process.get():
+            # Except if it's the base rule, or we're not in the main process/thread
+            # in which case we shouldn't try and alter the docstrings anyway.
+            # NOTE: The order of imports within child threads/processes is less
+            # controllable, and so we should just avoid checking whether plugins
+            # are already loaded.
+            pass
+        elif not plugins_loaded.get():
+            # Show a warning if a plugin has their imports set up in a suboptimal
+            # way. The example plugin imports the rules in both ways, to test the
+            # triggering of this warning.
+            rules_logger.warning(
+                f"Rule {name!r} has been imported before all plugins "
+                "have been fully loaded. For best performance, plugins "
+                "should import any rule definitions within their `get_rules()` "
+                "method. Please update your plugin to remove this warning. See: "
+                "https://docs.sqlfluff.com/en/stable/developingplugins.html"
+            )
+        elif class_dict.get("config_keywords", []):
             config_docs = "\n    **Configuration**\n"
             config_info = get_config_info()
             for keyword in sorted(class_dict["config_keywords"]):
                 try:
                     info_dict = config_info[keyword]
                 except KeyError:  # pragma: no cover
                     raise KeyError(
@@ -697,15 +720,15 @@
     # a line to the docstring.
     is_fix_compatible = False
 
     # Add comma separated string to Base Rule to ensure that it uses the same
     # Configuration that is defined in the Config.py file
     split_comma_separated_string = staticmethod(split_comma_separated_string)
 
-    def __init__(self, code, description, **kwargs):
+    def __init__(self, code, description, **kwargs) -> None:
         self.description = description
         self.code = code
         # kwargs represents the config passed to the rule. Add all kwargs as class
         # attributes so they can be accessed in rules which inherit from this class
         for key, value in kwargs.items():
             self.__dict__[key] = value
 
@@ -720,15 +743,15 @@
                         "Unrecognized config '{}' for Rule {}. If this "
                         "is a new option, please add it to "
                         "`default_config.cfg`"
                     ).format(keyword, code)
                 )
 
     @classmethod
-    def get_config_ref(cls):
+    def get_config_ref(cls) -> str:
         """Return the config lookup ref for this rule.
 
         If a `name` is defined, it's the name - otherwise the code.
 
         The name is a much more understandable reference and so makes config
         files more readable. For backward compatibility however we also support
         the rule code for those without names.
@@ -762,17 +785,17 @@
 
     def crawl(
         self,
         tree: BaseSegment,
         dialect: Dialect,
         fix: bool,
         templated_file: Optional["TemplatedFile"],
-        ignore_mask: List[NoQaDirective],
+        ignore_mask: Optional[IgnoreMask],
         fname: Optional[str],
-        config: FluffConfig,
+        config,
     ) -> Tuple[List[SQLLintError], Tuple[RawSegment, ...], List[LintFix], Any]:
         """Run the rule on a given tree.
 
         Returns:
             A tuple of (vs, raw_stack, fixes, memory)
 
         """
@@ -877,15 +900,21 @@
     # HELPER METHODS --------
     @staticmethod
     def _log_critical_errors(error: Exception):  # pragma: no cover
         """This method is monkey patched into a "raise" for certain tests."""
         pass
 
     def _process_lint_result(
-        self, res, templated_file, ignore_mask, new_lerrs, new_fixes, root
+        self,
+        res: LintResult,
+        templated_file: Optional[TemplatedFile],
+        ignore_mask: Optional[IgnoreMask],
+        new_lerrs: List[SQLLintError],
+        new_fixes: List[LintFix],
+        root: BaseSegment,
     ):
         # Unless the rule declares that it's already template safe. Do safety
         # checks.
         if not self.template_safe_fixes:
             self.discard_unsafe_fixes(res, templated_file)
         lerr = res.to_linting_error(rule=self)
         ignored = False
@@ -917,37 +946,39 @@
                         [ps.segment for ps in parent_stack],
                     )
                     lerr = None
                     ignored = True
                     break
 
             if lerr and ignore_mask:
-                filtered = LintedFile.ignore_masked_violations([lerr], ignore_mask)
+                filtered = ignore_mask.ignore_masked_violations([lerr])
                 if not filtered:
                     lerr = None
                     ignored = True
         if lerr:
             new_lerrs.append(lerr)
         if not ignored:
             new_fixes.extend(res.fixes)
 
     @staticmethod
-    def filter_meta(segments, keep_meta=False):
+    def filter_meta(segments, keep_meta=False) -> tuple:
         """Filter the segments to non-meta.
 
         Or optionally the opposite if keep_meta is True.
         """
         buff = []
         for elem in segments:
             if elem.is_meta is keep_meta:
                 buff.append(elem)
         return tuple(buff)
 
     @classmethod
-    def get_parent_of(cls, segment, root_segment):  # pragma: no cover TODO?
+    def get_parent_of(
+        cls, segment: BaseSegment, root_segment: BaseSegment
+    ):  # pragma: no cover TODO?
         """Return the segment immediately containing segment.
 
         NB: This is recursive.
 
         Args:
             segment: The segment to look for.
             root_segment: Some known parent of the segment
@@ -1037,15 +1068,15 @@
 
     @staticmethod
     def _choose_anchor_segment(
         root_segment: BaseSegment,
         edit_type: str,
         segment: BaseSegment,
         filter_meta: bool = False,
-    ):
+    ) -> BaseSegment:
         """Choose the anchor point for a lint fix, i.e. where to apply the fix.
 
         From a grammar perspective, segments near the leaf of the tree are
         generally less likely to allow general edits such as whitespace
         insertion.
 
         This function avoids such issues by taking a proposed anchor point
@@ -1077,15 +1108,15 @@
             children_lists: List[List[BaseSegment]] = []
             if filter_meta:
                 # Optionally check against filtered (non-meta only) children.
                 children_lists.append(
                     [child for child in seg.segments if not child.is_meta]
                 )
             # Always check against the full set of children.
-            children_lists.append(seg.segments)
+            children_lists.append(list(seg.segments))
             children: List[BaseSegment]
             for children in children_lists:
                 if edit_type == "create_before" and children[0] is child:
                     linter_logger.debug(
                         "Hoisting anchor from before %s to %s", anchor, seg
                     )
                     anchor = seg
@@ -1171,15 +1202,15 @@
     """
 
     def __init__(self, name, config_info) -> None:
         self.name = name
         self.config_info = config_info
         self._register: Dict[str, RuleManifest] = {}
 
-    def _validate_config_options(self, config, rule_ref: Optional[str] = None):
+    def _validate_config_options(self, config, rule_ref: Optional[str] = None) -> None:
         """Ensure that all config options are valid.
 
         Config options can also be checked for a specific rule e.g CP01.
         """
         rule_config = config.get_section("rules")
         for config_name, info_dict in self.config_info.items():
             config_option = (
@@ -1467,12 +1498,12 @@
             # Allow variable substitution in making the description
             kwargs["description"] = self._register[code].description.format(**kwargs)
             # Instantiate when ready
             instantiated_rules.append(rule_class(**kwargs))
 
         return RulePack(instantiated_rules, reference_map)
 
-    def copy(self):
+    def copy(self) -> "RuleSet":
         """Return a copy of self with a separate register."""
         new_ruleset = copy.copy(self)
         new_ruleset._register = self._register.copy()
         return new_ruleset
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/config_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 on valid inputs and definitions.
 
 This mapping is used to validate rule config inputs, as well
 as document rule configuration.
 """
 
 from sqlfluff.core.plugin.host import get_plugin_manager
+from typing import Any, Dict
 
 STANDARD_CONFIG_INFO_DICT = {
     "tab_space_size": {
         "validation": range(100),
         "definition": (
             "The number of spaces to consider equal to one tab. "
             "Used in the fixing step of this rule."
@@ -211,14 +212,14 @@
     "preferred_type_casting_style": {
         "validation": ["consistent", "shorthand", "convert", "cast"],
         "definition": ("The expectation for using sql type casting"),
     },
 }
 
 
-def get_config_info() -> dict:
+def get_config_info() -> Dict[str, Any]:
     """Gets the config from core sqlfluff and sqlfluff plugins and merges them."""
     plugin_manager = get_plugin_manager()
     configs_info = plugin_manager.hook.get_configs_info()
     return {
         k: v for config_info_dict in configs_info for k, v in config_info_dict.items()
     }
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/crawlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 from sqlfluff.core.rules.context import RuleContext
 
 
 class BaseCrawler(ABC):
     """The base interface for crawler classes."""
 
-    def __init__(self, works_on_unparsable: bool = False, **kwargs):
+    def __init__(self, works_on_unparsable: bool = False, **kwargs) -> None:
         self.works_on_unparsable = works_on_unparsable
 
-    def passes_filter(self, segment: BaseSegment):
+    def passes_filter(self, segment: BaseSegment) -> bool:
         """Returns true if this segment considered at all.
 
         This method is called during crawling but also
         in evaluating the anchors for linting violations
         and their fixes to make sure we don't get issues
         with linting sections of queries that we can't
         parse.
@@ -46,15 +46,15 @@
 
 class SegmentSeekerCrawler(BaseCrawler):
     """A crawler that efficiently searches for specific segment types.
 
     The segment type(s) are specified on creation.
     """
 
-    def __init__(self, types: Set[str], provide_raw_stack=False, **kwargs):
+    def __init__(self, types: Set[str], provide_raw_stack=False, **kwargs) -> None:
         self.types = types
         # Tracking a raw stack involves a lot of tuple manipulation, so we
         # only do it when required - otherwise we skip it. Rules can explicitly
         # request it when defining their crawler.
         self.provide_raw_stack = provide_raw_stack
         super().__init__(**kwargs)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 def get_rules_from_path(
     # All rule files are expected in the format of L*.py
     rules_path=os.path.abspath(
         os.path.join(os.path.dirname(__file__), "../../rules", "L*.py")
     ),
-    base_module="sqlfluff.rules",
-):
+    base_module: str = "sqlfluff.rules",
+) -> list:
     """Reads all of the Rule classes from a path into a list."""
     # Create a rules dictionary for importing in
     # sqlfluff/src/sqlfluff/core/rules/__init__.py
     rules = []
 
     for module in sorted(glob(rules_path)):
         # Manipulate the module path to extract the filename without the .py
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.2.0/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.2.0/src/sqlfluff/core/slice_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     """Convert a slice into a tuple of (start, stop)."""
     assert s.start is not None and s.stop is not None
     return (s.start, s.stop)
 
 
 def slice_length(s: slice) -> int:
     """Get the length of a slice."""
-    return s.stop - s.start
+    length: int = s.stop - s.start
+    return length
 
 
 def is_zero_slice(s: slice) -> bool:
     """Return true if this is a zero slice."""
-    return s.stop == s.start
+    is_zero: bool = s.stop == s.start
+    return is_zero
 
 
 def zero_slice(i: int) -> slice:
     """Construct a zero slice from a single integer."""
     return slice(i, i)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.2.0/src/sqlfluff/core/string_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def frame_msg(msg: str) -> str:
     """Frame a message with hashes so that it covers five lines."""
     return f"\n###\n#\n# {msg}\n#\n###"
 
 
-def curtail_string(s: str, length=20) -> str:
+def curtail_string(s: str, length: int = 20) -> str:
     """Trim a string nicely to length."""
     if len(s) > length:
         return s[:length] + "..."
     else:
         return s
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 # Although these shouldn't usually be instantiated from here
 # we import them to make sure they get registered.
 from sqlfluff.core.templaters.base import RawTemplater, RawFileSlice
 from sqlfluff.core.templaters.jinja import JinjaTemplater
 from sqlfluff.core.templaters.python import PythonTemplater
 from sqlfluff.core.templaters.placeholder import PlaceholderTemplater
+from typing import Iterator, Type
 
 
-def core_templaters():
+def core_templaters() -> Iterator[Type[RawTemplater]]:
     """Returns the templater tuples for the core templaters."""
     yield from [RawTemplater, JinjaTemplater, PythonTemplater, PlaceholderTemplater]
 
 
 __all__ = (
     "RawFileSlice",
     "TemplatedFile",
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,23 @@
     raw: str  # Source string
     slice_type: str
     source_idx: int  # Offset from beginning of source string
     slice_subtype: Optional[str] = None
     # Block index, incremented on start or end block tags, e.g. "if", "for"
     block_idx: int = 0
 
-    def end_source_idx(self):
+    def end_source_idx(self) -> int:
         """Return the closing index of this slice."""
         return self.source_idx + len(self.raw)
 
-    def source_slice(self):
+    def source_slice(self) -> slice:
         """Return the a slice object for this slice."""
         return slice(self.source_idx, self.end_source_idx())
 
-    def is_source_only_slice(self):
+    def is_source_only_slice(self) -> bool:
         """Based on its slice_type, does it only appear in the *source*?
 
         There are some slice types which are automatically source only.
         There are *also* some which are source only because they render
         to an empty string.
         """
         # TODO: should any new logic go here?
@@ -199,22 +199,22 @@
             if tfs.templated_slice.stop != len(templated_str):
                 raise SQLFluffSkipFile(  # pragma: no cover
                     "Length of templated file mismatch with final slice: "
                     f"{len(templated_str)} != {tfs.templated_slice.stop}."
                 )
 
     @classmethod
-    def from_string(cls, raw):
+    def from_string(cls, raw) -> "TemplatedFile":
         """Create TemplatedFile from a string."""
         return cls(source_str=raw, fname="<string>")
 
-    def __repr__(self):  # pragma: no cover TODO?
+    def __repr__(self) -> str:  # pragma: no cover TODO?
         return "<TemplatedFile>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return the templated file if coerced to string."""
         return self.templated_str
 
     def get_line_pos_of_char_pos(
         self, char_pos: int, source: bool = True
     ) -> Tuple[int, int]:
         """Get the line number and position of a point in the source file.
@@ -461,15 +461,15 @@
 
     This also acts as the base templating class.
     """
 
     name = "raw"
     templater_selector = "templater"
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """Placeholder init function.
 
         Here we should load any initial config found in the root directory. The init
         function shouldn't take any arguments at this stage as we assume that it will
         load its own config. Maybe at this stage we might allow override parameters to
         be passed to the linter at runtime from the cli - that would be the only time we
         would pass arguments in here.
@@ -508,17 +508,17 @@
             config (:obj:`FluffConfig`): A specific config to use for this
                 templating operation. Only necessary for some templaters.
             formatter (:obj:`CallbackFormatter`): Optional object for output.
 
         """
         return TemplatedFile(in_str, fname=fname), []
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """Return true if `other` is of the same class as this one.
 
         NB: This is useful in comparing configs.
         """
         return isinstance(other, self.__class__)
 
-    def config_pairs(self):
+    def config_pairs(self) -> list:
         """Returns info about the given templater for output by the cli."""
         return [("templater", self.name)]
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/jinja.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from jinja2 import (
     Environment,
     FileSystemLoader,
     TemplateError,
     TemplateSyntaxError,
     meta,
 )
-from jinja2.environment import Template
 from jinja2.exceptions import TemplateNotFound, UndefinedError
 from jinja2.ext import Extension
 from jinja2.sandbox import SandboxedEnvironment
 
 from sqlfluff.core.config import FluffConfig
 from sqlfluff.core.errors import SQLBaseError, SQLTemplaterError
 from sqlfluff.core.templaters.base import (
@@ -71,15 +70,17 @@
             # undefined Jinja variable. It's safe to ignore this. Any
             # meaningful issues will surface later at linting time.
             pass
         # Return the context
         return context
 
     @classmethod
-    def _extract_macros_from_path(cls, path: List[str], env: Environment, ctx: Dict):
+    def _extract_macros_from_path(
+        cls, path: List[str], env: Environment, ctx: Dict
+    ) -> dict:
         """Take a path and extract macros from it."""
         macro_ctx = {}
         for path_entry in path:
             # Does it exist? It should as this check was done on config load.
             if not os.path.exists(path_entry):
                 raise ValueError(f"Path does not exist: {path_entry}")
 
@@ -195,15 +196,15 @@
         class ThisEmulator:
             """A class which emulates the `this` class from dbt."""
 
             name = "this_model"
             schema = "this_schema"
             database = "this_database"
 
-            def __str__(self):  # pragma: no cover TODO?
+            def __str__(self) -> str:  # pragma: no cover TODO?
                 return self.name
 
         dbt_builtins = {
             "ref": lambda model_ref: model_ref,
             "source": lambda source_name, table: f"{source_name}_{table}",
             "config": lambda **kwargs: "",
             "var": lambda variable, default="": "item",
@@ -338,34 +339,47 @@
                 self._extract_macros_from_config(
                     config=config, env=env, ctx=live_context
                 )
             )
 
         return live_context
 
-    def template_builder(
+    def construct_render_func(
         self, fname=None, config=None
-    ) -> Tuple[Environment, dict, Callable[[str], Template]]:
+    ) -> Tuple[Environment, dict, Callable[[str], str]]:
         """Builds and returns objects needed to create and run templates."""
         # Load the context
         env = self._get_jinja_env(config)
         live_context = self.get_context(fname=fname, config=config, env=env)
 
-        def make_template(in_str):
+        def render_func(in_str: str) -> str:
             """Used by JinjaTracer to instantiate templates.
 
             This function is a closure capturing internal state from process().
             Note that creating templates involves quite a bit of state known to
             _this_ function but not to JinjaTracer.
 
             https://www.programiz.com/python-programming/closure
             """
-            return env.from_string(in_str, globals=live_context)
+            # Load the template, passing the global context.
+            try:
+                template = env.from_string(in_str, globals=live_context)
+            except TemplateSyntaxError as err:  # pragma: no cover
+                # Something in the template didn't parse, return the original
+                # and a violation around what happened.
+                # NOTE: Most parsing exceptions will be captured when we call
+                # env.parse() in the .process() method. Hence this exception
+                # handling should never be called.
+                raise SQLTemplaterError(
+                    f"Failure to parse jinja template: {err}.",
+                    line_no=err.lineno,
+                )
+            return template.render()
 
-        return env, live_context, make_template
+        return env, live_context, render_func
 
     @large_file_check
     def process(
         self, *, in_str: str, fname: str, config=None, formatter=None
     ) -> Tuple[Optional[TemplatedFile], list]:
         """Process a string and return the new string.
 
@@ -389,98 +403,90 @@
         if not config:  # pragma: no cover
             raise ValueError(
                 "For the jinja templater, the `process()` method requires a config "
                 "object."
             )
 
         try:
-            env, live_context, make_template = self.template_builder(
+            env, live_context, render_func = self.construct_render_func(
                 fname=fname, config=config
             )
         except SQLTemplaterError as err:
             return None, [err]
 
-        # Load the template, passing the global context.
-        try:
-            template = make_template(in_str)
-        except TemplateSyntaxError as err:
-            # Something in the template didn't parse, return the original
-            # and a violation around what happened.
-            return (
-                TemplatedFile(source_str=in_str, fname=fname),
-                [
-                    SQLTemplaterError(
-                        f"Failure to parse jinja template: {err}.",
-                        line_no=err.lineno,
-                    )
-                ],
-            )
-
         violations: List[SQLBaseError] = []
 
-        # Attempt to identify any undeclared variables. The majority
-        # will be found during the _crawl_tree step rather than this
-        # first Exception which serves only to catch catastrophic errors.
+        # Attempt to identify any undeclared variables or syntax errors.
+        # The majority of variables will be found during the _crawl_tree
+        # step rather than this first Exception which serves only to catch
+        # catastrophic errors.
         try:
             syntax_tree = env.parse(in_str)
             potentially_undefined_variables = meta.find_undeclared_variables(
                 syntax_tree
             )
-        except Exception as err:  # pragma: no cover
-            # TODO: Add a url here so people can get more help.
-            raise SQLTemplaterError(f"Failure in identifying Jinja variables: {err}.")
+        except Exception as err:
+            unrendered_out = TemplatedFile(
+                source_str=in_str,
+                fname=fname,
+            )
+            templater_error = SQLTemplaterError(
+                "Failed to parse Jinja syntax. Correct the syntax or select an "
+                "alternative templater."
+            )
+            # Capture a line number if we can.
+            if isinstance(err, TemplateSyntaxError):
+                templater_error.line_no = err.lineno
+            return unrendered_out, [templater_error]
 
         undefined_variables = set()
 
         class UndefinedRecorder:
             """Similar to jinja2.StrictUndefined, but remembers, not fails."""
 
             # Tell Jinja this object is safe to call and does not alter data.
             # https://jinja.palletsprojects.com/en/2.9.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
             unsafe_callable = False
             # https://jinja.palletsprojects.com/en/3.0.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
             alters_data = False
 
             @classmethod
-            def create(cls, name):
+            def create(cls, name: str) -> "UndefinedRecorder":
                 return UndefinedRecorder(name=name)
 
-            def __init__(self, name):
+            def __init__(self, name: str) -> None:
                 self.name = name
 
-            def __str__(self):
+            def __str__(self) -> str:
                 """Treat undefined vars as empty, but remember for later."""
                 undefined_variables.add(self.name)
                 return ""
 
-            def __getattr__(self, item):
+            def __getattr__(self, item) -> "UndefinedRecorder":
                 undefined_variables.add(self.name)
                 return UndefinedRecorder(f"{self.name}.{item}")
 
-            def __call__(self, *args, **kwargs):
+            def __call__(self, *args, **kwargs) -> "UndefinedRecorder":
                 return UndefinedRecorder(f"{self.name}()")
 
         Undefined = (
             UndefinedRecorder
             if "templating" not in config.get("ignore")
             else DummyUndefined
         )
         for val in potentially_undefined_variables:
             if val not in live_context:
                 live_context[val] = Undefined.create(val)  # type: ignore
 
         try:
-            # NB: Passing no context. Everything is loaded when the template is loaded.
-            out_str = template.render(**live_context)
             # Slice the file once rendered.
             raw_sliced, sliced_file, out_str = self.slice_file(
                 in_str,
-                out_str,
+                render_func=render_func,
                 config=config,
-                make_template=make_template,
             )
             if undefined_variables:
                 # Lets go through and find out where they are:
                 for template_err_val in self._crawl_tree(
                     syntax_tree, undefined_variables, in_str
                 ):
                     violations.append(template_err_val)
@@ -509,35 +515,24 @@
                 line_no=1,
                 line_pos=1,
             )
             violations.append(template_err)
             return None, violations
 
     def slice_file(
-        self, raw_str: str, templated_str: str, config=None, **kwargs
+        self, raw_str: str, render_func: Callable[[str], str], config=None, **kwargs
     ) -> Tuple[List[RawFileSlice], List[TemplatedFileSlice], str]:
         """Slice the file to determine regions where we can fix."""
         # The JinjaTracer slicing algorithm is more robust, but it requires
-        # us to create and render a second template (not raw_str) and is only
-        # enabled if the caller passes a make_template() function.
-        make_template = kwargs.pop("make_template", None)
-        if make_template is None:
-            # make_template() was not provided. Use the base class
-            # implementation instead.
-            return super().slice_file(
-                raw_str, templated_str, config, **kwargs
-            )  # pragma: no cover
+        # us to create and render a second template (not raw_str).
 
         templater_logger.info("Slicing File Template")
-        templater_logger.debug("    Raw String: %r", raw_str)
-        templater_logger.debug("    Templated String: %r", templated_str)
-        # TRICKY: Note that the templated_str parameter is not used. JinjaTracer
-        # uses make_template() to build and render the template itself.
+        templater_logger.debug("    Raw String: %r", raw_str[:80])
         analyzer = JinjaAnalyzer(raw_str, self._get_jinja_env())
-        tracer = analyzer.analyze(make_template)
+        tracer = analyzer.analyze(render_func)
         trace = tracer.trace(append_to_templated=kwargs.pop("append_to_templated", ""))
         return trace.raw_sliced, trace.sliced_file, trace.templated_str
 
 
 class DummyUndefined(jinja2.Undefined):
     """Acts as a dummy value to try and avoid template failures.
 
@@ -548,23 +543,23 @@
 
     # Tell Jinja this object is safe to call and does not alter data.
     # https://jinja.palletsprojects.com/en/2.9.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
     unsafe_callable = False
     # https://jinja.palletsprojects.com/en/3.0.x/sandbox/#jinja2.sandbox.SandboxedEnvironment.is_safe_callable
     alters_data = False
 
-    def __init__(self, name):
+    def __init__(self, name) -> None:
         super().__init__()
         self.name = name
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name.replace(".", "_")
 
     @classmethod
-    def create(cls, name):
+    def create(cls, name) -> "DummyUndefined":
         """Factory method.
 
         When ignoring=templating is configured, use 'name' as the value for
         undefined variables. We deliberately avoid recording and reporting
         undefined variables as errors. Using 'name' as the value won't always
         work, but using 'name', combined with implementing the magic methods
         (such as __eq__, see above), works well in most cases.
@@ -577,18 +572,18 @@
 
     def __getattr__(self, item):
         return self.create(f"{self.name}.{item}")
 
     # Implement the most common magic methods. This helps avoid
     # templating errors for undefined variables.
     # https://www.tutorialsteacher.com/python/magic-methods-in-python
-    def _self_impl(self, *args, **kwargs):
+    def _self_impl(self, *args, **kwargs) -> "DummyUndefined":
         return self
 
-    def _bool_impl(self, *args, **kwargs):
+    def _bool_impl(self, *args, **kwargs) -> bool:
         return True
 
     __add__ = _self_impl
     __sub__ = _self_impl
     __mul__ = _self_impl
     __floordiv__ = _self_impl
     __truediv__ = _self_impl
@@ -608,28 +603,28 @@
     __lt__ = _bool_impl
     __le__ = _bool_impl
     __eq__ = _bool_impl
     __ne__ = _bool_impl
     __ge__ = _bool_impl
     __gt__ = _bool_impl
 
-    def __hash__(self):  # pragma: no cov
+    def __hash__(self) -> int:  # pragma: no cov
         # This is called by the "in" operator, among other things.
         return 0
 
     def __iter__(self):
         return [self].__iter__()
 
 
 class DBTTestExtension(Extension):
     """Jinja extension to handle the dbt test tag."""
 
     tags = {"test"}
 
-    def parse(self, parser):
+    def parse(self, parser) -> jinja2.nodes.Macro:
         """Parses out the contents of the test tag."""
         node = jinja2.nodes.Macro(lineno=next(parser.stream).lineno)
         test_name = parser.parse_assign_target(name_only=True).name
 
         parser.parse_signature(node)
         node.name = f"test_{test_name}"
         node.body = parser.parse_statements(("name:endtest",), drop_needle=True)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """Defines the templaters."""
 
 import ast
 from string import Formatter
-from typing import Iterable, Dict, Tuple, List, Iterator, Optional, NamedTuple
+from typing import (
+    Any,
+    Iterable,
+    Dict,
+    Tuple,
+    List,
+    Iterator,
+    Optional,
+    NamedTuple,
+    Callable,
+)
 
 from sqlfluff.core.errors import SQLTemplaterError
 from sqlfluff.core.string_helpers import findall
 from sqlfluff.core.slice_helpers import offset_slice, zero_slice
 
 from sqlfluff.core.templaters.base import (
     RawTemplater,
@@ -121,27 +131,27 @@
         # Trim end:
         new_slice, tail_buffer = new_slice._trim_end(
             templated_str=templated_str, target_end="tail"
         )
         # Return
         return head_buffer, new_slice, tail_buffer
 
-    def try_simple(self):
+    def try_simple(self) -> TemplatedFileSlice:
         """Try to turn this intermediate slice into a simple slice."""
         # Yield anything simple
         if len(self.slice_buffer) == 1:
             return TemplatedFileSlice(
                 self.slice_buffer[0].slice_type,
                 self.source_slice,
                 self.templated_slice,
             )
         else:
             raise ValueError("IntermediateFileSlice is not simple!")
 
-    def coalesce(self):
+    def coalesce(self) -> TemplatedFileSlice:
         """Coalesce this whole slice into a single one. Brutally."""
         return TemplatedFileSlice(
             PythonTemplater._coalesce_types(self.slice_buffer),
             self.source_slice,
             self.templated_slice,
         )
 
@@ -156,20 +166,20 @@
 
     The python templater also defines a lot of the logic for how
     to allow fixing and translation in a templated file.
     """
 
     name = "python"
 
-    def __init__(self, override_context=None, **kwargs):
+    def __init__(self, override_context=None, **kwargs) -> None:
         self.default_context = dict(test_value="__test__")
         self.override_context = override_context or {}
 
     @staticmethod
-    def infer_type(s):
+    def infer_type(s) -> Any:
         """Infer a python type from a string and convert.
 
         Given a string value, convert it to a more specific built-in Python type
         (e.g. int, float, list, dictionary) if possible.
 
         """
         try:
@@ -219,42 +229,54 @@
                 mostly for loading config files at runtime.
             config (:obj:`FluffConfig`): A specific config to use for this
                 templating operation. Only necessary for some templaters.
             formatter (:obj:`CallbackFormatter`): Optional object for output.
 
         """
         live_context = self.get_context(fname=fname, config=config)
-        try:
-            new_str = in_str.format(**live_context)
-        except KeyError as err:
-            # TODO: Add a url here so people can get more help.
-            raise SQLTemplaterError(
-                "Failure in Python templating: {}. Have you configured your "
-                "variables?".format(err)
-            )
+
+        def render_func(raw_str: str) -> str:
+            """Render the string using the captured live_context."""
+            try:
+                rendered_str = raw_str.format(**live_context)
+            except KeyError as err:
+                raise SQLTemplaterError(
+                    "Failure in Python templating: {}. Have you configured your "
+                    "variables? https://docs.sqlfluff.com/en/stable/"
+                    "configuration.html#templating-configuration".format(err)
+                )
+            return rendered_str
+
         raw_sliced, sliced_file, new_str = self.slice_file(
-            in_str, new_str, config=config
+            in_str,
+            render_func=render_func,
+            config=config,
         )
         return (
             TemplatedFile(
                 source_str=in_str,
                 templated_str=new_str,
                 fname=fname,
                 sliced_file=sliced_file,
                 raw_sliced=raw_sliced,
             ),
             [],
         )
 
     def slice_file(
-        self, raw_str: str, templated_str: str, config=None, **kwargs
+        self, raw_str: str, render_func: Callable[[str], str], config=None, **kwargs
     ) -> Tuple[List[RawFileSlice], List[TemplatedFileSlice], str]:
         """Slice the file to determine regions where we can fix."""
         templater_logger.info("Slicing File Template")
         templater_logger.debug("    Raw String: %r", raw_str)
+        # Render the templated string.
+        # NOTE: This seems excessive in this simple example, but for other templating
+        # engines we need more control over the rendering so may need to call this
+        # method more than once.
+        templated_str = render_func(raw_str)
         templater_logger.debug("    Templated String: %r", templated_str)
         # Slice the raw file
         raw_sliced = list(self._slice_template(raw_str))
         templater_logger.debug("    Raw Sliced:")
         for idx, raw_slice in enumerate(raw_sliced):
             templater_logger.debug("        %s: %r", idx, raw_slice)
         # Find the literals
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.2.0/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 This is a newer slicing algorithm that handles cases heuristic.py does not.
 """
 
 from dataclasses import dataclass, field
 import logging
 import regex
-from typing import Callable, cast, Dict, List, NamedTuple, Optional, Tuple
+from typing import Callable, cast, Dict, List, NamedTuple, Optional, Tuple, Union
 
 from jinja2 import Environment
-from jinja2.environment import Template
 from jinja2.exceptions import TemplateSyntaxError
 
 from sqlfluff.core.templaters.base import (
     RawFileSlice,
     TemplatedFileSlice,
 )
 
@@ -48,37 +47,36 @@
 
     def __init__(
         self,
         raw_str: str,
         raw_sliced: List[RawFileSlice],
         raw_slice_info: Dict[RawFileSlice, RawSliceInfo],
         sliced_file: List[TemplatedFileSlice],
-        make_template: Callable[[str], Template],
+        render_func: Callable[[str], str],
     ):
         # Input
         self.raw_str = raw_str
         self.raw_sliced = raw_sliced
         self.raw_slice_info = raw_slice_info
         self.sliced_file = sliced_file
-        self.make_template = make_template
+        self.render_func = render_func
 
         # Internal bookkeeping
         self.program_counter: int = 0
         self.source_idx: int = 0
 
     def trace(self, append_to_templated: str = "") -> JinjaTrace:
         """Executes raw_str. Returns template output and trace."""
         trace_template_str = "".join(
             cast(str, self.raw_slice_info[rs].alternate_code)
             if self.raw_slice_info[rs].alternate_code is not None
             else rs.raw
             for rs in self.raw_sliced
         )
-        trace_template = self.make_template(trace_template_str)
-        trace_template_output = trace_template.render()
+        trace_template_output = self.render_func(trace_template_str)
         # Split output by section. Each section has two possible formats.
         trace_entries: List[regex.Match] = list(
             regex.finditer(r"\0", trace_template_output)
         )
         # If the file has no templated entries, we should just iterate
         # through the raw slices to add all the placeholders.
         if not trace_entries:
@@ -123,18 +121,18 @@
 
         # TRICKY: The 'append_to_templated' parameter is only used by the dbt
         # templater, passing "\n" for this parameter if we need to add one back.
         # (The Jinja templater does not pass this parameter, so
         # 'append_to_templated' gets the default value of "", empty string.)
         # For more detail, see the comments near the call to slice_file() in
         # plugins/sqlfluff-templater-dbt/sqlfluff_templater_dbt/templater.py.
-        templated_str = self.make_template(self.raw_str).render() + append_to_templated
+        templated_str = self.render_func(self.raw_str) + append_to_templated
         return JinjaTrace(templated_str, self.raw_sliced, self.sliced_file)
 
-    def find_slice_index(self, slice_identifier) -> int:
+    def find_slice_index(self, slice_identifier: Union[int, str]) -> int:
         """Given a slice identifier, return its index.
 
         A slice identifier is a string like 00000000000000000000000000000002.
         """
         raw_slices_search_result = [
             idx
             for idx, rs in enumerate(self.raw_sliced)
@@ -142,15 +140,17 @@
         ]
         if len(raw_slices_search_result) != 1:
             raise ValueError(  # pragma: no cover
                 f"Internal error. Unable to locate slice for {slice_identifier}."
             )
         return raw_slices_search_result[0]
 
-    def move_to_slice(self, target_slice_idx, target_slice_length):
+    def move_to_slice(
+        self, target_slice_idx: int, target_slice_length: Union[int, str]
+    ) -> None:
         """Given a template location, walk execution to that point."""
         while self.program_counter < len(self.raw_sliced):
             self.record_trace(
                 target_slice_length if self.program_counter == target_slice_idx else 0
             )
             current_raw_slice = self.raw_sliced[self.program_counter]
             if self.program_counter == target_slice_idx:
@@ -170,15 +170,17 @@
                     # target.
                     if next_slice_idx <= target_slice_idx:
                         candidates.append(next_slice_idx)
                 # Choose the candidate that takes us closest to the target.
                 candidates.sort(key=lambda c: abs(target_slice_idx - c))
                 self.program_counter = candidates[0]
 
-    def record_trace(self, target_slice_length, slice_idx=None, slice_type=None):
+    def record_trace(
+        self, target_slice_length, slice_idx=None, slice_type=None
+    ) -> None:
         """Add the specified (default: current) location to the trace."""
         if slice_idx is None:
             slice_idx = self.program_counter
         if slice_type is None:
             slice_type = self.raw_sliced[slice_idx].slice_type
         self.sliced_file.append(
             TemplatedFileSlice(
@@ -198,15 +200,15 @@
 
 class JinjaAnalyzer:
     """Analyzes a Jinja template to prepare for tracing."""
 
     re_open_tag = regex.compile(r"^\s*({[{%])[\+\-]?\s*")
     re_close_tag = regex.compile(r"\s*[\+\-]?([}%]})\s*$")
 
-    def __init__(self, raw_str: str, env: Environment):
+    def __init__(self, raw_str: str, env: Environment) -> None:
         # Input
         self.raw_str: str = raw_str
         self.env = env
 
         # Output
         self.raw_sliced: List[RawFileSlice] = []
         self.raw_slice_info: Dict[RawFileSlice, RawSliceInfo] = {}
@@ -333,15 +335,15 @@
         # raw_end and raw_begin are whole tags rather
         # than blocks and comments where we get partial
         # tags.
         "raw_end": "block",
         "raw_begin": "block",
     }
 
-    def analyze(self, make_template: Callable[[str], Template]) -> JinjaTracer:
+    def analyze(self, render_func: Callable[[str], str]) -> JinjaTracer:
         """Slice template in jinja."""
         # str_buff and str_parts are two ways we keep track of tokens received
         # from Jinja. str_buff concatenates them together, while str_parts
         # accumulates the individual strings. We generally prefer using
         # str_parts. That's because Jinja doesn't just split on whitespace, so
         # by keeping tokens as Jinja returns them, the code is more robust.
         # Consider the following:
@@ -469,15 +471,15 @@
                 str_buff = ""
                 str_parts = []
         return JinjaTracer(
             self.raw_str,
             self.raw_sliced,
             self.raw_slice_info,
             self.sliced_file,
-            make_template,
+            render_func,
         )
 
     def track_templated(
         self, m_open: regex.Match, m_close: regex.Match, tag_contents: List[str]
     ) -> RawSliceInfo:
         """Compute tracking info for Jinja templated region, e.g. {{ foo }}."""
         unique_alternate_id = self.next_slice_id()
@@ -489,15 +491,15 @@
         alternate_code = (
             f"\0{unique_alternate_id} {open_} " f"{''.join(tag_contents)} {close_}"
         )
         return self.make_raw_slice_info(unique_alternate_id, alternate_code)
 
     def track_call(
         self, m_open: regex.Match, m_close: regex.Match, tag_contents: List[str]
-    ):
+    ) -> RawSliceInfo:
         """Set up tracking for "{% call ... %}"."""
         unique_alternate_id = self.next_slice_id()
         open_ = m_open.group(1)
         close_ = m_close.group(1)
         # Here, we still need to evaluate the original tag contents, e.g. in
         # case it has intentional side effects, but also return a slice ID
         # for tracking.
@@ -520,15 +522,17 @@
         # Replace literal text with a unique ID.
         self.raw_slice_info[self.raw_sliced[-1]] = self.slice_info_for_literal(
             len(raw), ""
         )
         self.idx_raw += len(raw)
 
     @staticmethod
-    def extract_block_type(tag_name, block_subtype):
+    def extract_block_type(
+        tag_name: str, block_subtype: Optional[str] = None
+    ) -> Tuple[str, Optional[str]]:
         """Determine block type."""
         # :TRICKY: Syntactically, the Jinja {% include %} directive looks like
         # a block, but its behavior is basically syntactic sugar for
         # {{ open("somefile).read() }}. Thus, treat it as templated code.
         # It's a similar situation with {% import %} and {% from ... import %}.
         if tag_name in ["include", "import", "from", "do"]:
             block_type = "templated"
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/core/timing.py` & `sqlfluff-2.2.0/src/sqlfluff/core/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class TimingSummary:
     """An object for tracking the timing of similar steps across many files."""
 
     def __init__(self, steps: Optional[List[str]] = None):
         self.steps = steps
         self._timings: List[Dict[str, float]] = []
 
-    def add(self, timing_dict: Dict[str, float]):
+    def add(self, timing_dict: Dict[str, float]) -> None:
         """Add a timing dictionary to the summary."""
         self._timings.append(timing_dict)
         if not self.steps:
             self.steps = list(timing_dict.keys())
 
     def summary(self) -> Dict[str, Dict[str, float]]:
         """Generate a summary for display."""
@@ -42,20 +42,22 @@
 
 class RuleTimingSummary:
     """An object for tracking the timing of rules across many files."""
 
     def __init__(self) -> None:
         self._timings: List[Tuple[str, str, float]] = []
 
-    def add(self, rule_timings: List[Tuple[str, str, float]]):
+    def add(self, rule_timings: List[Tuple[str, str, float]]) -> None:
         """Add a set of rule timings."""
         # Add records to the main list.
         self._timings.extend(rule_timings)
 
-    def summary(self, threshold=0.5) -> Dict[str, Dict[str, Union[float, str]]]:
+    def summary(
+        self, threshold: float = 0.5
+    ) -> Dict[str, Dict[str, Union[float, str]]]:
         """Generate a summary for display."""
         keys: Set[Tuple[str, str]] = set()
         vals: Dict[Tuple[str, str], List[float]] = defaultdict(list)
 
         for code, name, time in self._timings:
             vals[(code, name)].append(time)
             keys.add((code, name))
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,19 +999,19 @@
         Each reference is an ObjectReferencePart. If some are split, then a
         segment may appear twice, but the substring will only appear once.
         """
         # Extract the references from those identifiers (because some may be quoted)
         for elem in self.recursive_crawl("identifier"):
             yield from self._iter_reference_parts(elem)
 
-    def is_qualified(self):
+    def is_qualified(self) -> bool:
         """Return if there is more than one element to the reference."""
         return len(list(self.iter_raw_references())) > 1
 
-    def qualification(self):
+    def qualification(self) -> str:
         """Return the qualification type of this reference."""
         return "qualified" if self.is_qualified() else "unqualified"
 
     class ObjectReferenceLevel(Enum):
         """Labels for the "levels" of a reference.
 
         Note: Since SQLFluff does not have access to database catalog
@@ -1246,14 +1246,24 @@
     type = "numeric_literal"
     match_grammar: Matchable = Sequence(
         Ref("SignedSegmentGrammar"),
         Ref("NumericLiteralSegment"),
     )
 
 
+class AggregateOrderByClause(BaseSegment):
+    """An order by clause for an aggregate fucntion.
+
+    Defined as a class to allow a specific type for rule AM06
+    """
+
+    type = "aggregate_order_by"
+    match_grammar: Matchable = Ref("OrderByClauseSegment")
+
+
 ansi_dialect.add(
     # FunctionContentsExpressionGrammar intended as a hook to override
     # in other dialects.
     FunctionContentsExpressionGrammar=Ref("ExpressionSegment"),
     FunctionContentsGrammar=AnyNumberOf(
         Ref("ExpressionSegment"),
         # A Cast-like function
@@ -1279,15 +1289,15 @@
                 # but for COUNT(*) or similar we allow the star segment
                 # here.
                 Ref("StarSegment"),
                 Delimited(Ref("FunctionContentsExpressionGrammar")),
             ),
         ),
         Ref(
-            "OrderByClauseSegment"
+            "AggregateOrderByClause"
         ),  # used by string_agg (postgres), group_concat (exasol),listagg (snowflake)..
         Sequence(Ref.keyword("SEPARATOR"), Ref("LiteralGrammar")),
         # like a function call: POSITION ( 'QL' IN 'SQL')
         Sequence(
             OneOf(
                 Ref("QuotedLiteralSegment"),
                 Ref("SingleIdentifierGrammar"),
@@ -3441,16 +3451,22 @@
                     "FUTURE",
                     _schema_object_types_plural,
                     "IN",
                     OneOf("DATABASE", "SCHEMA"),
                 ),
                 optional=True,
             ),
-            Delimited(Ref("ObjectReferenceSegment"), terminator=OneOf("TO", "FROM")),
-            Ref("FunctionParameterListGrammar", optional=True),
+            Delimited(
+                Ref("ObjectReferenceSegment"),
+                Sequence(
+                    Ref("FunctionNameSegment"),
+                    Ref("FunctionParameterListGrammar", optional=True),
+                ),
+                terminator=OneOf("TO", "FROM"),
+            ),
         ),
         Sequence("LARGE", "OBJECT", Ref("NumericLiteralSegment")),
     )
 
     match_grammar: Matchable = OneOf(
         # Based on https://www.postgresql.org/docs/13/sql-grant.html
         # and https://docs.snowflake.com/en/sql-reference/sql/grant-privilege.html
@@ -3906,15 +3922,15 @@
         Ref("CreateSequenceStatementSegment"),
         Ref("AlterSequenceStatementSegment"),
         Ref("DropSequenceStatementSegment"),
         Ref("CreateTriggerStatementSegment"),
         Ref("DropTriggerStatementSegment"),
     )
 
-    def get_table_references(self):
+    def get_table_references(self) -> set:
         """Use parsed tree to extract table references."""
         table_refs = {
             tbl_ref.raw for tbl_ref in self.recursive_crawl("table_reference")
         }
         cte_refs = {
             cte_def.get_identifier().raw
             for cte_def in self.recursive_crawl("common_table_expression")
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,26 @@
 clickhouse_dialect.sets("unreserved_keywords").update(UNRESERVED_KEYWORDS)
 clickhouse_dialect.replace(
     SingleIdentifierGrammar=OneOf(
         Ref("NakedIdentifierSegment"),
         Ref("QuotedIdentifierSegment"),
         Ref("SingleQuotedIdentifierSegment"),
     ),
+    QuotedLiteralSegment=OneOf(
+        TypedParser(
+            "single_quote",
+            ansi.LiteralSegment,
+            type="quoted_literal",
+        ),
+        TypedParser(
+            "dollar_quote",
+            ansi.LiteralSegment,
+            type="quoted_literal",
+        ),
+    ),
 )
 
 clickhouse_dialect.insert_lexer_matchers(
     # https://clickhouse.com/docs/en/sql-reference/functions#higher-order-functions---operator-and-lambdaparams-expr-function
     [StringLexer("lambda", r"->", SymbolSegment, segment_kwargs={"type": "lambda"})],
     before="newline",
 )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 NOT
 NULL
 NULLIF
 OF
 ON
 OR
 ORDER
+RETURNING
 ROW
 ROWS
 SELECT
 SET
 SINK
 SINKS
 TO
@@ -270,15 +271,14 @@
 REPLACE
 REPLICA
 REPLICAS
 REPLICATION
 RESET
 RESTRICT
 RETENTION
-RETURNING
 RIGHT
 ROLE
 ROLES
 ROLLBACK
 ROTATE
 S3
 SASL
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1200,14 +1200,15 @@
 
 class AlterTableStatementSegment(BaseSegment):
     """An `ALTER TABLE .. ALTER COLUMN` statement.
 
     Overriding ANSI to add `CHANGE COLUMN` and `DROP COLUMN` support.
 
     https://dev.mysql.com/doc/refman/8.0/en/alter-table.html
+    https://mariadb.com/kb/en/alter-table/
 
     """
 
     type = "alter_table_statement"
     match_grammar = Sequence(
         "ALTER",
         "TABLE",
@@ -1218,15 +1219,29 @@
                 Sequence(
                     Ref("ParameterNameSegment"),
                     Ref("EqualsSegment", optional=True),
                     OneOf(Ref("LiteralGrammar"), Ref("NakedIdentifierSegment")),
                 ),
                 # Add column
                 Sequence(
-                    OneOf("ADD", "MODIFY"),
+                    "ADD",
+                    Ref.keyword("COLUMN", optional=True),
+                    Ref("IfNotExistsGrammar", optional=True),
+                    Ref("ColumnDefinitionSegment"),
+                    OneOf(
+                        Sequence(
+                            OneOf("FIRST", "AFTER"), Ref("ColumnReferenceSegment")
+                        ),
+                        # Bracketed Version of the same
+                        Ref("BracketedColumnReferenceListGrammar"),
+                        optional=True,
+                    ),
+                ),
+                Sequence(
+                    "MODIFY",
                     Ref.keyword("COLUMN", optional=True),
                     Ref("ColumnDefinitionSegment"),
                     OneOf(
                         Sequence(
                             OneOf("FIRST", "AFTER"), Ref("ColumnReferenceSegment")
                         ),
                         # Bracketed Version of the same
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 https://www.postgresql.org/docs/13/sql-keywords-appendix.html
 Here, "not-keyword" refers to a word not being a keyword, and will be removed from any
 default keyword definition, these keywords are, or have been, an ANSI keyword.
 
 There are also some keywords that are(n't) supported as types and function, but there
 isn't support for that distinction at present.
 """
+from typing import List, Tuple
 
 
-def priority_keyword_merge(*args):
+def priority_keyword_merge(*args: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
     """Merge keyword lists, giving priority to entries in later lists.
 
     *args is a list of keyword lists, these lists should be of tuples in the form
     (keyword, type)
 
     """
     keyword_lists = [*args]
@@ -34,15 +35,15 @@
             base_list.append(item)
 
         keyword_lists.pop(1)
 
     return base_list
 
 
-def get_keywords(keyword_list, keyword_type):
+def get_keywords(keyword_list: List[Tuple[str, str]], keyword_type: str) -> List[str]:
     """Get a list of keywords of the required type.
 
     keyword_type should be one of "not-keyword", "reserved", "non-reserved"
     """
     keywords = [x[0] for x in keyword_list if x[1].startswith(keyword_type)]
 
     return keywords
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from sqlfluff.core.parser import (
     AnyNumberOf,
     AnySetOf,
     Anything,
     BaseSegment,
     Bracketed,
     CodeSegment,
+    Dedent,
     Delimited,
+    Indent,
     Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     Ref,
     RegexLexer,
     RegexParser,
     SegmentGenerator,
     Sequence,
+    StartsWith,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects import dialect_postgres as postgres
 from sqlfluff.dialects.dialect_redshift_keywords import (
     redshift_reserved_keywords,
     redshift_unreserved_keywords,
 )
@@ -1831,14 +1834,45 @@
             "LIKE",
             Ref("QuotedLiteralSegment"),
             optional=True,
         ),
     )
 
 
+class GrantUsageDatashareStatementSegment(BaseSegment):
+    """A `GRANT DATASHARES` statement.
+
+    https://docs.aws.amazon.com/redshift/latest/dg/r_GRANT.html
+    section "Granting datashare permissions"
+    Note: According to docummentation, multiple accounts and namespaces can be
+          specified. However, tests using redshift instance showed this causes a syntax
+          error.
+    """
+
+    type = "grant_datashare_statement"
+    match_grammar = Sequence(
+        OneOf("GRANT", "REVOKE"),
+        "USAGE",
+        "ON",
+        "DATASHARE",
+        Ref("ObjectReferenceSegment"),
+        OneOf("TO", "FROM"),
+        OneOf(
+            Sequence("NAMESPACE", Ref("QuotedLiteralSegment")),
+            Sequence(
+                "ACCOUNT",
+                Sequence(
+                    Ref("QuotedLiteralSegment"),
+                    Sequence("VIA", "DATA", "CATALOG", optional=True),
+                ),
+            ),
+        ),
+    )
+
+
 class CreateRlsPolicyStatementSegment(BaseSegment):
     """A `CREATE RLS POLICY` statement.
 
     https://docs.aws.amazon.com/redshift/latest/dg/r_CREATE_RLS_POLICY.html
     """
 
     type = "create_rls_policy_statement"
@@ -2015,14 +2049,15 @@
             Ref("AnalyzeCompressionStatementSegment"),
             Ref("AlterProcedureStatementSegment"),
             Ref("CallStatementSegment"),
             Ref("CreateRlsPolicyStatementSegment"),
             Ref("ManageRlsPolicyStatementSegment"),
             Ref("DropRlsPolicyStatementSegment"),
             Ref("CreateExternalFunctionStatementSegment"),
+            Ref("GrantUsageDatashareStatementSegment"),
         ],
     )
 
 
 class PartitionedBySegment(BaseSegment):
     """Partitioned By Segment.
 
@@ -2565,7 +2600,60 @@
         OneOf("DEFAULT", Ref("QuotedLiteralSegment")),
         Sequence(
             "RETRY_TIMEOUT",
             Ref("NumericLiteralSegment"),
             optional=True,
         ),
     )
+
+
+class QualifyClauseSegment(BaseSegment):
+    """A `QUALIFY` clause like in `SELECT`.
+
+    https://docs.aws.amazon.com/redshift/latest/dg/r_QUALIFY_clause.html
+    """
+
+    type = "qualify_clause"
+    match_grammar = Sequence(
+        "QUALIFY",
+        Indent,
+        Ref("ExpressionSegment"),
+        Dedent,
+    )
+
+
+class SelectStatementSegment(ansi.SelectStatementSegment):
+    """A snowflake `SELECT` statement including optional Qualify.
+
+    https://docs.aws.amazon.com/redshift/latest/dg/r_QUALIFY_clause.html
+    """
+
+    type = "select_statement"
+    match_grammar = StartsWith(
+        # NB: In bigquery, the select clause may include an EXCEPT, which
+        # will also match the set operator, but by starting with the whole
+        # select clause rather than just the SELECT keyword, we normally
+        # mitigate that here. But this isn't BigQuery! So we can be more
+        # efficient and just use the keyword.
+        "SELECT",
+        terminator=Ref("SetOperatorSegment"),
+    )
+
+    parse_grammar = ansi.SelectStatementSegment.parse_grammar.copy(
+        insert=[Ref("QualifyClauseSegment", optional=True)],
+        before=Ref("OrderByClauseSegment", optional=True),
+    )
+
+
+class UnorderedSelectStatementSegment(ansi.UnorderedSelectStatementSegment):
+    """A snowflake unordered `SELECT` statement including optional Qualify.
+
+    https://docs.aws.amazon.com/redshift/latest/dg/r_QUALIFY_clause.html
+    """
+
+    type = "select_statement"
+    match_grammar = ansi.UnorderedSelectStatementSegment.match_grammar.copy()
+
+    parse_grammar = ansi.UnorderedSelectStatementSegment.parse_grammar.copy(
+        insert=[Ref("QualifyClauseSegment", optional=True)],
+        before=Ref("OverlapsClauseSegment", optional=True),
+    )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1034,14 +1034,15 @@
 VARBINARY
 VARBYTE
 VARCHAR
 VARIADIC
 VARYING
 VERSION
 VERSIONING
+VIA
 VIEW
 VIEWS
 VOLATILE
 WALLET
 WAREHOUSE
 WEEK
 WEEKDAY
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -2363,16 +2363,22 @@
                         Sequence("FILE", "FORMATS"),
                     ),
                     "IN",
                     OneOf("DATABASE", "SCHEMA"),
                 ),
                 optional=True,
             ),
-            Delimited(Ref("ObjectReferenceSegment"), terminator=OneOf("TO", "FROM")),
-            Ref("FunctionParameterListGrammar", optional=True),
+            Delimited(
+                Ref("ObjectReferenceSegment"),
+                Sequence(
+                    Ref("FunctionNameSegment"),
+                    Ref("FunctionParameterListGrammar", optional=True),
+                ),
+                terminator=OneOf("TO", "FROM"),
+            ),
         ),
     )
 
     match_grammar: Matchable = OneOf(
         # https://docs.snowflake.com/en/sql-reference/sql/grant-privilege.html
         Sequence(
             "GRANT",
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     StartsWith,
     RegexParser,
     Matchable,
     MultiStringParser,
     StringLexer,
     AnySetOf,
 )
+from sqlfluff.core.parser.segments import BracketedSegment
 from sqlfluff.core.parser.segments.raw import CodeSegment, KeywordSegment
 from sqlfluff.dialects.dialect_sparksql_keywords import (
     RESERVED_KEYWORDS,
     UNRESERVED_KEYWORDS,
 )
 
 from sqlfluff.dialects import dialect_ansi as ansi
@@ -392,15 +393,15 @@
         Ref("CommaSegment"),
         Ref("CastOperatorSegment"),
         Ref("StartSquareBracketSegment"),
         Ref("StartBracketSegment"),
         Ref("BinaryOperatorGrammar"),
         Ref("DelimiterGrammar"),
         Ref("JoinLikeClauseGrammar"),
-        ansi.BracketedSegment,
+        BracketedSegment,
     ),
     FunctionContentsExpressionGrammar=OneOf(
         Ref("ExpressionSegment"),
         Ref("StarSegment"),
     ),
 )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.2.0/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.2.0/src/sqlfluff/diff_quality_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,48 +10,49 @@
 from diff_cover.command_runner import execute, run_command_for_code
 from diff_cover.hook import hookimpl as diff_cover_hookimpl
 from diff_cover.violationsreporters.base import (
     QualityDriver,
     QualityReporter,
     Violation,
 )
+from typing import List
 
 
 logger = logging.getLogger(__name__)
 
 
 class SQLFluffDriver(QualityDriver):
     """SQLFluff driver for use by SQLFluffViolationReporter."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             [sys.executable, "-m", "sqlfluff.cli.commands"],
             [".sql"],
             [
                 s.encode(sys.getfilesystemencoding())
                 for s in ["sqlfluff", "lint", "--format=json"]
             ],
             exit_codes=[0, 1],
         )
 
-    def parse_reports(self, reports):  # pragma: no cover
+    def parse_reports(self, reports) -> None:  # pragma: no cover
         """Parse report output. Not used by SQLFluff."""
         pass
 
-    def installed(self):
+    def installed(self) -> bool:
         """Check if SQLFluff is installed."""
         return run_command_for_code("sqlfluff") == 0
 
 
 class SQLFluffViolationReporter(QualityReporter):
     """Class that implements diff-quality integration."""
 
     supported_extensions = ["sql"]
 
-    def __init__(self, **kw):
+    def __init__(self, **kw) -> None:
         """Calls the base class constructor to set the object's name."""
         super().__init__(SQLFluffDriver(), **kw)
 
     def violations_batch(self, src_paths):
         """Return a dictionary of Violations recorded in `src_paths`."""
         # Check if SQLFluff is installed.
         if self.driver_tool_installed is None:
@@ -74,15 +75,15 @@
                             Violation(v["line_no"], v["description"])
                             for v in file["violations"]
                         ]
         else:
             logger.warning("Not running SQLFluff: No files to check")
         return self.violations_dict
 
-    def _run_sqlfluff(self, src_paths):
+    def _run_sqlfluff(self, src_paths) -> List[str]:
         # Prepare the SQLFluff command to run.
         command = copy.deepcopy(self.driver.command)
         if self.options:
             for arg in self.options.split():
                 command.append(arg)
         for src_path in src_paths:
             if src_path.endswith(".sql") and os.path.exists(src_path):
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Implementation of Rule AL01."""
-from typing import Optional, Tuple
+from typing import cast, Optional, Tuple
 
 from sqlfluff.core.parser import (
     KeywordSegment,
+    BaseSegment,
+    RawSegment,
 )
 
 from sqlfluff.core.rules import BaseRule, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.utils.reflow import ReflowSequence
 
 
@@ -58,14 +60,15 @@
         """
         # Config type hints
         self.aliasing: str
 
         assert context.segment.is_type("alias_expression")
         if context.parent_stack[-1].is_type(*self._target_parent_types):
             # Search for an AS keyword.
+            as_keyword: Optional[BaseSegment]
             for as_keyword in context.segment.segments:
                 if as_keyword.raw_upper == "AS":
                     break
             else:
                 as_keyword = None
 
             if as_keyword:
@@ -75,15 +78,15 @@
                         anchor=as_keyword,
                         # Generate the fixes to remove and respace accordingly.
                         fixes=ReflowSequence.from_around_target(
                             as_keyword,
                             context.parent_stack[0],
                             config=context.config,
                         )
-                        .without(as_keyword)
+                        .without(cast(RawSegment, as_keyword))
                         .respace()
                         .get_fixes(),
                     )
 
             elif self.aliasing != "implicit":
                 self.logger.debug("Inserting AS keyword and respacing.")
                 for identifier in context.segment.raw_segments:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implementation of Rule AL04."""
 
 import itertools
 from typing import List, Optional, Tuple
-
+from sqlfluff.dialects.dialect_ansi import ObjectReferenceSegment
 from sqlfluff.core.dialects.common import AliasInfo, ColumnAliasInfo
 from sqlfluff.core.parser import BaseSegment
 from sqlfluff.core.rules import BaseRule, LintResult, RuleContext, EvalResultType
 from sqlfluff.utils.analysis.select import get_select_statement_info
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 
 
@@ -64,15 +64,15 @@
     groups: Tuple[str, ...] = ("all", "core", "aliasing", "aliasing.unique")
     crawl_behaviour = SegmentSeekerCrawler({"select_statement"})
 
     def _lint_references_and_aliases(
         self,
         table_aliases: List[AliasInfo],
         standalone_aliases: List[str],
-        references: List[BaseSegment],
+        references: List[ObjectReferenceSegment],
         col_aliases: List[ColumnAliasInfo],
         using_cols: List[str],
         parent_select: Optional[BaseSegment],
     ) -> Optional[List[LintResult]]:
         """Check whether any aliases are duplicates.
 
         NB: Subclasses of this error should override this function.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                     # not required.
                     return False
 
         # This should never happen. Return False just to be safe.
         return False  # pragma: no cover
 
     @classmethod
-    def _analyze_table_aliases(cls, query: AL05Query, dialect: Dialect):
+    def _analyze_table_aliases(cls, query: AL05Query, dialect: Dialect) -> None:
         # Get table aliases defined in query.
         for selectable in query.selectables:
             select_info = selectable.select_info
             if select_info:
                 # Record the aliases.
                 query.aliases += select_info.table_aliases
 
@@ -182,15 +182,15 @@
                         cls._resolve_and_mark_reference(query, tr.part)
 
         # Visit children.
         for child in query.children:
             cls._analyze_table_aliases(cast(AL05Query, child), dialect)
 
     @classmethod
-    def _resolve_and_mark_reference(cls, query: AL05Query, ref: str):
+    def _resolve_and_mark_reference(cls, query: AL05Query, ref: str) -> None:
         # Does this query define the referenced alias?
         if any(ref == a.ref_str for a in query.aliases):
             # Yes. Record the reference.
             query.tbl_refs.add(ref)
         elif query.parent:
             # No. Recursively check the query's parent hierarchy.
             cls._resolve_and_mark_reference(cast(AL05Query, query.parent), ref)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Implementation of Rule AL06."""
 
-from typing import Optional
+from typing import List, Optional
 
 from sqlfluff.core.rules import BaseRule, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.utils.functional import FunctionalContext
 
 
 class Rule_AL06(BaseRule):
@@ -45,30 +45,30 @@
 
     name = "aliasing.length"
     aliases = ("L066",)
     groups = ("all", "core", "aliasing")
     config_keywords = ["min_alias_length", "max_alias_length"]
     crawl_behaviour = SegmentSeekerCrawler({"select_statement"})
 
-    def _eval(self, context: RuleContext) -> Optional[LintResult]:
+    def _eval(self, context: RuleContext) -> Optional[List[LintResult]]:
         """Identify aliases in from clause and join conditions.
 
         Find base table, table expressions in join, and other expressions in select
         clause and decide if it's needed to report them.
         """
         self.min_alias_length: Optional[int]
         self.max_alias_length: Optional[int]
 
         assert context.segment.is_type("select_statement")
         children = FunctionalContext(context).segment.children()
         from_expression_elements = children.recursive_crawl("from_expression_element")
 
         return self._lint_aliases(from_expression_elements) or None
 
-    def _lint_aliases(self, from_expression_elements):
+    def _lint_aliases(self, from_expression_elements) -> Optional[List[LintResult]]:
         """Lint all table aliases."""
         # A buffer to keep any violations.
         violation_buff = []
 
         # For each table, check whether it is aliased, and if so check the
         # lengths.
         for from_expression_element in from_expression_elements:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Implementation of Rule AL07."""
 
 from collections import Counter, defaultdict
-from typing import Generator, NamedTuple, Optional
+from typing import Generator, NamedTuple, Optional, List
 
 from sqlfluff.core.parser import BaseSegment
 from sqlfluff.core.rules import BaseRule, LintFix, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 
 from sqlfluff.utils.functional import sp, FunctionalContext
 
@@ -85,15 +85,15 @@
     name = "aliasing.forbid"
     aliases = ("L031",)
     groups = ("all", "aliasing")
     config_keywords = ["force_enable"]
     crawl_behaviour = SegmentSeekerCrawler({"select_statement"})
     is_fix_compatible = True
 
-    def _eval(self, context: RuleContext) -> Optional[LintResult]:
+    def _eval(self, context: RuleContext) -> Optional[List[LintResult]]:
         """Identify aliases in from clause and join conditions.
 
         Find base table, table expressions in join, and other expressions in select
         clause and decide if it's needed to report them.
         """
         # Config type hints
         self.force_enable: bool
@@ -104,15 +104,15 @@
         # about whether backticks are required (and whether the query is valid
         # or not, even with them), depending on whether the GCP project name is
         # present, or just the dataset name. Since SQLFluff doesn't have access
         # to BigQuery when it is looking at the query, it would be complex for
         # this rule to do the right thing. For now, the rule simply disables
         # itself.
         if not self.force_enable:
-            return LintResult()
+            return None
 
         assert context.segment.is_type("select_statement")
 
         children = FunctionalContext(context).segment.children()
         from_clause_segment = children.select(sp.is_type("from_clause")).first()
         base_table = (
             from_clause_segment.children(sp.is_type("from_expression"))
@@ -184,15 +184,15 @@
             alias_identifier_ref = alias_exp_ref.get_child("identifier")
             yield TableAliasInfo(
                 table_ref, whitespace_ref, alias_exp_ref, alias_identifier_ref
             )
 
     def _lint_aliases_in_join(
         self, base_table, from_expression_elements, column_reference_segments, segment
-    ):
+    ) -> Optional[List[LintResult]]:
         """Lint and fix all aliases in joins - except for self-joins."""
         # A buffer to keep any violations.
         violation_buff = []
 
         to_check = list(
             self._filter_table_expressions(base_table, from_expression_elements)
         )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """The aliasing plugin bundle."""
 
 from sqlfluff.core.plugin import hookimpl
-
-from sqlfluff.rules.aliasing.AL01 import Rule_AL01
-from sqlfluff.rules.aliasing.AL02 import Rule_AL02
-from sqlfluff.rules.aliasing.AL03 import Rule_AL03
-from sqlfluff.rules.aliasing.AL04 import Rule_AL04
-from sqlfluff.rules.aliasing.AL05 import Rule_AL05
-from sqlfluff.rules.aliasing.AL06 import Rule_AL06
-from sqlfluff.rules.aliasing.AL07 import Rule_AL07
+from sqlfluff.core.rules import BaseRule
+from typing import List, Type
 
 
 @hookimpl
-def get_rules():
-    """Get plugin rules."""
+def get_rules() -> List[Type[BaseRule]]:
+    """Get plugin rules.
+
+    NOTE: Rules are imported only on fetch to manage import times
+    when rules aren't used.
+    """
+    from sqlfluff.rules.aliasing.AL01 import Rule_AL01
+    from sqlfluff.rules.aliasing.AL02 import Rule_AL02
+    from sqlfluff.rules.aliasing.AL03 import Rule_AL03
+    from sqlfluff.rules.aliasing.AL04 import Rule_AL04
+    from sqlfluff.rules.aliasing.AL05 import Rule_AL05
+    from sqlfluff.rules.aliasing.AL06 import Rule_AL06
+    from sqlfluff.rules.aliasing.AL07 import Rule_AL07
+
     return [Rule_AL01, Rule_AL02, Rule_AL03, Rule_AL04, Rule_AL05, Rule_AL06, Rule_AL07]
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     """
 
     name = "ambiguous.column_count"
     aliases = ("L044",)
     groups: Tuple[str, ...] = ("all", "ambiguous")
     crawl_behaviour = SegmentSeekerCrawler(set(_START_TYPES))
 
-    def _handle_alias(self, selectable, alias_info, query):
+    def _handle_alias(self, selectable, alias_info, query) -> None:
         select_info_target = SelectCrawler.get(
             query, alias_info.from_expression_element
         )[0]
         if isinstance(select_info_target, str):
             # It's an alias to an external table whose
             # number of columns could vary without our
             # knowledge. Thus, warn.
@@ -83,21 +83,21 @@
                 f"Query target {select_info_target} is external. Generating warning."
             )
             raise RuleFailure(selectable.selectable)
         else:
             # Handle nested SELECT.
             self._analyze_result_columns(select_info_target)
 
-    def _analyze_result_columns(self, query: Query):
+    def _analyze_result_columns(self, query: Query) -> None:
         """Given info on a list of SELECTs, determine whether to warn."""
         # Recursively walk from the given query (select_info_list) to any
         # wildcard columns in the select targets. If every wildcard evdentually
         # resolves to a query without wildcards, all is well. Otherwise, warn.
         if not query.selectables:
-            return  # pragma: no cover
+            return None  # pragma: no cover
         for selectable in query.selectables:
             self.logger.debug(f"Analyzing query: {selectable.selectable.raw}")
             for wildcard in selectable.get_wildcard_info():
                 if wildcard.tables:
                     for wildcard_table in wildcard.tables:
                         self.logger.debug(
                             f"Wildcard: {wildcard.segment.raw} has target "
@@ -128,26 +128,26 @@
                     # querying from a nested select in FROM.
                     query_list = SelectCrawler.get(
                         query, query.selectables[0].selectable
                     )
                     for o in query_list:
                         if isinstance(o, Query):
                             self._analyze_result_columns(o)
-                            return
+                            return None
                     self.logger.debug(
                         f'Query target "{query.selectables[0].selectable.raw}" has no '
                         "targets. Generating warning."
                     )
                     raise RuleFailure(query.selectables[0].selectable)
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Outermost query should produce known number of columns."""
         if not FunctionalContext(context).parent_stack.any(sp.is_type(*_START_TYPES)):
             crawler = SelectCrawler(context.segment, context.dialect)
 
             # Begin analysis at the outer query.
             if crawler.query_tree:
                 try:
-                    return self._analyze_result_columns(crawler.query_tree)
+                    self._analyze_result_columns(crawler.query_tree)
                 except RuleFailure as e:
                     return LintResult(anchor=e.anchor)
         return None
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,19 @@
     name = "ambiguous.column_references"
     aliases = ("L054",)
     groups: Tuple[str, ...] = ("all", "core", "ambiguous")
     config_keywords = ["group_by_and_order_by_style"]
     crawl_behaviour = SegmentSeekerCrawler(
         {"groupby_clause", "orderby_clause", "grouping_expression_list"}
     )
-    _ignore_types: List[str] = ["withingroup_clause", "window_specification"]
+    _ignore_types: List[str] = [
+        "withingroup_clause",
+        "window_specification",
+        "aggregate_order_by",
+    ]
 
     def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """Inconsistent column references in GROUP BY/ORDER BY clauses."""
         # Config type hints
         self.group_by_and_order_by_style: str
 
         # We only care about GROUP BY/ORDER BY clauses.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     name = "ambiguous.set_columns"
     aliases = ("L068",)
     groups: Tuple[str, ...] = ("all", "ambiguous")
     crawl_behaviour = SegmentSeekerCrawler({"set_expression"}, provide_raw_stack=True)
 
     def __handle_alias_case(
         self, parent_query, alias_info, query, context, resolve_targets, wildcard
-    ):
+    ) -> None:
         select_info_target = SelectCrawler.get(
             parent_query, alias_info.from_expression_element
         )[0]
         if isinstance(select_info_target, str):
             cte = query.lookup_cte(select_info_target)
             if cte:
                 self.__resolve_wildcard(
@@ -81,16 +81,16 @@
                 parent_query,
                 resolve_targets,
             )
 
     def __resolve_wildcard(
         self,
         context: RuleContext,
-        query,
-        parent_query,
+        query: Query,
+        parent_query: Query,
         resolve_targets,
     ):
         """Attempt to resolve the wildcard to a list of selectables."""
         process_queries = query.selectables
         # if one of the source queries for a query within the set is a
         # set expression, just use the first query. If that first query isn't
         # reflective of the others, that will be caught when that segment
@@ -134,14 +134,15 @@
                         for o in query_list:
                             if isinstance(o, Query):
                                 self.__resolve_wildcard(
                                     context, o, parent_query, resolve_targets
                                 )
                                 return resolve_targets
             else:
+                assert selectable.select_info
                 resolve_targets.extend(
                     [target for target in selectable.select_info.select_targets]
                 )
 
         return resolve_targets
 
     def _get_select_target_counts(self, context: RuleContext, crawler):
@@ -163,14 +164,16 @@
                 # stack to check whether they resolve to wildcards
 
                 select_crawler = SelectCrawler(
                     selectable.selectable,
                     context.dialect,
                     parent_stack=context.parent_stack,
                 ).query_tree
+                assert select_crawler
+                assert parent_crawler.query_tree
                 select_list = self.__resolve_wildcard(
                     context,
                     select_crawler,
                     parent_crawler.query_tree,
                     [],
                 )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         # function_name). Then it is likely an existing user defined function (UDF)
         # which are case sensitive so ignore for this.
         if parent.get_type() == "function_name" and len(parent.segments) != 1:
             return [LintResult(memory=context.memory)]
 
         return [self._handle_segment(context.segment, context)]
 
-    def _handle_segment(self, segment, context: RuleContext) -> LintResult:
+    def _handle_segment(self, segment: BaseSegment, context: RuleContext) -> LintResult:
         # NOTE: this mutates the memory field.
         memory = context.memory
         self.logger.info("_handle_segment: %s, %s", segment, segment.get_type())
         # Config type hints
         self.ignore_words_regex: str
 
         # Get the capitalisation policy configuration.
@@ -243,15 +243,15 @@
             return LintResult(
                 anchor=segment,
                 fixes=[self._get_fix(segment, fixed_raw)],
                 memory=memory,
                 description=f"{self._description_elem} must be {consistency}{policy}",
             )
 
-    def _get_fix(self, segment, fixed_raw):
+    def _get_fix(self, segment: BaseSegment, fixed_raw: str) -> LintFix:
         """Given a segment found to have a fix, returns a LintFix for it.
 
         May be overridden by subclasses, which is useful when the parse tree
         structure varies from this simple base case.
         """
         return LintFix.replace(segment, [segment.edit(fixed_raw)])
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV06.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,29 +57,30 @@
     groups = ("all", "convention")
     config_keywords = ["multiline_newline", "require_final_semicolon"]
     crawl_behaviour = RootOnlyCrawler()
     is_fix_compatible = True
 
     @staticmethod
     def _handle_preceding_inline_comments(
-        before_segment: Sequence[RawSegment], anchor_segment: BaseSegment
+        before_segment: Sequence[BaseSegment], anchor_segment: BaseSegment
     ):
         """Adjust segments to not move preceding inline comments.
 
         We don't want to move inline comments that are on the same line
         as the preceding code segment as they could contain noqa instructions.
         """
         # See if we have a preceding inline comment on the same line as the preceding
         # segment.
         same_line_comment = next(
             (
                 s
                 for s in before_segment
                 if s.is_comment
                 and not s.is_type("block_comment")
+                and s.pos_marker
                 and s.pos_marker.working_line_no
                 # We don't need to handle the case where raw_segments is empty
                 # because it never is. It's either a segment with raw children
                 # or a raw segment which returns [self] as raw_segments.
                 == anchor_segment.raw_segments[-1].pos_marker.working_line_no
             ),
             None,
@@ -89,33 +90,39 @@
         if same_line_comment:
             anchor_segment = same_line_comment
             before_segment = before_segment[: before_segment.index(same_line_comment)]
 
         return before_segment, anchor_segment
 
     @staticmethod
-    def _handle_trailing_inline_comments(parent_segment, anchor_segment):
+    def _handle_trailing_inline_comments(
+        parent_segment: BaseSegment, anchor_segment: BaseSegment
+    ) -> BaseSegment:
         """Adjust anchor_segment to not move trailing inline comment.
 
         We don't want to move inline comments that are on the same line
         as the preceding code segment as they could contain noqa instructions.
         """
         # See if we have a trailing inline comment on the same line as the preceding
         # segment.
         for comment_segment in parent_segment.recursive_crawl("comment"):
+            assert comment_segment.pos_marker
+            assert anchor_segment.pos_marker
             if (
                 comment_segment.pos_marker.working_line_no
                 == anchor_segment.pos_marker.working_line_no
             ) and (not comment_segment.is_type("block_comment")):
                 anchor_segment = comment_segment
 
         return anchor_segment
 
     @staticmethod
-    def _is_one_line_statement(parent_segment, segment):
+    def _is_one_line_statement(
+        parent_segment: BaseSegment, segment: BaseSegment
+    ) -> bool:
         """Check if the statement containing the provided segment is one line."""
         # Find statement segment containing the current segment.
         statement_segment = next(
             (
                 ps.segment
                 for ps in (parent_segment.path_to(segment) or [])
                 if ps.segment.is_type("statement")
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV09.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Implementation of Rule CV09."""
 
 import regex
-from typing import Optional
+from typing import List, Optional
 
 from sqlfluff.core.rules import BaseRule, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 
 
 class Rule_CV09(BaseRule):
     """Block a list of configurable words from being used.
@@ -97,15 +97,15 @@
                         return LintResult(
                             anchor=context.segment,
                             description=f"Use of blocked regex '{source_str}'.",
                         )
 
         return None
 
-    def _init_blocked_words(self):
+    def _init_blocked_words(self) -> List[str]:
         """Called first time rule is evaluated to fetch & cache the blocked_words."""
         blocked_words_config = getattr(self, "blocked_words")
         if blocked_words_config:
             self.blocked_words_list = self.split_comma_separated_string(
                 blocked_words_config.upper()
             )
         else:  # pragma: no cover
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/convention/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """The convention plugin bundle."""
 
 from sqlfluff.core.plugin import hookimpl
-
-from sqlfluff.rules.convention.CV01 import Rule_CV01
-from sqlfluff.rules.convention.CV02 import Rule_CV02
-from sqlfluff.rules.convention.CV03 import Rule_CV03
-from sqlfluff.rules.convention.CV04 import Rule_CV04
-from sqlfluff.rules.convention.CV05 import Rule_CV05
-from sqlfluff.rules.convention.CV06 import Rule_CV06
-from sqlfluff.rules.convention.CV07 import Rule_CV07
-from sqlfluff.rules.convention.CV08 import Rule_CV08
-from sqlfluff.rules.convention.CV09 import Rule_CV09
-from sqlfluff.rules.convention.CV10 import Rule_CV10
-from sqlfluff.rules.convention.CV11 import Rule_CV11
+from sqlfluff.core.rules import BaseRule
+from typing import List, Type
 
 
 @hookimpl
-def get_rules():
-    """Get plugin rules."""
+def get_rules() -> List[Type[BaseRule]]:
+    """Get plugin rules.
+
+    NOTE: Rules are imported only on fetch to manage import times
+    when rules aren't used.
+    """
+    from sqlfluff.rules.convention.CV01 import Rule_CV01
+    from sqlfluff.rules.convention.CV02 import Rule_CV02
+    from sqlfluff.rules.convention.CV03 import Rule_CV03
+    from sqlfluff.rules.convention.CV04 import Rule_CV04
+    from sqlfluff.rules.convention.CV05 import Rule_CV05
+    from sqlfluff.rules.convention.CV06 import Rule_CV06
+    from sqlfluff.rules.convention.CV07 import Rule_CV07
+    from sqlfluff.rules.convention.CV08 import Rule_CV08
+    from sqlfluff.rules.convention.CV09 import Rule_CV09
+    from sqlfluff.rules.convention.CV10 import Rule_CV10
+    from sqlfluff.rules.convention.CV11 import Rule_CV11
+
     return [
         Rule_CV01,
         Rule_CV02,
         Rule_CV03,
         Rule_CV04,
         Rule_CV05,
         Rule_CV06,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT03.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 
     name = "layout.operators"
     aliases = ("L007",)
     groups = ("all", "layout")
     crawl_behaviour = SegmentSeekerCrawler({"binary_operator", "comparison_operator"})
     is_fix_compatible = True
 
-    def _seek_newline(self, segments: Sequence[BaseSegment], idx: int, dir: int):
+    def _seek_newline(
+        self, segments: Sequence[BaseSegment], idx: int, dir: int
+    ) -> bool:
         """Seek in a direction, looking for newlines.
 
         Args:
             segments: A sequence of segments to seek within.
             idx: The index of the "current" segment.
             dir: The direction to seek in (+1 for forward, -1 for backward)
         """
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT05.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,25 @@
 
         # Ignore any comment line if appropriate.
         if self.ignore_comment_lines:
             raw_segments = context.segment.raw_segments
             for res in results[:]:
                 # First handle the easy case that the anchor (i.e. the start
                 # of the line is a comment).
+                assert res.anchor
+                assert res.anchor.pos_marker
                 if res.anchor.is_type("comment"):
                     self.logger.debug(
                         "Purging result on long line starting with comment: %s",
                         res.anchor.pos_marker.working_line_no,
                     )
                     results.remove(res)
                     continue
                 # Then look for comments on the rest of the line:
+                assert res.anchor.pos_marker
                 raw_idx = raw_segments.index(res.anchor)
                 for seg in raw_segments[raw_idx:]:
                     if (
                         seg.pos_marker.working_line_no
                         != res.anchor.pos_marker.working_line_no
                     ):
                         # We've gone past the end of the line. Stop looking.
@@ -85,14 +88,16 @@
         # Ignore any comment clauses if present.
         if self.ignore_comment_clauses:
             raw_segments = context.segment.raw_segments
             for res in results[:]:
                 # The anchor should be the first raw on the line. Work forward
                 # until we're not on the line. Check if any have a parent which
                 # is a comment_clause.
+                assert res.anchor
+                assert res.anchor.pos_marker
                 raw_idx = raw_segments.index(res.anchor)
                 for seg in raw_segments[raw_idx:]:
                     if (
                         seg.pos_marker.working_line_no
                         != res.anchor.pos_marker.working_line_no
                     ):
                         # We've gone past the end of the line. Stop looking.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT07.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     NewlineSegment,
 )
 
 from sqlfluff.core.rules import BaseRule, LintFix, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.utils.functional import sp, FunctionalContext
 
+from typing import Optional
+
 
 class Rule_LT07(BaseRule):
     """``WITH`` clause closing bracket should be on a new line.
 
     **Anti-pattern**
 
     In this example, the closing bracket is on the same line as CTE.
@@ -43,15 +45,15 @@
     aliases = ("L018",)
     groups = ("all", "core", "layout")
     crawl_behaviour = SegmentSeekerCrawler(
         {"with_compound_statement"}, provide_raw_stack=True
     )
     is_fix_compatible = True
 
-    def _eval(self, context: RuleContext):
+    def _eval(self, context: RuleContext) -> Optional[LintResult]:
         """WITH clause closing bracket should be aligned with WITH keyword.
 
         Look for a with clause and evaluate the position of closing brackets.
         """
         # We only trigger on start_bracket (open parenthesis)
         assert context.segment.is_type("with_compound_statement")
 
@@ -120,7 +122,9 @@
                             seg,
                             [
                                 NewlineSegment(),
                             ],
                         )
                     ],
                 )
+
+        return None
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT09.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     name = "layout.select_targets"
     aliases = ("L036",)
     groups = ("all", "layout")
     config_keywords = ["wildcard_policy"]
     crawl_behaviour = SegmentSeekerCrawler({"select_clause"})
     is_fix_compatible = True
 
-    def _eval(self, context: RuleContext):
+    def _eval(self, context: RuleContext) -> Optional[LintResult]:
         self.wildcard_policy: str
         assert context.segment.is_type("select_clause")
         select_targets_info = self._get_indexes(context)
         select_clause = FunctionalContext(context).segment
         wildcards = select_clause.children(
             sp.is_type("select_clause_element")
         ).children(sp.is_type("wildcard_expression"))
@@ -101,17 +101,18 @@
                 select_targets_info,
                 context,
             )
         elif len(select_targets_info.select_targets):
             return self._eval_multiple_select_target_elements(
                 select_targets_info, context.segment
             )
+        return None
 
     @staticmethod
-    def _get_indexes(context: RuleContext):
+    def _get_indexes(context: RuleContext) -> SelectTargetsInfo:
         children = FunctionalContext(context).segment.children()
         select_targets = children.select(sp.is_type("select_clause_element"))
         first_select_target_idx = children.find(select_targets.get())
         selects = children.select(sp.is_keyword("select"))
         select_idx = children.find(selects.get()) if selects else -1
         newlines = children.select(sp.is_type("newline"))
         first_new_line_idx = children.find(newlines.get()) if newlines else -1
@@ -153,15 +154,17 @@
             first_whitespace_idx,
             comment_after_select_idx,
             select_targets,
             from_segment,
             list(pre_from_whitespace),
         )
 
-    def _eval_multiple_select_target_elements(self, select_targets_info, segment):
+    def _eval_multiple_select_target_elements(
+        self, select_targets_info, segment
+    ) -> Optional[LintResult]:
         """Multiple select targets. Ensure each is on a separate line."""
         # Insert newline before every select target.
         fixes = []
         for i, select_target in enumerate(select_targets_info.select_targets):
             base_segment = (
                 segment if not i else select_targets_info.select_targets[i - 1]
             )
@@ -206,14 +209,16 @@
                             [NewlineSegment()],
                         )
                     )
 
         if fixes:
             return LintResult(anchor=segment, fixes=fixes)
 
+        return None
+
     def _eval_single_select_target_element(
         self, select_targets_info, context: RuleContext
     ):
         select_clause = FunctionalContext(context).segment
         parent_stack = context.parent_stack
 
         # If it's all on one line, then there's no issue.
@@ -344,21 +349,22 @@
                             fixes.append(LintFix.delete(seg))
                             all_deletes.add(seg)
                     fixes_ += [
                         LintFix.delete(seg)
                         for seg in move_after_select_clause
                         if seg not in all_deletes
                     ]
-                    fixes_.append(
-                        LintFix.create_after(
-                            select_clause[0],
-                            ([NewlineSegment()] if add_newline else [])
-                            + list(move_after_select_clause),
+                    if move_after_select_clause or add_newline:
+                        fixes_.append(
+                            LintFix.create_after(
+                                select_clause[0],
+                                ([NewlineSegment()] if add_newline else [])
+                                + list(move_after_select_clause),
+                            )
                         )
-                    )
                     return fixes_
 
                 if select_stmt.segments[after_select_clause_idx].is_type("newline"):
                     # Since we're deleting the newline, we should also delete all
                     # whitespace before it or it will add random whitespace to
                     # following statements. So walk back through the segment
                     # deleting whitespace until you get the previous newline, or
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/layout/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """The aliasing plugin bundle."""
 
 from sqlfluff.core.plugin import hookimpl
-
-from sqlfluff.rules.layout.LT01 import Rule_LT01
-from sqlfluff.rules.layout.LT02 import Rule_LT02
-from sqlfluff.rules.layout.LT03 import Rule_LT03
-from sqlfluff.rules.layout.LT04 import Rule_LT04
-from sqlfluff.rules.layout.LT05 import Rule_LT05
-from sqlfluff.rules.layout.LT06 import Rule_LT06
-from sqlfluff.rules.layout.LT07 import Rule_LT07
-from sqlfluff.rules.layout.LT08 import Rule_LT08
-from sqlfluff.rules.layout.LT09 import Rule_LT09
-from sqlfluff.rules.layout.LT10 import Rule_LT10
-from sqlfluff.rules.layout.LT11 import Rule_LT11
-from sqlfluff.rules.layout.LT12 import Rule_LT12
-from sqlfluff.rules.layout.LT13 import Rule_LT13
+from sqlfluff.core.rules import BaseRule
+from typing import List, Type
 
 
 @hookimpl
-def get_rules():
-    """Get plugin rules."""
+def get_rules() -> List[Type[BaseRule]]:
+    """Get plugin rules.
+
+    NOTE: Rules are imported only on fetch to manage import times
+    when rules aren't used.
+    """
+    from sqlfluff.rules.layout.LT01 import Rule_LT01
+    from sqlfluff.rules.layout.LT02 import Rule_LT02
+    from sqlfluff.rules.layout.LT03 import Rule_LT03
+    from sqlfluff.rules.layout.LT04 import Rule_LT04
+    from sqlfluff.rules.layout.LT05 import Rule_LT05
+    from sqlfluff.rules.layout.LT06 import Rule_LT06
+    from sqlfluff.rules.layout.LT07 import Rule_LT07
+    from sqlfluff.rules.layout.LT08 import Rule_LT08
+    from sqlfluff.rules.layout.LT09 import Rule_LT09
+    from sqlfluff.rules.layout.LT10 import Rule_LT10
+    from sqlfluff.rules.layout.LT11 import Rule_LT11
+    from sqlfluff.rules.layout.LT12 import Rule_LT12
+    from sqlfluff.rules.layout.LT13 import Rule_LT13
+
     return [
         Rule_LT01,
         Rule_LT02,
         Rule_LT03,
         Rule_LT04,
         Rule_LT05,
         Rule_LT06,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF01.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     def _analyze_table_references(
         self,
         query: RF01Query,
         dml_target_table: Optional[Tuple[str, ...]],
         dialect: Dialect,
         violations: List[LintResult],
-    ):
+    ) -> None:
         # For each query...
         for selectable in query.selectables:
             select_info = selectable.select_info
             self.logger.debug(
                 "Selectable: %s",
                 selectable,
             )
@@ -168,15 +168,15 @@
         # Visit children.
         for child in query.children:
             self._analyze_table_references(
                 cast(RF01Query, child), dml_target_table, dialect, violations
             )
 
     @staticmethod
-    def _should_ignore_reference(reference, selectable):
+    def _should_ignore_reference(reference, selectable) -> bool:
         ref_path = selectable.selectable.path_to(reference)
         # Ignore references occurring in an "INTO" clause:
         # - They are table references, not column references.
         # - They are the target table, similar to an INSERT or UPDATE
         #   statement, thus not expected to match a table in the FROM
         #   clause.
         if ref_path:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF02.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Implementation of Rule RF02."""
 import regex
 from typing import List, Optional
-
+from sqlfluff.core.dialects.common import AliasInfo, ColumnAliasInfo
+from sqlfluff.core.parser import BaseSegment
 from sqlfluff.core.rules import LintResult
 from sqlfluff.rules.aliasing.AL04 import Rule_AL04
 
 
 class Rule_RF02(Rule_AL04):
     """References should be qualified if select has more than one referenced table/view.
 
@@ -37,20 +38,20 @@
     name = "references.qualification"
     aliases = ("L027",)
     groups = ("all", "references")
     # Crawl behaviour is defined in AL04
 
     def _lint_references_and_aliases(
         self,
-        table_aliases,
-        standalone_aliases,
+        table_aliases: List[AliasInfo],
+        standalone_aliases: List[str],
         references,
-        col_aliases,
-        using_cols,
-        parent_select,
+        col_aliases: List[ColumnAliasInfo],
+        using_cols: List[str],
+        parent_select: Optional[BaseSegment],
     ) -> Optional[List[LintResult]]:
         # Config type hints
         self.ignore_words_regex: str
 
         # Do we have more than one? If so, all references should be qualified.
         if len(table_aliases) <= 1:
             return None
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF03.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     LintFix,
     LintResult,
     EvalResultType,
     RuleContext,
 )
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.utils.functional import sp, FunctionalContext
-from sqlfluff.dialects.dialect_ansi import IdentifierSegment
+from sqlfluff.dialects.dialect_ansi import IdentifierSegment, ObjectReferenceSegment
 
 
 _START_TYPES = ["select_statement", "set_expression", "with_compound_statement"]
 
 
 class Rule_RF03(BaseRule):
     """References should be consistent in statements with a single table.
@@ -157,33 +157,33 @@
         for child in children:
             yield from self._visit_queries(child, visited)
 
 
 def _check_references(
     table_aliases: List[AliasInfo],
     standalone_aliases: List[str],
-    references: List[BaseSegment],
+    references: List[ObjectReferenceSegment],
     col_aliases: List[ColumnAliasInfo],
     single_table_references: str,
     is_struct_dialect: bool,
     fix_inconsistent_to: Optional[str],
     fixable: bool,
 ) -> Iterator[LintResult]:
     """Iterate through references and check consistency."""
     # A buffer to keep any violations.
     col_alias_names: List[str] = [c.alias_identifier_name for c in col_aliases]
     table_ref_str: str = table_aliases[0].ref_str
     table_ref_str_source = table_aliases[0].segment
     # Check all the references that we have.
     seen_ref_types: Set[str] = set()
     for ref in references:
-        this_ref_type: str = ref.qualification()  # type: ignore
+        this_ref_type: str = ref.qualification()
         if this_ref_type == "qualified" and is_struct_dialect:
             # If this col appears "qualified" check if it is more logically a struct.
-            if next(ref.iter_raw_references()).part != table_ref_str:  # type: ignore
+            if next(ref.iter_raw_references()).part != table_ref_str:
                 this_ref_type = "unqualified"
 
         lint_res = _validate_one_reference(
             single_table_references,
             ref,
             this_ref_type,
             standalone_aliases,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF04.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Implementation of Rule RF04."""
 import regex
-from typing import Optional
+from typing import List, Optional
 
 from sqlfluff.core.rules import BaseRule, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.utils.identifers import identifiers_policy_applicable
 
 
 class Rule_RF04(BaseRule):
@@ -106,15 +106,15 @@
                 )
             )
         ):
             return LintResult(anchor=context.segment)
         else:
             return None
 
-    def _init_ignore_string(self):
+    def _init_ignore_string(self) -> List[str]:
         """Called first time rule is evaluated to fetch & cache the ignore_words."""
         # Use str() in case bools are passed which might otherwise be read as bool
         ignore_words_config = str(getattr(self, "ignore_words"))
         if ignore_words_config and ignore_words_config != "None":
             self.ignore_words_list = self.split_comma_separated_string(
                 ignore_words_config.lower()
             )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/references/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """The references plugin bundle."""
 
 from sqlfluff.core.plugin import hookimpl
-
-from sqlfluff.rules.references.RF01 import Rule_RF01
-from sqlfluff.rules.references.RF02 import Rule_RF02
-from sqlfluff.rules.references.RF03 import Rule_RF03
-from sqlfluff.rules.references.RF04 import Rule_RF04
-from sqlfluff.rules.references.RF05 import Rule_RF05
-from sqlfluff.rules.references.RF06 import Rule_RF06
+from sqlfluff.core.rules import BaseRule
+from typing import List, Type
 
 
 @hookimpl
-def get_rules():
-    """Get plugin rules."""
+def get_rules() -> List[Type[BaseRule]]:
+    """Get plugin rules.
+
+    NOTE: Rules are imported only on fetch to manage import times
+    when rules aren't used.
+    """
+    from sqlfluff.rules.references.RF01 import Rule_RF01
+    from sqlfluff.rules.references.RF02 import Rule_RF02
+    from sqlfluff.rules.references.RF03 import Rule_RF03
+    from sqlfluff.rules.references.RF04 import Rule_RF04
+    from sqlfluff.rules.references.RF05 import Rule_RF05
+    from sqlfluff.rules.references.RF06 import Rule_RF06
+
     return [Rule_RF01, Rule_RF02, Rule_RF03, Rule_RF04, Rule_RF05, Rule_RF06]
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST03.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def _find_all_ctes(cls, query: Query) -> Iterator[Query]:
         if query.ctes:
             yield query
         for query in query.ctes.values():
             yield from cls._find_all_ctes(query)
 
     @classmethod
-    def _visit_sources(cls, query: Query):
+    def _visit_sources(cls, query: Query) -> None:
         for selectable in query.selectables:
             for source in query.crawl_sources(selectable.selectable, pop=True):
                 if isinstance(source, Query):
                     cls._visit_sources(source)
         for child in query.children:
             cls._visit_sources(child)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST05.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         if result:
             lint_result, from_expression, alias_name, subquery_parent = result
             assert any(
                 from_expression is seg for seg in subquery_parent.recursive_crawl_all()
             )
             this_seg_clone = clone_map[from_expression]
             new_table_ref = _create_table_ref(alias_name, context.dialect)
-            this_seg_clone.segments = [new_table_ref]
+            this_seg_clone.segments = (new_table_ref,)
             ctes.replace_with_clone(subquery_parent, clone_map)
 
             # Issue 3617: In T-SQL (and possibly other dialects) the automated fix
             # leaves parentheses in a location that causes a syntax error. This is an
             # unusual corner case. For simplicity, we still generate the lint warning
             # but don't try to generate a fix. Someone could look at this later (a
             # correct fix would involve removing the parentheses.)
@@ -237,15 +237,15 @@
                         )
 
     def _lint_query(
         self,
         dialect: Dialect,
         query: Query,
         ctes: "_CTEBuilder",
-        case_preference,
+        case_preference: str,
         clone_map,
     ) -> Optional[Tuple[LintResult, BaseSegment, str, BaseSegment]]:
         """Given the root query, compute lint warnings."""
         nsq: _NestedSubQuerySummary
         for nsq in self._nested_subqueries(query, dialect):
             alias_name, is_new_name = ctes.create_cte_alias(nsq.table_alias)
             # 'anchor' is the TableExpressionSegment we fix/replace w/CTE name.
@@ -291,28 +291,26 @@
         # We only want the first one.
         return select_statement
     return None  # pragma: no cover
 
 
 def _is_correlated_subquery(
     nested_select: Segments, select_source_names: Set[str], dialect: Dialect
-):
+) -> bool:
     """Given nested select and the sources of its parent, determine if correlated.
 
     https://en.wikipedia.org/wiki/Correlated_subquery
     """
     select_statement = _get_first_select_statement_descendant(nested_select[0])
     if not select_statement:
         return False  # pragma: no cover
     nested_select_info = get_select_statement_info(select_statement, dialect)
     if nested_select_info:
         for r in nested_select_info.reference_buffer:
-            for tr in r.extract_possible_references(  # type: ignore
-                level=r.ObjectReferenceLevel.TABLE  # type: ignore
-            ):
+            for tr in r.extract_possible_references(level=r.ObjectReferenceLevel.TABLE):
                 # Check for correlated subquery, as indicated by use of a
                 # parent reference.
                 if tr.part in select_source_names:
                     return True
     return False
 
 
@@ -335,15 +333,15 @@
             used_names.append(cte_name)
         return used_names
 
     def has_duplicate_aliases(self) -> bool:
         used_names = self.list_used_names()
         return len(set(used_names)) != len(used_names)
 
-    def insert_cte(self, cte: CTEDefinitionSegment):
+    def insert_cte(self, cte: CTEDefinitionSegment) -> None:
         """Add a new CTE to the list as late as possible but before all its parents."""
         # This should still have the position markers of its true position
         inbound_subquery = (
             Segments(cte).children().last(lambda seg: bool(seg.pos_marker))
         )
         insert_position = next(
             (
@@ -399,15 +397,15 @@
         return new_select
 
     def ensure_space_after_from(
         self,
         output_select: BaseSegment,
         output_select_clone: BaseSegment,
         subquery_parent: BaseSegment,
-    ):
+    ) -> List[LintFix]:
         """Ensure there's whitespace between "FROM" and the CTE table name."""
         fixes = []
         if subquery_parent is output_select:
             (
                 missing_space_after_from,
                 from_clause,
                 from_clause_children,
@@ -436,33 +434,33 @@
                 # modify it directly. Create a LintFix to do it.
                 fixes.append(
                     LintFix.create_after(from_segment[0], [WhitespaceSegment()])
                 )
         return fixes
 
     @staticmethod
-    def _missing_space_after_from(segment):
+    def _missing_space_after_from(segment: BaseSegment):
         missing_space_after_from = False
         from_clause_children = None
         from_segment = None
         from_clause = segment.get_child("from_clause")
         if from_clause is not None:
             from_clause_children = Segments(*from_clause.segments)
             from_segment = from_clause_children.first(is_keyword("from"))
             if from_segment and not from_clause_children.select(
                 start_seg=from_segment[0], loop_while=is_whitespace()
             ):
                 missing_space_after_from = True
         return missing_space_after_from, from_clause, from_clause_children, from_segment
 
-    def replace_with_clone(self, segment, clone_map):
+    def replace_with_clone(self, segment, clone_map) -> None:
         for idx, cte in enumerate(self.ctes):
             if any(segment is seg for seg in cte.recursive_crawl_all()):
                 self.ctes[idx] = clone_map[self.ctes[idx]]
-                return
+                return None
 
 
 def _is_child(maybe_parent: Segments, maybe_child: Segments) -> bool:
     """Is the child actually between the start and end markers of the parent."""
     assert (
         len(maybe_child) == 1
     ), "Cannot assess child relationship of multiple segments"
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST06.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,29 +128,29 @@
             for i, band in enumerate(select_element_order_preference):
                 for e in band:
                     # Identify simple select target
                     if segment.get_child(e):
                         self._validate(i, segment)
 
                     # Identify function
-                    elif type(e) == tuple and e[0] == "function":
+                    elif isinstance(e, tuple) and e[0] == "function":
                         try:
                             if (
                                 segment.get_child("function")
                                 .get_child("function_name")
                                 .raw
                                 == e[1]
                             ):
                                 self._validate(i, segment)
                         except AttributeError:
                             # If the segment doesn't match
                             pass
 
                     # Identify simple expression
-                    elif type(e) == tuple and e[0] == "expression":
+                    elif isinstance(e, tuple) and e[0] == "expression":
                         try:
                             if (
                                 segment.get_child("expression").get_child(e[1])
                                 and segment.get_child("expression").segments[0].type
                                 in (
                                     "column_reference",
                                     "object_reference",
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST07.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,17 @@
         .first()
         .children(sp.is_type("identifier"))
         .apply(lambda el: el.raw)
     )
     return using_cols
 
 
-def _generate_join_conditions(table_a_ref: str, table_b_ref: str, columns: List[str]):
+def _generate_join_conditions(
+    table_a_ref: str, table_b_ref: str, columns: List[str]
+) -> List[BaseSegment]:
     edit_segments: List[BaseSegment] = []
     for col in columns:
         edit_segments = edit_segments + [
             _create_col_reference(
                 table_a_ref,
                 col,
             ),
@@ -205,14 +207,14 @@
 
         to_delete.append(seg)
 
     assert insert_anchor, "Insert Anchor must be present at this point"
     return to_delete, insert_anchor
 
 
-def _create_col_reference(table_ref: str, column_name: str):
-    segments = [
+def _create_col_reference(table_ref: str, column_name: str) -> ColumnReferenceSegment:
+    segments = (
         IdentifierSegment(raw=table_ref, type="naked_identifier"),
         SymbolSegment(raw=".", type="symbol"),
         IdentifierSegment(raw=column_name, type="naked_identifier"),
-    ]
+    )
     return ColumnReferenceSegment(segments=segments, pos_marker=None)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/structure/ST08.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implementation of Rule ST08."""
-from typing import Optional
+from typing import Optional, Tuple
 
-from sqlfluff.core.parser import KeywordSegment, WhitespaceSegment
+from sqlfluff.core.parser import KeywordSegment, WhitespaceSegment, BaseSegment
 from sqlfluff.core.rules import BaseRule, LintFix, LintResult, RuleContext
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
-from sqlfluff.utils.functional import sp, FunctionalContext
+from sqlfluff.utils.functional import sp, FunctionalContext, Segments
 from sqlfluff.utils.reflow.sequence import ReflowSequence
 
 
 class Rule_ST08(BaseRule):
     """``DISTINCT`` used with parentheses.
 
     **Anti-pattern**
@@ -113,15 +113,17 @@
             if fixes:
                 return LintResult(
                     anchor=anchor,
                     fixes=fixes,
                 )
         return None
 
-    def _remove_unneeded_brackets(self, context, bracketed):
+    def _remove_unneeded_brackets(
+        self, context: RuleContext, bracketed: Segments
+    ) -> Tuple[BaseSegment, ReflowSequence]:
         # Remove the brackets and strip any meta segments.
         anchor = bracketed.get()
         assert anchor
         seq = ReflowSequence.from_around_target(
             anchor,
             context.parent_stack[0],
             config=context.config,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-"""The structure plugin bundle."""
+"""The ambiguous plugin bundle.
 
-from sqlfluff.core.plugin import hookimpl
+NOTE: Yes the title of this bundle is ...ambiguous. 😁
+"""
 
-from sqlfluff.rules.structure.ST01 import Rule_ST01
-from sqlfluff.rules.structure.ST02 import Rule_ST02
-from sqlfluff.rules.structure.ST03 import Rule_ST03
-from sqlfluff.rules.structure.ST04 import Rule_ST04
-from sqlfluff.rules.structure.ST05 import Rule_ST05
-from sqlfluff.rules.structure.ST06 import Rule_ST06
-from sqlfluff.rules.structure.ST07 import Rule_ST07
-from sqlfluff.rules.structure.ST08 import Rule_ST08
+from sqlfluff.core.plugin import hookimpl
+from sqlfluff.core.rules import BaseRule
+from typing import List, Type
 
 
 @hookimpl
-def get_rules():
-    """Get plugin rules."""
-    return [
-        Rule_ST01,
-        Rule_ST02,
-        Rule_ST03,
-        Rule_ST04,
-        Rule_ST05,
-        Rule_ST06,
-        Rule_ST07,
-        Rule_ST08,
-    ]
+def get_rules() -> List[Type[BaseRule]]:
+    """Get plugin rules.
+
+    NOTE: Rules are imported only on fetch to manage import times
+    when rules aren't used.
+    """
+    from sqlfluff.rules.ambiguous.AM01 import Rule_AM01
+    from sqlfluff.rules.ambiguous.AM02 import Rule_AM02
+    from sqlfluff.rules.ambiguous.AM03 import Rule_AM03
+    from sqlfluff.rules.ambiguous.AM04 import Rule_AM04
+    from sqlfluff.rules.ambiguous.AM05 import Rule_AM05
+    from sqlfluff.rules.ambiguous.AM06 import Rule_AM06
+    from sqlfluff.rules.ambiguous.AM07 import Rule_AM07
+
+    return [Rule_AM01, Rule_AM02, Rule_AM03, Rule_AM04, Rule_AM05, Rule_AM06, Rule_AM07]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.2.0/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/analysis/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Basic code analysis tools for SELECT statements."""
 from typing import List, NamedTuple, Optional
 
 from sqlfluff.core.dialects.base import Dialect
+from sqlfluff.dialects.dialect_ansi import ObjectReferenceSegment
 from sqlfluff.core.dialects.common import AliasInfo, ColumnAliasInfo
 from sqlfluff.core.parser.segments.base import BaseSegment
 
 
 class SelectStatementColumnsAndTables(NamedTuple):
     """Structure returned by get_select_statement_info()."""
 
     select_statement: BaseSegment
     table_aliases: List[AliasInfo]
     standalone_aliases: List[str]  # value table function aliases
-    reference_buffer: List[BaseSegment]
+    reference_buffer: List[ObjectReferenceSegment]
     select_targets: List[BaseSegment]
     col_aliases: List[ColumnAliasInfo]
     using_cols: List[str]
 
 
 def get_select_statement_info(
     segment: BaseSegment, dialect: Optional[Dialect], early_exit: bool = True
@@ -123,15 +124,15 @@
                 standalone_aliases.append(alias_info[0])
         elif alias_info not in table_aliases:
             table_aliases.append(alias_info)
 
     return table_aliases, standalone_aliases
 
 
-def _has_value_table_function(table_expr, dialect):
+def _has_value_table_function(table_expr, dialect) -> bool:
     if not dialect:
         # We need the dialect to get the value table function names. If
         # we don't have it, assume the clause does not have a value table
         # function.
         return False  # pragma: no cover
 
     for function_name in table_expr.recursive_crawl("function_name"):
@@ -139,15 +140,15 @@
         # remove
         # See: https://github.com/sqlfluff/sqlfluff/issues/1304
         if function_name.raw.upper().strip() in dialect.sets("value_table_functions"):
             return True
     return False
 
 
-def _get_pivot_table_columns(segment, dialect):
+def _get_pivot_table_columns(segment, dialect) -> list:
     if not dialect:
         # We need the dialect to get the pivot table column names. If
         # we don't have it, assume the clause does not have a pivot table
         return []  # pragma: no cover
 
     fc = segment.recursive_crawl("from_pivot_expression")
     if not fc:
@@ -165,15 +166,17 @@
 
 # Lambda arguments,
 # e.g. `x` and `y` in `x -> x is not null` and `(x, y) -> x + y`
 # are declared in-place, and are as such standalone – i.e. they do not reference
 # identifiers or columns that we should expect to be declared somewhere else.
 # These columns are interesting to identify since they can get special
 # treatment in some rules.
-def _get_lambda_argument_columns(segment, dialect):
+def _get_lambda_argument_columns(
+    segment: BaseSegment, dialect: Dialect
+) -> Optional[List[str]]:
     if not dialect or dialect.name not in ["athena", "sparksql"]:
         # Only athena and sparksql are known to have lambda expressions,
         # so all other dialects will have zero lambda columns
         return []
 
     lambda_argument_columns = []
     for potential_lambda in segment.recursive_crawl("expression"):
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     dialect: Dialect
 
     def as_str(self) -> str:
         """String representation for logging/testing."""
         return self.selectable.raw
 
     @cached_property
-    def select_info(self):
+    def select_info(self) -> Optional[SelectStatementColumnsAndTables]:
         """Returns SelectStatementColumnsAndTables on the SELECT."""
         if self.selectable.is_type("select_statement"):
             return get_select_statement_info(
                 self.selectable, self.dialect, early_exit=False
             )
         else:  # DML or values_clause
             # This is a bit dodgy, but a very useful abstraction. Here, we
@@ -242,15 +242,15 @@
 
         # Stack of segments currently being processed
         query_stack: List[Query] = []
         # Tracks which segments caused a Query to be added to query_stack,
         # so we can pop "query_stack" when those segments complete processing.
         pop_queries_for = []
 
-        def append_query(query, parent_stack):
+        def append_query(query, parent_stack) -> None:
             """Bookkeeping when a new Query is created."""
             if query_stack:
                 query.parent = query_stack[-1]
                 query.parent.children.append(query)
             query_stack.append(query)
             if len(query_stack) == 1 and self.query_tree is None:
                 self.query_tree = query_stack[0]
@@ -262,15 +262,15 @@
                     self.query_tree.parent = SelectCrawler.get_parent_query(
                         parent_segment, dialect, parent_stack
                     )
                 else:
                     self.query_tree.parent = parent
             pop_queries_for.append(path[-1])
 
-        def finish_segment():
+        def finish_segment() -> None:
             """Bookkeeping when a segment finishes processing."""
             try:
                 idx = pop_queries_for.index(path[-1])
                 query_stack.pop()
                 del pop_queries_for[idx]
             except ValueError:
                 pass
@@ -435,10 +435,10 @@
         if recurse_into:
             for seg in seg.segments:
                 yield from cls.visit_segments(seg, path, recurse_into)
         yield "end", path
         path.pop()
 
     @classmethod
-    def get_parent_query(cls, seg, dialect, parent_stack):
+    def get_parent_query(cls, seg, dialect, parent_stack) -> Optional[Query]:
         """Creates a query tree from a querys parent stack to create full path."""
         return cls(seg, dialect, parent_stack=parent_stack).query_tree
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,13 +42,13 @@
     def raw_stack(self) -> "Segments":  # pragma: no cover
         """Returns a Segments object for context.raw_stack."""
         return Segments(
             *self.context.raw_stack, templated_file=self.context.templated_file
         )
 
     @property
-    def raw_segments(self):  # pragma: no cover
+    def raw_segments(self) -> Segments:  # pragma: no cover
         """Returns a Segments object for all the raw segments in the file."""
         file_segment = self.context.parent_stack[0]
         return Segments(
             *file_segment.get_raw_segments(), templated_file=self.context.templated_file
         )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 
 def is_slice_type(
     *slice_types: str,
 ) -> Callable[[RawFileSlice], bool]:
     """Returns a function that determines if segment is one of the types."""
 
-    def _(raw_slice: RawFileSlice):
+    def _(raw_slice: RawFileSlice) -> bool:
         return any(raw_slice.slice_type == slice_type for slice_type in slice_types)
 
     return _
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 from sqlfluff.utils.functional.templated_file_slices import TemplatedFileSlices
 from sqlfluff.core.templaters.base import TemplatedFile
 
 
 def raw_is(*raws: str) -> Callable[[BaseSegment], bool]:  # pragma: no cover
     """Returns a function that determines if segment matches one of the raw inputs."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return segment.raw in raws
 
     return _
 
 
 def raw_upper_is(*raws: str) -> Callable[[BaseSegment], bool]:
     """Returns a function that determines if segment matches one of the raw inputs."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return segment.raw_upper in raws
 
     return _
 
 
 def is_type(*seg_type: str) -> Callable[[BaseSegment], bool]:
     """Returns a function that determines if segment is one of the types."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return segment.is_type(*seg_type)
 
     return _
 
 
-def is_keyword(*keyword_name) -> Callable[[BaseSegment], bool]:
+def is_keyword(*keyword_name: str) -> Callable[[BaseSegment], bool]:
     """Returns a function that determines if it's a matching keyword."""
     return and_(
         is_type("keyword"), raw_upper_is(*[raw.upper() for raw in keyword_name])
     )
 
 
 def is_code() -> Callable[[BaseSegment], bool]:
@@ -121,33 +121,33 @@
 
     return _
 
 
 def and_(*functions: Callable[[BaseSegment], bool]) -> Callable[[BaseSegment], bool]:
     """Returns a function that computes the functions and-ed together."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return all(function(segment) for function in functions)
 
     return _
 
 
 def or_(*functions: Callable[[BaseSegment], bool]) -> Callable[[BaseSegment], bool]:
     """Returns a function that computes the functions or-ed together."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return any(function(segment) for function in functions)
 
     return _
 
 
 def not_(fn: Callable[[BaseSegment], bool]) -> Callable[[BaseSegment], bool]:
     """Returns a function that computes: not fn()."""
 
-    def _(segment: BaseSegment):
+    def _(segment: BaseSegment) -> bool:
         return not fn(segment)
 
     return _
 
 
 def raw_slices(
     segment: BaseSegment,
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/segments.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     Provides useful operations on a sequence of segments to simplify rule creation.
     """
 
     def __new__(cls, *segments, templated_file=None):
         """Override new operator."""
         return super(Segments, cls).__new__(cls, segments)
 
-    def __init__(self, *_: BaseSegment, templated_file: Optional[TemplatedFile] = None):
+    def __init__(
+        self, *_: BaseSegment, templated_file: Optional[TemplatedFile] = None
+    ) -> None:
         self.templated_file = templated_file
 
     def __add__(self, segments_) -> "Segments":
         return Segments(
             *tuple(self).__add__(tuple(segments_)), templated_file=self.templated_file
         )
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 
 def is_slice_type(
     *slice_types: str,
 ) -> Callable[[TemplatedFileSlice], bool]:
     """Returns a function that determines if segment is one the types."""
 
-    def _(raw_slice: TemplatedFileSlice):
+    def _(raw_slice: TemplatedFileSlice) -> bool:
         return any(raw_slice.slice_type == slice_type for slice_type in slice_types)
 
     return _
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Provides useful operations on a sequence of slices to simplify rule creation.
     """
 
     def __new__(cls, *templated_slices, templated_file=None):
         """Override new operator."""
         return super(TemplatedFileSlices, cls).__new__(cls, templated_slices)
 
-    def __init__(self, *_: TemplatedFileSlice, templated_file: TemplatedFile):
+    def __init__(self, *_: TemplatedFileSlice, templated_file: TemplatedFile) -> None:
         self.templated_file = templated_file
 
     def all(
         self, predicate: Optional[Callable[[TemplatedFileSlice], bool]] = None
     ) -> bool:
         """Do all the templated slices match?"""
         for s in self:
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def incorporate(
         self,
         before: Optional[str] = None,
         after: Optional[str] = None,
         within: Optional[str] = None,
         line_position: Optional[str] = None,
         config: Optional[ConfigElementType] = None,
-    ):
+    ) -> None:
         """Mutate the config based on additional information."""
         config = config or {}
         self.spacing_before = (
             before or config.get("spacing_before", None) or self.spacing_before
         )
         self.spacing_after = (
             after or config.get("spacing_after", None) or self.spacing_after
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     stack_hashes: Tuple[int, ...]
     # This is a convenience cache to speed up operations.
     stack_hash_set: FrozenSet[int]
     stack_class_types: Tuple[FrozenSet[str], ...]
     stack_positions: Dict[int, StackPosition]
 
     @classmethod
-    def from_raw_and_stack(cls, raw: RawSegment, stack: Sequence[PathStep]):
+    def from_raw_and_stack(
+        cls, raw: RawSegment, stack: Sequence[PathStep]
+    ) -> "DepthInfo":
         """Construct from a raw and its stack."""
         stack_hashes = tuple(hash(ps.segment) for ps in stack)
         return cls(
             stack_depth=len(stack),
             stack_hashes=stack_hashes,
             stack_hash_set=frozenset(stack_hashes),
             stack_class_types=tuple(frozenset(ps.segment.class_types) for ps in stack),
@@ -83,15 +85,15 @@
         # We should expect there to be _at least_ one common ancestor, because
         # they should share the same file segment. If that's not the case we
         # we should error because it's likely a bug or programming error.
         assert common_hashes, "DepthInfo comparison shares no common ancestor!"
         common_depth = len(common_hashes)
         return self.stack_hashes[:common_depth]
 
-    def trim(self, amount: int):
+    def trim(self, amount: int) -> "DepthInfo":
         """Return a DepthInfo object with some amount trimmed."""
         if amount == 0:
             # The trivial case.
             return self
         new_hash_set = self.stack_hash_set.difference(self.stack_hashes[-amount:])
         return self.__class__(
             stack_depth=self.stack_depth - amount,
@@ -163,15 +165,15 @@
             raise KeyError(
                 "Tried to get depth info for unknown "
                 f"segment {raw} with UUID {raw.uuid}"
             ) from err
 
     def copy_depth_info(
         self, anchor: RawSegment, new_segment: RawSegment, trim: int = 0
-    ):
+    ) -> None:
         """Copy the depth info for one segment and apply to another.
 
         This mutates the existing depth map. That's ok because it's
         an idempotent operation and uuids should be unique.
 
         This is used in edits to a reflow sequence when new segments are
         inserted and can't infer their own depth info.
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,17 @@
 
     impulse: int
     trough: int
     # Defaults to an empty tuple if unset.
     implicit_indents: Tuple[int, ...] = ()
 
     @classmethod
-    def from_combination(cls, first: Optional["IndentStats"], second: "IndentStats"):
+    def from_combination(
+        cls, first: Optional["IndentStats"], second: "IndentStats"
+    ) -> "IndentStats":
         """Create IndentStats from two consecutive IndentStats.
 
         This is mostly used for combining the effects of indent and dedent
         tokens either side of a comment.
 
         NOTE: The *first* is considered optional, because if we're
         calling this function, we're assuming that there's always
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/reindent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 """Methods for deducing and understanding indents."""
 
 from collections import defaultdict
 from itertools import chain
 import logging
-from typing import Iterator, List, Optional, Set, Tuple, cast, Dict, DefaultDict
+from typing import (
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    cast,
+    Dict,
+    DefaultDict,
+    FrozenSet,
+)
 from dataclasses import dataclass
 from sqlfluff.core.errors import SQLFluffUserError
 
 from sqlfluff.core.parser.segments import Indent, SourceFix
 
 from sqlfluff.core.parser import (
     RawSegment,
@@ -80,15 +90,15 @@
     # i.e. An Indent segment which takes the balance from 1 to 2 but with
     # no newline is an untaken indent of value 2.
     # It also only covers untaken indents _before_ this point. If this point
     # is _also_ an untaken indent, we should be able to infer that ourselves.
     untaken_indents: Tuple[int, ...]
 
     @property
-    def closing_indent_balance(self):
+    def closing_indent_balance(self) -> int:
         return self.initial_indent_balance + self.indent_impulse
 
 
 @dataclass
 class _IndentLine:
     """Temporary structure for handing a line of indent points.
 
@@ -96,29 +106,29 @@
     for things like comments and templated elements, after
     constructing all the metadata for the points on the line.
     """
 
     initial_indent_balance: int
     indent_points: List[_IndentPoint]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Compressed repr method to ease logging."""
         return (
             f"IndentLine(iib={self.initial_indent_balance}, ipts=["
             + ", ".join(
                 f"iPt@{ip.idx}({ip.indent_impulse}, {ip.indent_trough}, "
                 f"{ip.initial_indent_balance}, {ip.last_line_break_idx}, "
                 f"{ip.is_line_break}, {ip.untaken_indents})"
                 for ip in self.indent_points
             )
             + "])"
         )
 
     @classmethod
-    def from_points(cls, indent_points: List[_IndentPoint]):
+    def from_points(cls, indent_points: List[_IndentPoint]) -> "_IndentLine":
         # Catch edge case for first line where we'll start with a
         # block if no initial indent.
         if indent_points[-1].last_line_break_idx:
             starting_balance = indent_points[0].closing_indent_balance
         else:
             starting_balance = 0
         return cls(starting_balance, indent_points)
@@ -150,15 +160,15 @@
     def is_all_templates(self, elements: ReflowSequenceType) -> bool:
         """Is this line made up of just template elements?"""
         block_segments = list(self._iter_block_segments(elements))
         return bool(block_segments) and all(
             seg.is_type("placeholder", "template_loop") for seg in block_segments
         )
 
-    def desired_indent_units(self, forced_indents: List[int]):
+    def desired_indent_units(self, forced_indents: List[int]) -> int:
         """Calculate the desired indent units.
 
         This is the heart of the indentation calculations.
 
         First we work out how many previous indents are untaken.
         In the easy case, we just use the number of untaken
         indents from previous points. The more complicated example
@@ -203,19 +213,19 @@
             self.indent_points[0].untaken_indents,
             self.indent_points[0].indent_impulse,
             self.indent_points[0].indent_trough,
             desired_indent,
         )
         return desired_indent
 
-    def closing_balance(self):
+    def closing_balance(self) -> int:
         """The closing indent balance of the line."""
         return self.indent_points[-1].closing_indent_balance
 
-    def opening_balance(self):
+    def opening_balance(self) -> int:
         """The opening indent balance of the line.
 
         NOTE: We use the first point for the starting balance rather than
         the line starting balance because we're using this to detect missing
         lines and if the line has been corrected then we don't want to do
         that.
         """
@@ -1441,15 +1451,15 @@
 
     return results
 
 
 def lint_indent_points(
     elements: ReflowSequenceType,
     single_indent: str,
-    skip_indentation_in: Set[str] = set(),
+    skip_indentation_in: FrozenSet[str] = frozenset(),
     allow_implicit_indents: bool = False,
 ) -> Tuple[ReflowSequenceType, List[LintResult]]:
     """Lint the indent points to check we have line breaks where we should.
 
     For linting indentation - we *first* need to make sure there are
     line breaks in all the places there should be. This takes an input
     set of indent points, and inserts additional line breaks in the
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/respace.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # We're in the utils module, but users will expect reflow
 # logs to appear in the context of rules. Hence it's a subset
 # of the rules logger.
 reflow_logger = logging.getLogger("sqlfluff.rules.reflow")
 
 
-def _unpack_constraint(constraint: str, strip_newlines: bool):
+def _unpack_constraint(constraint: str, strip_newlines: bool) -> Tuple[str, bool]:
     """Unpack a spacing constraint.
 
     Used as a helper function in `determine_constraints`.
     """
     # Check for deprecated options.
     if constraint == "inline":  # pragma: no cover
         reflow_logger.warning(
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/reflow/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return self.lint_results
 
     def get_raw(self) -> str:
         """Get the current raw representation."""
         return "".join(elem.raw for elem in self.elements)
 
     @staticmethod
-    def _validate_reflow_sequence(elements: ReflowSequenceType):
+    def _validate_reflow_sequence(elements: ReflowSequenceType) -> None:
         # An empty set of elements _is_ allowed as an edge case.
         if not elements:
             # Return early if so
             return None
         # Check odds and evens
         OddType = elements[0].__class__
         EvenType = ReflowPoint if OddType is ReflowBlock else ReflowBlock
@@ -116,14 +116,15 @@
             assert all(
                 isinstance(elem, OddType) for elem in elements[::2]
             ), f"Not all odd elements are {OddType.__name__}"
             # Check evens are all blocks
             assert all(
                 isinstance(elem, EvenType) for elem in elements[1::2]
             ), f"Not all even elements are {EvenType.__name__}"
+            return None
         except AssertionError as err:  # pragma: no cover
             for elem in elements:
                 reflow_logger.error("   - %s", elem)
             reflow_logger.exception("Assertion check on ReflowSequence failed.")
             raise err
 
     @staticmethod
@@ -558,15 +559,15 @@
             elements=elem_buff,
             root_segment=self.root_segment,
             reflow_config=self.reflow_config,
             depth_map=self.depth_map,
             lint_results=lint_results,
         )
 
-    def reindent(self):
+    def reindent(self) -> "ReflowSequence":
         """Reindent lines within a sequence."""
         if self.lint_results:
             raise NotImplementedError(  # pragma: no cover
                 "rebreak cannot currently handle pre-existing embodied fixes."
             )
 
         single_indent = construct_single_indent(
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/testing/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Testing utils for working with the CLIs."""
-from click.testing import CliRunner
+from click.testing import CliRunner, Result
+from typing import Optional, List, Dict, Any
 
 
 def invoke_assert_code(
-    ret_code=0,
-    args=None,
-    kwargs=None,
-    cli_input=None,
-    mix_stderr=True,
-    output_contains="",
-):
+    ret_code: int = 0,
+    args: Optional[List[Any]] = None,
+    kwargs: Optional[Dict[str, Any]] = None,
+    cli_input: Optional[str] = None,
+    mix_stderr: bool = True,
+    output_contains: str = "",
+) -> Result:
     """Invoke a command and check return code."""
     args = args or []
     kwargs = kwargs or {}
     if cli_input:
         kwargs["input"] = cli_input
     runner = CliRunner(mix_stderr=mix_stderr)
     result = runner.invoke(*args, **kwargs)
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.2.0/src/sqlfluff/utils/testing/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Testing utils for rule plugins."""
 from sqlfluff.core import Linter
 from sqlfluff.core.errors import SQLParseError, SQLTemplaterError
-from sqlfluff.core.rules import get_ruleset
+from sqlfluff.core.rules import BaseRule, get_ruleset
 from sqlfluff.core.config import FluffConfig
 from typing import Tuple, List, NamedTuple, Optional, Set
 from glob import glob
 
 import pytest
 import yaml
 
@@ -46,15 +46,15 @@
                     y[i].update({"configs": global_config})
         ids.extend([rule + "_" + t for t in y])
         test_cases.extend([RuleTestCase(rule=rule, **v) for k, v in y.items()])
 
     return ids, test_cases
 
 
-def get_rule_from_set(code, config):
+def get_rule_from_set(code, config) -> BaseRule:
     """Fetch a rule from the rule set."""
     for r in get_ruleset().get_rulepack(config=config).rules:
         if r.code == code:  # pragma: no cover
             return r
     raise ValueError(f"{code!r} not in {get_ruleset()!r}")
 
 
@@ -76,14 +76,15 @@
             pytest.fail(f"Linter failed with {e.desc()}")  # pragma: no cover
     parse_errors = list(
         filter(lambda v: isinstance(v, (SQLParseError, SQLTemplaterError)), lerrs)
     )
     if parse_errors:
         pytest.fail(f"Found the following parse errors in test case: {parse_errors}")
     if not any(v.rule.code == code for v in lerrs):
+        assert linted.tree
         print(f"Parsed File:\n{linted.tree.stringify()}")
         pytest.fail(
             f"No {code} failures found in query which should fail.",
             pytrace=False,
         )
     if line_numbers:
         actual_line_numbers = [e.line_no for e in lerrs]
@@ -113,15 +114,17 @@
 
     # This section is mainly for aid in debugging.
     rendered = linter.render_string(sql, fname="<STR>", config=cfg, encoding="utf-8")
     parsed = linter.parse_rendered(rendered, recurse=True)
     if parsed.violations:
         if msg:
             print(msg)  # pragma: no cover
+        assert parsed.tree
         pytest.fail(parsed.violations[0].desc() + "\n" + parsed.tree.stringify())
+    assert parsed.tree
     print(f"Parsed:\n {parsed.tree.stringify()}")
 
     # Note that lint_string() runs the templater and parser again, in order to
     # test the whole linting pipeline in the same way that users do. In other
     # words, the "rendered" and "parsed" variables above are irrelevant to this
     # line of code.
     lint_result = linter.lint_string(sql, config=cfg, fname="<STR>")
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.2.0/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.4
+Version: 2.2.0
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.2.0/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 src/sqlfluff/core/dialects/common.py
 src/sqlfluff/core/linter/__init__.py
 src/sqlfluff/core/linter/common.py
 src/sqlfluff/core/linter/linted_dir.py
 src/sqlfluff/core/linter/linted_file.py
 src/sqlfluff/core/linter/linter.py
 src/sqlfluff/core/linter/linting_result.py
+src/sqlfluff/core/linter/noqa.py
 src/sqlfluff/core/linter/runner.py
 src/sqlfluff/core/parser/__init__.py
 src/sqlfluff/core/parser/context.py
 src/sqlfluff/core/parser/helpers.py
 src/sqlfluff/core/parser/lexer.py
 src/sqlfluff/core/parser/markers.py
 src/sqlfluff/core/parser/match_logging.py
@@ -59,14 +60,15 @@
 src/sqlfluff/core/parser/grammar/anyof.py
 src/sqlfluff/core/parser/grammar/base.py
 src/sqlfluff/core/parser/grammar/conditional.py
 src/sqlfluff/core/parser/grammar/delimited.py
 src/sqlfluff/core/parser/grammar/greedy.py
 src/sqlfluff/core/parser/grammar/noncode.py
 src/sqlfluff/core/parser/grammar/sequence.py
+src/sqlfluff/core/parser/grammar/types.py
 src/sqlfluff/core/parser/segments/__init__.py
 src/sqlfluff/core/parser/segments/base.py
 src/sqlfluff/core/parser/segments/ephemeral.py
 src/sqlfluff/core/parser/segments/generator.py
 src/sqlfluff/core/parser/segments/meta.py
 src/sqlfluff/core/parser/segments/raw.py
 src/sqlfluff/core/plugin/__init__.py
```

### Comparing `sqlfluff-2.1.4/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.2.0/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.4/test/test_testing.py` & `sqlfluff-2.2.0/test/test_testing.py`

 * *Files identical despite different names*

