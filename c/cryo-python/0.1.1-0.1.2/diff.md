# Comparing `tmp/cryo_python-0.1.1.tar.gz` & `tmp/cryo_python-0.1.2.tar.gz`

## Comparing `cryo_python-0.1.1.tar` & `cryo_python-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/Cargo.toml
--rw-r--r--   0      502       20     8308 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/args.rs
--rw-r--r--   0      502       20      456 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/lib.rs
--rw-r--r--   0      502       20      380 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/main.rs
--rw-r--r--   0      502       20      509 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/args.rs
--rw-r--r--   0      502       20     7031 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/blocks.rs
--rw-r--r--   0      502       20     4845 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/file_output.rs
--rw-r--r--   0      502       20      156 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/mod.rs
--rw-r--r--   0      502       20     5425 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/query.rs
--rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/source.rs
--rw-r--r--   0      502       20     1281 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/run.rs
--rw-r--r--   0      502       20     6307 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_cli/src/summaries.rs
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/Cargo.toml
--rw-r--r--   0      502       20      646 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/collect.rs
--rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs
--rw-r--r--   0      502       20    15170 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks.rs
--rw-r--r--   0      502       20     2834 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs
--rw-r--r--   0      502       20     1541 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs
--rw-r--r--   0      502       20     8279 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/logs.rs
--rw-r--r--   0      502       20      184 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/mod.rs
--rw-r--r--   0      502       20     1546 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs
--rw-r--r--   0      502       20    20155 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs
--rw-r--r--   0      502       20     1618 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs
--rw-r--r--   0      502       20    20921 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/traces.rs
--rw-r--r--   0      502       20     2510 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/transactions.rs
--rw-r--r--   0      502       20     7794 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs
--rw-r--r--   0      502       20     5620 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/freeze.rs
--rw-r--r--   0      502       20      428 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/lib.rs
--rw-r--r--   0      502       20     1192 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs
--rw-r--r--   0      502       20     1222 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs
--rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs
--rw-r--r--   0      502       20      260 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/mod.rs
--rw-r--r--   0      502       20     3216 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs
--rw-r--r--   0      502       20     1809 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs
--rw-r--r--   0      502       20     1516 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/conversions.rs
--rw-r--r--   0      502       20      770 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs
--rw-r--r--   0      502       20     2755 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/export.rs
--rw-r--r--   0      502       20      117 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/mod.rs
--rw-r--r--   0      502       20      505 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/sort.rs
--rw-r--r--   0      502       20       61 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/mod.rs
--rw-r--r--   0      502       20     3609 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs
--rw-r--r--   0      502       20     4013 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs
--rw-r--r--   0      502       20     2584 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/errors.rs
--rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/files.rs
--rw-r--r--   0      502       20     1113 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/mod.rs
--rw-r--r--   0      502       20     1583 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/queries.rs
--rw-r--r--   0      502       20     4713 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/schemas.rs
--rw-r--r--   0      502       20     3611 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/sources.rs
--rw-r--r--   0      502       20     2002 2023-07-29 00:55:34.000000 cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/summaries.rs
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 cryo_python-0.1.1/Cargo.toml
--rw-r--r--   0      502       20     3124 2023-07-29 00:55:34.000000 cryo_python-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0      502       20      685 2023-07-29 00:55:34.000000 cryo_python-0.1.1/.gitignore
--rw-r--r--   0      502       20       71 2023-07-31 06:19:43.000000 cryo_python-0.1.1/build.rs
--rw-r--r--   0      502       20      518 2023-07-29 00:55:34.000000 cryo_python-0.1.1/pyproject.toml
--rw-r--r--   0      502       20      171 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/__init__.py
--rw-r--r--   0      502       20     1034 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_args.py
--rw-r--r--   0      502       20     1461 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_collect.py
--rw-r--r--   0      502       20     1002 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_freeze.py
--rw-r--r--   0      502       20     1592 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python/cryo/_spec.py
--rw-r--r--   0      502       20      180 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_chunks.py
--rw-r--r--   0      502       20      189 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_columns.py
--rw-r--r--   0      502       20     1190 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_datatypes.py
--rw-r--r--   0      502       20     1433 2023-07-29 00:55:34.000000 cryo_python-0.1.1/python_tests/test_output_formats.py
--rw-r--r--   0      502       20     3336 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/collect_adapter.rs
--rw-r--r--   0      502       20     3820 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/freeze_adapter.rs
--rw-r--r--   0      502       20      594 2023-07-29 00:55:34.000000 cryo_python-0.1.1/src/lib.rs
--rw-r--r--   0      502       20   121447 2023-07-31 21:49:21.000000 cryo_python-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 cryo_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/Cargo.toml
+-rw-r--r--   0      502       20     8435 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/args.rs
+-rw-r--r--   0      502       20      456 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/lib.rs
+-rw-r--r--   0      502       20      380 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/main.rs
+-rw-r--r--   0      502       20      509 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/args.rs
+-rw-r--r--   0      502       20     7031 2023-08-04 17:03:33.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/blocks.rs
+-rw-r--r--   0      502       20     4845 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/file_output.rs
+-rw-r--r--   0      502       20      156 2023-08-04 17:03:33.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/mod.rs
+-rw-r--r--   0      502       20     5425 2023-08-04 17:03:33.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/query.rs
+-rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/source.rs
+-rw-r--r--   0      502       20     1511 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/run.rs
+-rw-r--r--   0      502       20     6307 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_cli/src/summaries.rs
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/Cargo.toml
+-rw-r--r--   0      502       20      646 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/collect.rs
+-rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs
+-rw-r--r--   0      502       20    16086 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/blocks.rs
+-rw-r--r--   0      502       20     5250 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/blocks_and_transactions.rs
+-rw-r--r--   0      502       20     1541 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs
+-rw-r--r--   0      502       20     8279 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/logs.rs
+-rw-r--r--   0      502       20      184 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/mod.rs
+-rw-r--r--   0      502       20     1546 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs
+-rw-r--r--   0      502       20    20220 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs
+-rw-r--r--   0      502       20     1618 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs
+-rw-r--r--   0      502       20    20929 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/traces.rs
+-rw-r--r--   0      502       20     2665 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/transactions.rs
+-rw-r--r--   0      502       20     7794 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs
+-rw-r--r--   0      502       20     5620 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/freeze.rs
+-rw-r--r--   0      502       20      428 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/lib.rs
+-rw-r--r--   0      502       20     1192 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs
+-rw-r--r--   0      502       20     1222 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs
+-rw-r--r--   0      502       20     1999 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs
+-rw-r--r--   0      502       20      260 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/mod.rs
+-rw-r--r--   0      502       20     3216 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs
+-rw-r--r--   0      502       20     1809 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs
+-rw-r--r--   0      502       20     1516 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/conversions.rs
+-rw-r--r--   0      502       20      770 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs
+-rw-r--r--   0      502       20     2755 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/export.rs
+-rw-r--r--   0      502       20      117 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/mod.rs
+-rw-r--r--   0      502       20      505 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/sort.rs
+-rw-r--r--   0      502       20       61 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/datatypes/mod.rs
+-rw-r--r--   0      502       20     3609 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs
+-rw-r--r--   0      502       20     4013 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs
+-rw-r--r--   0      502       20     2760 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/errors.rs
+-rw-r--r--   0      502       20     1556 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/files.rs
+-rw-r--r--   0      502       20     1113 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/mod.rs
+-rw-r--r--   0      502       20     1583 2023-07-29 00:55:34.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/queries.rs
+-rw-r--r--   0      502       20     5218 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/schemas.rs
+-rw-r--r--   0      502       20     3611 2023-08-01 07:00:14.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/sources.rs
+-rw-r--r--   0      502       20     1962 2023-08-04 17:03:38.000000 cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/summaries.rs
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 cryo_python-0.1.2/Cargo.toml
+-rw-r--r--   0      502       20     3124 2023-07-29 00:55:34.000000 cryo_python-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0      502       20      685 2023-07-29 00:55:34.000000 cryo_python-0.1.2/.gitignore
+-rw-r--r--   0      502       20       71 2023-07-31 06:19:43.000000 cryo_python-0.1.2/build.rs
+-rw-r--r--   0      502       20      518 2023-07-29 00:55:34.000000 cryo_python-0.1.2/pyproject.toml
+-rw-r--r--   0      502       20      191 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python/cryo/__init__.py
+-rw-r--r--   0      502       20     1100 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python/cryo/_args.py
+-rw-r--r--   0      502       20     1950 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python/cryo/_collect.py
+-rw-r--r--   0      502       20     1385 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python/cryo/_freeze.py
+-rw-r--r--   0      502       20     1617 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python/cryo/_spec.py
+-rw-r--r--   0      502       20      180 2023-07-29 00:55:34.000000 cryo_python-0.1.2/python_tests/test_chunks.py
+-rw-r--r--   0      502       20      189 2023-07-29 00:55:34.000000 cryo_python-0.1.2/python_tests/test_columns.py
+-rw-r--r--   0      502       20     1190 2023-07-29 00:55:34.000000 cryo_python-0.1.2/python_tests/test_datatypes.py
+-rw-r--r--   0      502       20     1425 2023-08-04 17:03:38.000000 cryo_python-0.1.2/python_tests/test_output_formats.py
+-rw-r--r--   0      502       20     3406 2023-08-04 17:03:38.000000 cryo_python-0.1.2/src/collect_adapter.rs
+-rw-r--r--   0      502       20     3834 2023-08-04 17:03:38.000000 cryo_python-0.1.2/src/freeze_adapter.rs
+-rw-r--r--   0      502       20      594 2023-07-29 00:55:34.000000 cryo_python-0.1.2/src/lib.rs
+-rw-r--r--   0      502       20   121447 2023-08-04 17:03:38.000000 cryo_python-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 cryo_python-0.1.2/PKG-INFO
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/Cargo.toml` & `cryo_python-0.1.2/local_dependencies/cryo_cli/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/args.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/args.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
     /// Block numbers, see syntax below
     #[arg(
         short,
         long,
         default_value = "0:latest",
         allow_hyphen_values(true),
-        help_heading = "Content Options"
+        help_heading = "Content Options",
+        num_args = 1..
     )]
     pub blocks: Vec<String>,
 
     /// Align block chunk boundaries to regular intervals,
     /// e.g. (1000, 2000, 3000) instead of (1106, 2106, 3106)
     #[arg(short, long, help_heading = "Content Options", verbatim_doc_comment)]
     pub align: bool,
@@ -85,14 +86,18 @@
     #[arg(long, value_name = "M", help_heading = "Acquisition Options")]
     pub max_concurrent_chunks: Option<u64>,
 
     /// Dry run, collect no data
     #[arg(short, long, help_heading = "Acquisition Options")]
     pub dry: bool,
 
+    /// Run quietly without printing information to stdout
+    #[arg(long)]
+    pub no_verbose: bool,
+
     /// Number of blocks per file
     #[arg(short, long, default_value_t = 1000, help_heading = "Output Options")]
     pub chunk_size: u64,
 
     /// Number of files (alternative to --chunk-size)
     #[arg(long, help_heading = "Output Options")]
     pub n_chunks: Option<u64>,
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/blocks.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/blocks.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/file_output.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/file_output.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/query.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/query.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/parse/source.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/parse/source.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/run.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/run.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 use std::time::SystemTime;
 
 use crate::{args, parse, summaries};
 use cryo_freeze::{FreezeError, FreezeSummary};
 
 /// run freeze for given Args
 pub async fn run(args: args::Args) -> Result<Option<FreezeSummary>, FreezeError> {
+    // parse inputs
     let t_start = SystemTime::now();
     let (query, source, sink) = match parse::parse_opts(&args).await {
         Ok(opts) => opts,
         Err(e) => return Err(e.into()),
     };
     let t_parse_done = SystemTime::now();
-    summaries::print_cryo_summary(&query, &source, &sink);
-    let summary = if args.dry {
-        println!("\n\n[dry run, exiting]");
-        None
-    } else {
+
+    // print summary
+    if !args.no_verbose {
+        summaries::print_cryo_summary(&query, &source, &sink);
+    }
+
+    // check dry run
+    if args.dry {
+        if !args.no_verbose {
+            println!("\n\n[dry run, exiting]");
+        }
+        return Ok(None)
+    };
+
+    // collect data
+    if !args.no_verbose {
         summaries::print_header("\n\ncollecting data");
-        match cryo_freeze::freeze(&query, &source, &sink).await {
-            Ok(freeze_summary) => {
-                let t_data_done = SystemTime::now();
+    }
+    match cryo_freeze::freeze(&query, &source, &sink).await {
+        Ok(freeze_summary) => {
+            // print summary
+            let t_data_done = SystemTime::now();
+            if !args.no_verbose {
                 println!("...done\n\n");
                 summaries::print_cryo_conclusion(
                     t_start,
                     t_parse_done,
                     t_data_done,
                     &query,
                     &freeze_summary,
-                );
-                Some(freeze_summary)
-            }
-            Err(e) => {
-                println!("{}", e);
-                return Err(e)
+                )
             }
+
+            // return summary
+            Ok(Some(freeze_summary))
         }
-    };
-    Ok(summary)
+
+        Err(e) => {
+            println!("{}", e);
+            Err(e)
+        }
+    }
 }
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_cli/src/summaries.rs` & `cryo_python-0.1.2/local_dependencies/cryo_cli/src/summaries.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/Cargo.toml` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/collect.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/collect.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/balance_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/blocks.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/blocks.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     types::{
         conversions::{ToVecHex, ToVecU8},
         BlockChunk, Blocks, CollectError, ColumnType, Dataset, Datatype, RowFilter, Source, Table,
     },
     with_series, with_series_binary,
 };
 
+pub(crate) type BlockTxGasTuple<TX> = Result<(Block<TX>, Option<Vec<u32>>), CollectError>;
+
 #[async_trait::async_trait]
 impl Dataset for Blocks {
     fn datatype(&self) -> Datatype {
         Datatype::Blocks
     }
 
     fn name(&self) -> &'static str {
@@ -68,15 +70,15 @@
         }
     }
 }
 
 async fn fetch_blocks(
     block_chunk: &BlockChunk,
     source: &Source,
-) -> mpsc::Receiver<Result<Option<Block<TxHash>>, CollectError>> {
+) -> mpsc::Receiver<BlockTxGasTuple<TxHash>> {
     let (tx, rx) = mpsc::channel(block_chunk.numbers().len());
 
     for number in block_chunk.numbers() {
         let tx = tx.clone();
         let provider = Arc::clone(&source.provider);
         let semaphore = source.semaphore.clone();
         let rate_limiter = source.rate_limiter.as_ref().map(Arc::clone);
@@ -84,45 +86,50 @@
             let _permit = match semaphore {
                 Some(semaphore) => Some(Arc::clone(&semaphore).acquire_owned().await),
                 _ => None,
             };
             if let Some(limiter) = rate_limiter {
                 Arc::clone(&limiter).until_ready().await;
             }
-            let block = provider.get_block(number).await.map_err(CollectError::ProviderError);
-            match tx.send(block).await {
+            let block = provider.get_block(number).await;
+            let result = match block {
+                Ok(Some(block)) => Ok((block, None)),
+                Ok(None) => Err(CollectError::CollectError("block not in node".to_string())),
+                Err(e) => Err(CollectError::ProviderError(e)),
+            };
+            match tx.send(result).await {
                 Ok(_) => {}
                 Err(tokio::sync::mpsc::error::SendError(_e)) => {
                     eprintln!("send error, try using a rate limit with --requests-per-second or limiting max concurrency with --max-concurrent-requests");
                     std::process::exit(1)
                 }
             }
         });
     }
     rx
 }
 
 pub(crate) trait ProcessTransactions {
-    fn process(&self, schema: &Table, columns: &mut TransactionColumns);
+    fn process(&self, schema: &Table, columns: &mut TransactionColumns, gas_used: Option<u32>);
 }
 
 impl ProcessTransactions for TxHash {
-    fn process(&self, _schema: &Table, _columns: &mut TransactionColumns) {
+    fn process(&self, _schema: &Table, _columns: &mut TransactionColumns, _gas_used: Option<u32>) {
         panic!("transaction data not available to process")
     }
 }
 
 impl ProcessTransactions for Transaction {
-    fn process(&self, schema: &Table, columns: &mut TransactionColumns) {
-        process_transaction(self, schema, columns)
+    fn process(&self, schema: &Table, columns: &mut TransactionColumns, gas_used: Option<u32>) {
+        process_transaction(self, schema, columns, gas_used)
     }
 }
 
 pub(crate) async fn blocks_to_dfs<TX: ProcessTransactions>(
-    mut blocks: mpsc::Receiver<Result<Option<Block<TX>>, CollectError>>,
+    mut blocks: mpsc::Receiver<BlockTxGasTuple<TX>>,
     blocks_schema: &Option<&Table>,
     transactions_schema: &Option<&Table>,
     chain_id: u64,
 ) -> Result<(Option<DataFrame>, Option<DataFrame>), CollectError> {
     // initialize
     let mut block_columns =
         if blocks_schema.is_none() { BlockColumns::new(0) } else { BlockColumns::new(100) };
@@ -133,35 +140,40 @@
     };
 
     // parse stream of blocks
     let mut n_blocks = 0;
     let mut n_txs = 0;
     while let Some(message) = blocks.recv().await {
         match message {
-            Ok(Some(block)) => {
+            Ok((block, gas_used)) => {
                 n_blocks += 1;
                 if let Some(schema) = blocks_schema {
                     process_block(&block, schema, &mut block_columns)
                 }
                 if let Some(schema) = transactions_schema {
-                    for tx in block.transactions.iter() {
-                        n_txs += 1;
-                        tx.process(schema, &mut transaction_columns)
+                    match gas_used {
+                        Some(gas_used) => {
+                            for (tx, gas_used) in block.transactions.iter().zip(gas_used) {
+                                n_txs += 1;
+                                tx.process(schema, &mut transaction_columns, Some(gas_used))
+                            }
+                        }
+                        None => {
+                            for tx in block.transactions.iter() {
+                                n_txs += 1;
+                                tx.process(schema, &mut transaction_columns, None)
+                            }
+                        }
                     }
                 }
             }
-            // _ => return Err(CollectError::TooManyRequestsError),
             Err(e) => {
                 println!("{:?}", e);
                 return Err(CollectError::TooManyRequestsError)
             }
-            Ok(None) => {
-                println!("NONE");
-                return Err(CollectError::TooManyRequestsError)
-            }
         }
     }
 
     // convert to dataframes
     let blocks_df = match blocks_schema {
         Some(schema) => Some(block_columns.create_df(schema, chain_id, n_blocks)?),
         None => None,
@@ -246,14 +258,15 @@
     transaction_hash: Vec<Vec<u8>>,
     nonce: Vec<u64>,
     from_address: Vec<Vec<u8>>,
     to_address: Vec<Option<Vec<u8>>>,
     value: Vec<String>,
     input: Vec<Vec<u8>>,
     gas_limit: Vec<u32>,
+    gas_used: Vec<u32>,
     gas_price: Vec<Option<u64>>,
     transaction_type: Vec<Option<u32>>,
     max_priority_fee_per_gas: Vec<Option<u64>>,
     max_fee_per_gas: Vec<Option<u64>>,
 }
 
 impl TransactionColumns {
@@ -264,14 +277,15 @@
             transaction_hash: Vec::with_capacity(n),
             nonce: Vec::with_capacity(n),
             from_address: Vec::with_capacity(n),
             to_address: Vec::with_capacity(n),
             value: Vec::with_capacity(n),
             input: Vec::with_capacity(n),
             gas_limit: Vec::with_capacity(n),
+            gas_used: Vec::with_capacity(n),
             gas_price: Vec::with_capacity(n),
             transaction_type: Vec::with_capacity(n),
             max_priority_fee_per_gas: Vec::with_capacity(n),
             max_fee_per_gas: Vec::with_capacity(n),
         }
     }
 
@@ -287,14 +301,15 @@
         with_series_binary!(cols, "transaction_hash", self.transaction_hash, schema);
         with_series!(cols, "nonce", self.nonce, schema);
         with_series_binary!(cols, "from_address", self.from_address, schema);
         with_series_binary!(cols, "to_address", self.to_address, schema);
         with_series!(cols, "value", self.value, schema);
         with_series_binary!(cols, "input", self.input, schema);
         with_series!(cols, "gas_limit", self.gas_limit, schema);
+        with_series!(cols, "gas_used", self.gas_used, schema);
         with_series!(cols, "gas_price", self.gas_price, schema);
         with_series!(cols, "transaction_type", self.transaction_type, schema);
         with_series!(cols, "max_priority_fee_per_gas", self.max_priority_fee_per_gas, schema);
         with_series!(cols, "max_fee_per_gas", self.max_fee_per_gas, schema);
 
         if schema.has_column("chain_id") {
             cols.push(Series::new("chain_id", vec![chain_id; n_rows]));
@@ -354,15 +369,20 @@
         columns.size.push(block.size.map(|x| x.as_u32()));
     }
     if schema.has_column("base_fee_per_gas") {
         columns.base_fee_per_gas.push(block.base_fee_per_gas.map(|value| value.as_u64()));
     }
 }
 
-fn process_transaction(tx: &Transaction, schema: &Table, columns: &mut TransactionColumns) {
+fn process_transaction(
+    tx: &Transaction,
+    schema: &Table,
+    columns: &mut TransactionColumns,
+    gas_used: Option<u32>,
+) {
     if schema.has_column("block_number") {
         match tx.block_number {
             Some(block_number) => columns.block_number.push(Some(block_number.as_u64())),
             None => columns.block_number.push(None),
         }
     }
     if schema.has_column("transaction_index") {
@@ -393,14 +413,17 @@
     }
     if schema.has_column("input") {
         columns.input.push(tx.input.to_vec());
     }
     if schema.has_column("gas_limit") {
         columns.gas_limit.push(tx.gas.as_u32());
     }
+    if schema.has_column("gas_used") {
+        columns.gas_used.push(gas_used.unwrap())
+    }
     if schema.has_column("gas_price") {
         columns.gas_price.push(tx.gas_price.map(|gas_price| gas_price.as_u64()));
     }
     if schema.has_column("transaction_type") {
         columns.transaction_type.push(tx.transaction_type.map(|value| value.as_u32()));
     }
     if schema.has_column("max_priority_fee_per_gas") {
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/code_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/logs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/logs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/nonce_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/state_diffs.rs`

 * *Files 5% similar despite different names*

```diff
@@ -182,15 +182,16 @@
     let mut code_from_value: Vec<Vec<u8>> = Vec::with_capacity(capacity);
     let mut code_to_value: Vec<Vec<u8>> = Vec::with_capacity(capacity);
 
     let mut n_rows = 0;
     while let Some(message) = rx.recv().await {
         match message {
             (block_num, Ok(blocks_traces)) => {
-                for ts in blocks_traces.iter() {
+                for (t_index, ts) in blocks_traces.iter().enumerate() {
+                    let t_index = t_index as u32;
                     if let (Some(tx), Some(StateDiff(state_diff))) =
                         (ts.transaction_hash, &ts.state_diff)
                     {
                         for (addr, addr_diff) in state_diff.iter() {
                             n_rows += n_rows;
 
                             // storage
@@ -202,15 +203,15 @@
                                         Diff::Died(value) => (*value, H256::zero()),
                                         Diff::Changed(ChangedType { from, to }) => (*from, *to),
                                     };
                                     if include_storage_block_number {
                                         storage_block_number.push(block_num);
                                     };
                                     if include_storage_transaction_index {
-                                        storage_transaction_index.push(block_num);
+                                        storage_transaction_index.push(t_index);
                                     };
                                     if include_storage_transaction_hash {
                                         storage_transaction_hash.push(tx.as_bytes().to_vec());
                                     };
                                     if include_storage_address {
                                         storage_address.push(addr.as_bytes().to_vec());
                                     };
@@ -236,15 +237,15 @@
                                         (from.to_string(), to.to_string())
                                     }
                                 };
                                 if include_balance_block_number {
                                     balance_block_number.push(block_num);
                                 };
                                 if include_balance_transaction_index {
-                                    balance_transaction_index.push(block_num);
+                                    balance_transaction_index.push(t_index);
                                 };
                                 if include_balance_transaction_hash {
                                     balance_transaction_hash.push(tx.as_bytes().to_vec());
                                 };
                                 if include_balance_address {
                                     balance_address.push(addr.as_bytes().to_vec());
                                 };
@@ -266,15 +267,15 @@
                                         (from.as_u64(), to.as_u64())
                                     }
                                 };
                                 if include_nonce_block_number {
                                     nonce_block_number.push(block_num);
                                 };
                                 if include_nonce_transaction_index {
-                                    nonce_transaction_index.push(block_num);
+                                    nonce_transaction_index.push(t_index);
                                 };
                                 if include_nonce_transaction_hash {
                                     nonce_transaction_hash.push(tx.as_bytes().to_vec());
                                 };
                                 if include_nonce_address {
                                     nonce_address.push(addr.as_bytes().to_vec());
                                 };
@@ -303,15 +304,15 @@
                                         (from.to_vec(), to.to_vec())
                                     }
                                 };
                                 if include_code_block_number {
                                     code_block_number.push(block_num);
                                 };
                                 if include_code_transaction_index {
-                                    code_transaction_index.push(block_num);
+                                    code_transaction_index.push(t_index);
                                 };
                                 if include_code_transaction_hash {
                                     code_transaction_hash.push(tx.as_bytes().to_vec());
                                 };
                                 if include_code_address {
                                     code_address.push(addr.as_bytes().to_vec());
                                 };
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/storage_diffs.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/traces.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/traces.rs`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,15 @@
                         }
                         if include_error {
                             error.push(trace.error.clone());
                         }
                     }
                 }
             }
-            _ => return Err(CollectError::TooManyRequestsError),
+            Err(e) => return Err(CollectError::RPCError(e.to_string())),
         }
     }
 
     let mut cols = Vec::new();
 
     with_series_binary!(cols, "action_from", action_from, schema);
     with_series_binary!(cols, "action_to", action_to, schema);
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/transactions.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/transactions.rs`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             ("from_address", ColumnType::Binary),
             ("to_address", ColumnType::Binary),
             ("value", ColumnType::Decimal128),
             ("value_str", ColumnType::String),
             ("value_float", ColumnType::Float64),
             ("input", ColumnType::Binary),
             ("gas_limit", ColumnType::UInt32),
+            ("gas_used", ColumnType::UInt32),
             ("gas_price", ColumnType::UInt64),
             ("transaction_type", ColumnType::UInt32),
             ("max_priority_fee_per_gas", ColumnType::UInt64),
             ("max_fee_per_gas", ColumnType::UInt64),
             ("chain_id", ColumnType::UInt64),
         ])
     }
@@ -64,15 +65,18 @@
     async fn collect_block_chunk(
         &self,
         chunk: &BlockChunk,
         source: &Source,
         schema: &Table,
         _filter: Option<&RowFilter>,
     ) -> Result<DataFrame, CollectError> {
-        let rx = blocks_and_transactions::fetch_blocks_and_transactions(chunk, source).await;
+        let include_gas_used = schema.has_column("gas_used");
+        let rx =
+            blocks_and_transactions::fetch_blocks_and_transactions(chunk, source, include_gas_used)
+                .await;
         let output = blocks::blocks_to_dfs(rx, &None, &Some(schema), source.chain_id).await;
         match output {
             Ok((_, Some(txs_df))) => Ok(txs_df),
             Ok((_, _)) => Err(CollectError::BadSchemaError),
             Err(e) => Err(e),
         }
     }
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/datasets/vm_traces.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/freeze.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/freeze.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/binary_chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/chunk_ops.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/number_chunk.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/chunks/subchunks.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/conversions.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/conversions.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/creation.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/dataframes/export.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/dataframes/export.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/datatypes/multi.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/datatypes/scalar.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/errors.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/errors.rs`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     #[error("Parsing error")]
     ParseError(#[from] ParseError),
 }
 
 /// Error related to data collection
 #[derive(Error, Debug)]
 pub enum CollectError {
+    /// General Collection error
+    #[error("Collect failed: {0}")]
+    CollectError(String),
+
     /// Error related to provider operations
     #[error("Failed to get block: {0}")]
     ProviderError(#[source] ProviderError),
 
     /// Error related to tokio task
     #[error("Task failed: {0}")]
     TaskFailed(#[source] tokio::task::JoinError),
@@ -49,14 +53,18 @@
     /// Error related to bad schema
     #[error("Bad schema specified")]
     BadSchemaError,
 
     /// Error related to too many requests
     #[error("try using a rate limit with --requests-per-second or limiting max concurrency with --max-concurrent-requests")]
     TooManyRequestsError,
+
+    /// Generic RPC Error
+    #[error("RPC call error")]
+    RPCError(String),
 }
 
 /// Error related to parsing
 #[derive(Error, Debug)]
 pub enum ParseError {
     /// Error related to parsing
     #[error("Parsing error")]
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/files.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/files.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/mod.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/queries.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/queries.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/schemas.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/schemas.rs`

 * *Files 7% similar despite different names*

```diff
@@ -121,21 +121,32 @@
             datatype.dataset().column_types().keys().map(|k| k.to_string()).collect()
         }
         (Some(columns), _, _) => columns.iter().map(|x| x.to_string()).collect(),
         (_, Some(include), _) if ((include.len() == 1) & include.contains(&"all".to_string())) => {
             datatype.dataset().column_types().keys().map(|k| k.to_string()).collect()
         }
         (_, Some(include), Some(exclude)) => {
-            let include_set: HashSet<_> = include.iter().collect();
-            let exclude_set: HashSet<_> = exclude.iter().collect();
-            let intersection: HashSet<_> = include_set.intersection(&exclude_set).collect();
-            assert!(intersection.is_empty(), "include and exclude should be non-overlapping");
-            include.to_vec()
+            let mut result: Vec<String> = default_columns.iter().map(|s| s.to_string()).collect();
+            let mut result_set: HashSet<String> = result.iter().cloned().collect();
+            let exclude_set: HashSet<String> = exclude.iter().cloned().collect();
+            include
+                .iter()
+                .filter(|item| !exclude_set.contains(*item) && result_set.insert(item.to_string()))
+                .for_each(|item| result.push(item.clone()));
+            result
+        }
+        (_, Some(include), None) => {
+            let mut result: Vec<String> = default_columns.iter().map(|s| s.to_string()).collect();
+            let mut result_set: HashSet<String> = result.iter().cloned().collect();
+            include
+                .iter()
+                .filter(|item| result_set.insert(item.to_string()))
+                .for_each(|item| result.push(item.clone()));
+            result
         }
-        (_, Some(include), None) => include.to_vec(),
         (_, None, Some(exclude)) => {
             let exclude_set: HashSet<_> = exclude.iter().collect();
             default_columns
                 .into_iter()
                 .filter(|s| !exclude_set.contains(&s.to_string()))
                 .map(|s| s.to_string())
                 .collect()
```

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/sources.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/sources.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/local_dependencies/cryo_freeze/src/types/summaries.rs` & `cryo_python-0.1.2/local_dependencies/cryo_freeze/src/types/summaries.rs`

 * *Files 4% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 pub struct FreezeSummary {
     /// number of chunks completed successfully
     pub n_completed: u64,
     /// number of chunks skipped
     pub n_skipped: u64,
     /// number of chunks that encountered an error
     pub n_errored: u64,
-    /// paths_by_type
-    pub paths_by_type: HashMap<Datatype, Vec<String>>,
+    /// paths
+    pub paths: HashMap<Datatype, Vec<String>>,
 }
 
 pub(crate) trait FreezeSummaryAgg {
     fn aggregate(self) -> FreezeSummary;
 }
 
 impl FreezeSummaryAgg for Vec<FreezeChunkSummary> {
     fn aggregate(self) -> FreezeSummary {
         let mut n_completed: u64 = 0;
         let mut n_skipped: u64 = 0;
         let mut n_errored: u64 = 0;
 
-        let mut paths_by_type = HashMap::new();
+        let mut paths = HashMap::new();
         for chunk_summary in self {
             if chunk_summary.skipped {
                 n_skipped += 1;
             } else if chunk_summary.errored {
                 n_errored += 1;
             } else {
                 n_completed += 1;
             }
             for (datatype, path) in chunk_summary.paths {
-                paths_by_type.entry(datatype).or_insert_with(Vec::new).push(path);
+                paths.entry(datatype).or_insert_with(Vec::new).push(path);
             }
         }
 
-        FreezeSummary { n_completed, n_skipped, n_errored, paths_by_type }
+        FreezeSummary { n_completed, n_skipped, n_errored, paths }
     }
 }
 
 /// Summary of freezing a single chunk
 pub struct FreezeChunkSummary {
     /// whether chunk was skipped
     pub skipped: bool,
```

### Comparing `cryo_python-0.1.1/Cargo.toml` & `cryo_python-0.1.2/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cryo_python"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 build = "build.rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "cryo"
 crate-type = ["cdylib"]
```

### Comparing `cryo_python-0.1.1/.github/workflows/CI.yml` & `cryo_python-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/.gitignore` & `cryo_python-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/pyproject.toml` & `cryo_python-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/python/cryo/_args.py` & `cryo_python-0.1.2/python/cryo/_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from typing_extensions import Unpack
 
 
 def parse_cli_args(
     start_block: _spec.BlockReference | None = None,
     end_block: _spec.BlockReference | None = None,
     file_format: _spec.FileFormat = 'parquet',
+    verbose: bool = True,
     **kwargs: Unpack[_spec.CryoCliArgs],
 ) -> _spec.CryoCliArgs:
     """
     TODO: write this part in rust
     """
 
     if start_block is not None and end_block is not None:
@@ -32,9 +33,11 @@
     elif file_format == 'csv':
         kwargs['csv'] = True
     # elif file_format == 'avro':
     #     kwargs['avro'] = True
     else:
         raise Exception('unknown file_format')
 
+    kwargs['no_verbose'] = not verbose
+
     return kwargs
```

### Comparing `cryo_python-0.1.1/python/cryo/_collect.py` & `cryo_python-0.1.2/python/cryo/_collect.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,17 +19,24 @@
     **kwargs: Unpack[_spec.CryoCliArgs],
 ) -> pl.DataFrame | pd.DataFrame | ListOfDicts | DictOfLists:
     """asynchronously collect data and return as dataframe"""
 
     from . import _args
     from . import _cryo_rust  # type: ignore
 
+    # parse inputs
     cli_args = _args.parse_cli_args(**kwargs)
+
+    # fix chunk size
+    cli_args['chunk_size'] = 20_000_000
+
+    # collect data
     result: pl.DataFrame = await _cryo_rust._collect(datatype, **cli_args)
 
+    # format output
     if output_format == 'polars':
         return result
     elif output_format == 'pandas':
         return result.to_pandas()
     elif output_format == 'list':
         return result.to_dicts()
     elif output_format == 'dict':
@@ -43,11 +50,19 @@
     output_format: _spec.PythonOutput = 'polars',
     **kwargs: Unpack[_spec.CryoCliArgs],
 ) -> pl.DataFrame | pd.DataFrame | ListOfDicts | DictOfLists:
     """collect data and return as dataframe"""
 
     import asyncio
 
-    return asyncio.run(
-        async_collect(datatype, output_format=output_format, **kwargs)
-    )
+    coroutine = async_collect(datatype, output_format=output_format, **kwargs)
+
+    try:
+        import concurrent.futures
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            future = executor.submit(loop.run_until_complete, coroutine)  # type: ignore
+            return future.result()  # type: ignore
+    except RuntimeError:
+        return asyncio.run(coroutine)
```

### Comparing `cryo_python-0.1.1/python/cryo/_spec.py` & `cryo_python-0.1.2/python/cryo/_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,8 +49,9 @@
         compression: str | None
         contract: str | bytes | None
         topic0: str | bytes | None
         topic1: str | bytes | None
         topic2: str | bytes | None
         topic3: str | bytes | None
         inner_request_size: int | None
+        no_verbose: bool
```

### Comparing `cryo_python-0.1.1/python_tests/test_datatypes.py` & `cryo_python-0.1.2/python_tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/python_tests/test_output_formats.py` & `cryo_python-0.1.2/python_tests/test_output_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def test_file_output(query, format):
     extension, reader = format
     output_dir = tempfile.mkdtemp()
     if extension != 'parquet':
         query = dict(query, **{extension: True})
     result = cryo.freeze(output_dir=output_dir, **query)
     for datatype in query['datatype']:
-        path = result['paths_by_type'][datatype]
+        path = result['paths'][datatype]
         assert isinstance(path, list) and len(path) == 1
         path = path[0]
         df_freeze = reader(path)
         query_without_datatype = dict(query)
         del query_without_datatype['datatype']
         df_collect = cryo.collect(datatype, **query_without_datatype)
         assert df_freeze.frame_equal(df_collect)
```

### Comparing `cryo_python-0.1.1/src/collect_adapter.rs` & `cryo_python-0.1.2/src/collect_adapter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         compression = vec!["lz4".to_string()],
         contract = None,
         topic0 = None,
         topic1 = None,
         topic2 = None,
         topic3 = None,
         inner_request_size = 1,
+        no_verbose = false,
     )
 )]
 #[allow(clippy::too_many_arguments)]
 pub fn _collect(
     py: Python<'_>,
     datatype: String,
     blocks: Vec<String>,
@@ -73,14 +74,15 @@
     compression: Vec<String>,
     contract: Option<String>,
     topic0: Option<String>,
     topic1: Option<String>,
     topic2: Option<String>,
     topic3: Option<String>,
     inner_request_size: u64,
+    no_verbose: bool,
 ) -> PyResult<&PyAny> {
     let args = Args {
         datatype: vec![datatype],
         blocks,
         align,
         reorg_buffer,
         include_columns,
@@ -107,14 +109,15 @@
         compression,
         contract,
         topic0,
         topic1,
         topic2,
         topic3,
         inner_request_size,
+        no_verbose,
     };
 
     pyo3_asyncio::tokio::future_into_py(py, async move {
         match run_collect(args).await {
             // Ok(df) => Ok(Python::with_gil(|py| py.None())),
             Ok(df) => Ok(PyDataFrame(df)),
             Err(_e) => Err(PyErr::new::<PyTypeError, _>("failed")),
```

### Comparing `cryo_python-0.1.1/src/freeze_adapter.rs` & `cryo_python-0.1.2/src/freeze_adapter.rs`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         compression = vec!["lz4".to_string()],
         contract = None,
         topic0 = None,
         topic1 = None,
         topic2 = None,
         topic3 = None,
         inner_request_size = 1,
+        no_verbose = false,
     )
 )]
 #[allow(clippy::too_many_arguments)]
 pub fn _freeze(
     py: Python<'_>,
     datatype: Vec<String>,
     blocks: Vec<String>,
@@ -74,14 +75,15 @@
     compression: Vec<String>,
     contract: Option<String>,
     topic0: Option<String>,
     topic1: Option<String>,
     topic2: Option<String>,
     topic3: Option<String>,
     inner_request_size: u64,
+    no_verbose: bool,
 ) -> PyResult<&PyAny> {
     let args = Args {
         datatype,
         blocks,
         align,
         reorg_buffer,
         include_columns,
@@ -108,32 +110,33 @@
         compression,
         contract,
         topic0,
         topic1,
         topic2,
         topic3,
         inner_request_size,
+        no_verbose,
     };
 
     pyo3_asyncio::tokio::future_into_py(py, async move {
         match run(args).await {
             Ok(Some(result)) => Python::with_gil(|py| {
-                let paths_by_type = PyDict::new(py);
-                for (key, values) in &result.paths_by_type {
+                let paths = PyDict::new(py);
+                for (key, values) in &result.paths {
                     let key = key.dataset().name();
                     let values: Vec<&str> = values.iter().map(AsRef::as_ref).collect();
-                    paths_by_type.set_item(key, values).unwrap();
+                    paths.set_item(key, values).unwrap();
                 }
-                let paths_by_type = paths_by_type.to_object(py);
+                let paths = paths.to_object(py);
 
                 let dict = [
                     ("n_completed".to_string(), result.n_completed.into_py(py)),
                     ("n_skipped".to_string(), result.n_skipped.into_py(py)),
                     ("n_errored".to_string(), result.n_errored.into_py(py)),
-                    ("paths_by_type".to_string(), paths_by_type),
+                    ("paths".to_string(), paths),
                 ]
                 .into_py_dict(py);
                 Ok(dict.to_object(py))
             }),
             Ok(None) => Ok(Python::with_gil(|py| py.None())),
             _ => Err(PyErr::new::<PyTypeError, _>("failed")),
         }
```

### Comparing `cryo_python-0.1.1/src/lib.rs` & `cryo_python-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryo_python-0.1.1/Cargo.lock` & `cryo_python-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
  "prefix-hex",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "cryo_python"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "cryo_cli",
  "cryo_freeze",
  "polars",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config",
```

