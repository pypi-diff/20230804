# Comparing `tmp/chromadb-client-0.4.5.dev0.tar.gz` & `tmp/chromadb-client-0.4.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-client-0.4.5.dev0.tar", last modified: Tue Aug  1 01:21:00 2023, max compression
+gzip compressed data, was "chromadb-client-0.4.6.dev0.tar", last modified: Fri Aug  4 06:33:07 2023, max compression
```

## Comparing `chromadb-client-0.4.5.dev0.tar` & `chromadb-client-0.4.6.dev0.tar`

### file list

```diff
@@ -1,247 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.020581 chromadb-client-0.4.5.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.028582 chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.028582 chromadb-client-0.4.5.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/chroma-client-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/chroma-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/chroma-release-python-client.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.github/workflows/pr-review-checklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.028582 chromadb-client-0.4.5.dev0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-01 01:20:54.000000 chromadb-client-0.4.5.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/RELEASE_PROCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/integration-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/version
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/bin/windows_upgrade_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/api/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/api/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.032582 chromadb-client-0.4.5.dev0/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/db/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/impl/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/impl/sqlite_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/mixins/embeddings_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/mixins/sysdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/db/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)   368824 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/experimental/density_relevance.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 01:20:54.000000 chromadb-client-0.4.5.dev0/chromadb/is_thin_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/migrations/embeddings_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/migrations/metadb/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/metadb/00002-embedding-metadata.sqlite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/migrations/sysdb/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/sysdb/00001-collections.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/sysdb/00002-segments.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.024581 chromadb-client-0.4.5.dev0/chromadb/segment/impl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/segment/impl/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/manager/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/segment/impl/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/metadata/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/brute_force_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/hnsw_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/local_hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/local_persistent_hnsw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.036582 chromadb-client-0.4.5.dev0/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.040583 chromadb-client-0.4.5.dev0/chromadb/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/telemetry/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/telemetry/posthog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.040583 chromadb-client-0.4.5.dev0/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.040583 chromadb-client-0.4.5.dev0/chromadb/test/db/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.040583 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/db/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.040583 chromadb-client-0.4.5.dev0/chromadb/test/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/ingest/test_producer_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb/test/property/
--rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_cross_version_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/property/test_persist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb/test/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/segment/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/segment/test_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb/test/stress/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/stress/test_many_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/test_multithreaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/test/utils/test_messagid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/distance_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/messageid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/chromadb/utils/read_write_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.044583 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-01 01:20:59.000000 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-08-01 01:21:00.000000 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:20:59.000000 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 01:20:59.000000 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 01:20:59.000000 chromadb-client-0.4.5.dev0/chromadb_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.024581 chromadb-client-0.4.5.dev0/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.048583 chromadb-client-0.4.5.dev0/clients/js/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.024581 chromadb-client-0.4.5.dev0/clients/js/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.048583 chromadb-client-0.4.5.dev0/clients/js/examples/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/browser/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/browser/app.ts
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/browser/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/browser/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/browser/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.048583 chromadb-client-0.4.5.dev0/clients/js/examples/node/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/node/app.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/node/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/examples/node/yarn.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/genapi.sh
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/openapitools.json
--rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.048583 chromadb-client-0.4.5.dev0/clients/js/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/ChromaClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/Collection.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/clients/js/src/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/api.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/configuration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/models.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/generated/runtime.ts
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/types.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/src/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/clients/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/add.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/collection.client.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/delete.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/get.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/initClient.ts
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/peek.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/query.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/update.collection.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/test/upsert.collections.test.ts
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/tsconfig.module.json
--rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/js/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/clients/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/python/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/python/build_python_thin_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/python/integration-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/python/is_thin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/clients/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/docker-compose.server.example.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/docs/CIP_Chroma_Improvment_Proposals.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.052583 chromadb-client-0.4.5.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/examples/basic_functionality/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/basic_functionality/alternative_embeddings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/basic_functionality/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/basic_functionality/where_filtering.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.028582 chromadb-client-0.4.5.dev0/examples/deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/chroma.tf
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/main.tf
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/startup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.028582 chromadb-client-0.4.5.dev0/examples/use_with/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/examples/use_with/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/use_with/cohere/cohere_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/use_with/cohere/cohere_python.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/examples/use_with/cohere/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/log_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-01 01:20:54.000000 chromadb-client-0.4.5.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 01:20:40.000000 chromadb-client-0.4.5.dev0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 01:21:00.056584 chromadb-client-0.4.5.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.052833 chromadb-client-0.4.6.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.060834 chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.060834 chromadb-client-0.4.6.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/chroma-client-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/chroma-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/chroma-release-python-client.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.github/workflows/pr-review-checklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-04 06:33:01.000000 chromadb-client-0.4.6.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/RELEASE_PROCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/integration-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/version
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/bin/windows_upgrade_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/api/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.064833 chromadb-client-0.4.6.dev0/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/api/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/db/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/impl/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/impl/sqlite_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/mixins/embeddings_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/mixins/sysdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/db/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)   368700 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/experimental/density_relevance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 06:33:01.000000 chromadb-client-0.4.6.dev0/chromadb/is_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/migrations/embeddings_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/embeddings_queue/00001-embeddings.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/migrations/metadb/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/metadb/00002-embedding-metadata.sqlite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/migrations/sysdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/sysdb/00001-collections.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/sysdb/00002-segments.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/migrations/sysdb/00003-collection-dimension.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.056833 chromadb-client-0.4.6.dev0/chromadb/segment/impl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/segment/impl/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/manager/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/segment/impl/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/metadata/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/brute_force_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/hnsw_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/local_hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/local_persistent_hnsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.068834 chromadb-client-0.4.6.dev0/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/telemetry/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/telemetry/posthog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/test/db/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00001-migration-1.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00001-migration-1.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00002-migration-2.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00002-migration-2.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00003-migration-3.psql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/00003-migration-3.sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/db/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.072834 chromadb-client-0.4.6.dev0/chromadb/test/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/ingest/test_producer_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb/test/property/
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_cross_version_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/property/test_persist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb/test/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/segment/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/segment/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb/test/stress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/stress/test_many_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/test_multithreaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/test/utils/test_messagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/distance_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/messageid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/chromadb/utils/read_write_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.076834 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-04 06:33:06.000000 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-08-04 06:33:07.000000 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 06:33:06.000000 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 06:33:06.000000 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 06:33:06.000000 chromadb-client-0.4.6.dev0/chromadb_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.056833 chromadb-client-0.4.6.dev0/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.080834 chromadb-client-0.4.6.dev0/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.056833 chromadb-client-0.4.6.dev0/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.080834 chromadb-client-0.4.6.dev0/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68042 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.080834 chromadb-client-0.4.6.dev0/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17080 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/examples/node/yarn.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/genapi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   448020 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.080834 chromadb-client-0.4.6.dev0/clients/js/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/ChromaClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/Collection.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/IEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/models.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/generated/runtime.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/types.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/add.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/collection.client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/delete.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/get.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/initClient.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/peek.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/query.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/update.collection.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/test/upsert.collections.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156893 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/clients/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/python/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/python/build_python_thin_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/python/integration-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/python/is_thin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/clients/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/docker-compose.server.example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/docs/CIP_Chroma_Improvment_Proposals.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.084834 chromadb-client-0.4.6.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/examples/basic_functionality/
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/basic_functionality/alternative_embeddings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/basic_functionality/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/basic_functionality/start_here.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/basic_functionality/where_filtering.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/documents/state_of_the_union_2022.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55150 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/documents/state_of_the_union_2023.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/chat_with_your_documents/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.060834 chromadb-client-0.4.6.dev0/examples/deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/chroma.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/startup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.060834 chromadb-client-0.4.6.dev0/examples/use_with/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/examples/use_with/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/use_with/cohere/cohere_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/use_with/cohere/cohere_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/examples/use_with/cohere/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/log_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-04 06:33:01.000000 chromadb-client-0.4.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 06:32:49.000000 chromadb-client-0.4.6.dev0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 06:33:07.088834 chromadb-client-0.4.6.dev0/setup.cfg
```

### Comparing `chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml` & `chromadb-client-0.4.6.dev0/.github/ISSUE_TEMPLATE/installation_trouble.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/chroma-client-integration-test.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/chroma-client-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/chroma-integration-test.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/chroma-integration-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/chroma-release-python-client.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/chroma-release-python-client.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/chroma-release.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/chroma-test.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.github/workflows/pr-review-checklist.yml` & `chromadb-client-0.4.6.dev0/.github/workflows/pr-review-checklist.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.pre-commit-config.yaml` & `chromadb-client-0.4.6.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/.vscode/settings.json` & `chromadb-client-0.4.6.dev0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/DEVELOP.md` & `chromadb-client-0.4.6.dev0/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/Dockerfile` & `chromadb-client-0.4.6.dev0/Dockerfile`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/LICENSE` & `chromadb-client-0.4.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/PKG-INFO` & `chromadb-client-0.4.6.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.4.5.dev0
+Version: 0.4.6.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.5.dev0 Summary: Chroma
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.6.dev0 Summary: Chroma
 Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.4.5.dev0/README.md` & `chromadb-client-0.4.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/RELEASE_PROCESS.md` & `chromadb-client-0.4.6.dev0/RELEASE_PROCESS.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/bin/generate_cloudformation.py` & `chromadb-client-0.4.6.dev0/bin/generate_cloudformation.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/bin/windows_upgrade_sqlite.py` & `chromadb-client-0.4.6.dev0/bin/windows_upgrade_sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from chromadb.config import Settings, System
 from chromadb.api import API
 
 logger = logging.getLogger(__name__)
 
 __settings = Settings()
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 # Workaround to deal with Colab's old sqlite3 version
 try:
     import google.colab  # noqa: F401
 
     IN_COLAB = True
 except ImportError:
```

### Comparing `chromadb-client-0.4.5.dev0/chromadb/api/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/api/fastapi.py` & `chromadb-client-0.4.6.dev0/chromadb/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/api/models/Collection.py` & `chromadb-client-0.4.6.dev0/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/api/segment.py` & `chromadb-client-0.4.6.dev0/chromadb/api/segment.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/api/types.py` & `chromadb-client-0.4.6.dev0/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/config.py` & `chromadb-client-0.4.6.dev0/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/base.py` & `chromadb-client-0.4.6.dev0/chromadb/db/base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/impl/sqlite.py` & `chromadb-client-0.4.6.dev0/chromadb/db/impl/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/impl/sqlite_pool.py` & `chromadb-client-0.4.6.dev0/chromadb/db/impl/sqlite_pool.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/migrations.py` & `chromadb-client-0.4.6.dev0/chromadb/db/migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/mixins/embeddings_queue.py` & `chromadb-client-0.4.6.dev0/chromadb/db/mixins/embeddings_queue.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/mixins/sysdb.py` & `chromadb-client-0.4.6.dev0/chromadb/db/mixins/sysdb.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/db/system.py` & `chromadb-client-0.4.6.dev0/chromadb/db/system.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/errors.py` & `chromadb-client-0.4.6.dev0/chromadb/errors.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/experimental/density_relevance.ipynb` & `chromadb-client-0.4.6.dev0/chromadb/experimental/density_relevance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981369047619048%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(3, 'chroma_client = "*

 * *            'chromadb.PersistentClient(path="./chroma)")\\n\')], delete: [6, 5, 4, 3]}}, 8: '*

 * *            '{\'source\': {insert: [(6, "    collection.add(ids=[str(i) for i in range(i, min(i + '*

 * *            "batch_size, len(dataset)))], documents=dataset['support'][i:i + batch_size], "*

 * *            "metadatas=[{'type': 'support'} for _ in range(i, min(i + batch_size, "*

 * *            'len(dataset)))])")], delete: [8, 7, 6]}}}',*

 * * "'metadata'": "{'langua […]*

```diff
@@ -107,18 +107,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import chromadb\n",
                 "from chromadb.config import Settings\n",
                 "\n",
-                "chroma_client = chromadb.Client(Settings(\n",
-                "    chroma_db_impl=\"duckdb+parquet\",\n",
-                "    persist_directory=\"./\"\n",
-                "))\n",
+                "chroma_client = chromadb.PersistentClient(path=\"./chroma)\")\n",
                 "\n",
                 "collection = chroma_client.get_or_create_collection(name=\"sciq\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -160,17 +157,15 @@
             "source": [
                 "# Load the data and persist \n",
                 "collection.delete()\n",
                 "\n",
                 "from tqdm.notebook import tqdm\n",
                 "batch_size = 1000\n",
                 "for i in tqdm(range(0, len(dataset), batch_size)):\n",
-                "    collection.add(ids=[str(i) for i in range(i, min(i + batch_size, len(dataset)))], documents=dataset['support'][i:i + batch_size], metadatas=[{'type': 'support'} for _ in range(i, min(i + batch_size, len(dataset)))])\n",
-                "    \n",
-                "chroma_client.persist()"
+                "    collection.add(ids=[str(i) for i in range(i, min(i + batch_size, len(dataset)))], documents=dataset['support'][i:i + batch_size], metadatas=[{'type': 'support'} for _ in range(i, min(i + batch_size, len(dataset)))])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -534,14 +529,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.10.12"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `chromadb-client-0.4.5.dev0/chromadb/ingest/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql` & `chromadb-client-0.4.6.dev0/chromadb/migrations/metadb/00001-embedding-metadata.sqlite.sql`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/manager/local.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/manager/local.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/metadata/sqlite.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/batch.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/batch.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/brute_force_index.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/brute_force_index.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/hnsw_params.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/hnsw_params.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/local_hnsw.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/local_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/segment/impl/vector/local_persistent_hnsw.py` & `chromadb-client-0.4.6.dev0/chromadb/segment/impl/vector/local_persistent_hnsw.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/server/fastapi/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/server/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/server/fastapi/types.py` & `chromadb-client-0.4.6.dev0/chromadb/server/fastapi/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 
 class AddEmbedding(BaseModel):  # type: ignore
     # Pydantic doesn't handle Union types cleanly like Embeddings which has
     # Union[int, float] so we use Any here to ensure data is parsed
     # to its original type.
     embeddings: Optional[List[Any]] = None
-    metadatas: Optional[List[Dict[Any, Any]]] = None
-    documents: Optional[List[str]] = None
+    metadatas: Optional[List[Optional[Dict[Any, Any]]]] = None
+    documents: Optional[List[Optional[str]]] = None
     ids: List[str]
 
 
 class UpdateEmbedding(BaseModel):  # type: ignore
     embeddings: Optional[List[Any]] = None
-    metadatas: Optional[List[Dict[Any, Any]]] = None
-    documents: Optional[List[str]] = None
+    metadatas: Optional[List[Optional[Dict[Any, Any]]]] = None
+    documents: Optional[List[Optional[str]]] = None
     ids: List[str]
 
 
 class QueryEmbedding(BaseModel):  # type: ignore
     # TODO: Pydantic doesn't bode well with recursive types so we use generic Dicts
     # for Where and WhereDocument. This is not ideal, but it works for now since
     # there is a lot of downstream validation.
```

### Comparing `chromadb-client-0.4.5.dev0/chromadb/telemetry/__init__.py` & `chromadb-client-0.4.6.dev0/chromadb/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/telemetry/events.py` & `chromadb-client-0.4.6.dev0/chromadb/telemetry/events.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/telemetry/posthog.py` & `chromadb-client-0.4.6.dev0/chromadb/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/conftest.py` & `chromadb-client-0.4.6.dev0/chromadb/test/conftest.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/db/test_base.py` & `chromadb-client-0.4.6.dev0/chromadb/test/db/test_base.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/db/test_migrations.py` & `chromadb-client-0.4.6.dev0/chromadb/test/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/db/test_system.py` & `chromadb-client-0.4.6.dev0/chromadb/test/db/test_system.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/ingest/test_producer_consumer.py` & `chromadb-client-0.4.6.dev0/chromadb/test/ingest/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/invariants.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/invariants.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/strategies.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/strategies.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_add.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_add.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,7 +82,27 @@
     coll = api.create_collection(
         "test", embedding_function=lambda texts: [[1, 2, 3] for _ in texts]  # type: ignore
     )
     embeddings: Embeddings = [[1, 2, 3] for _ in ooo_ids]
     coll.add(ids=ooo_ids, embeddings=embeddings)
     get_ids = coll.get(ids=ooo_ids)["ids"]
     assert get_ids == ooo_ids
+
+
+def test_add_partial(api: API) -> None:
+    """Tests adding a record set with some of the fields set to None."""
+
+    api.reset()
+
+    coll = api.create_collection("test")
+    # TODO: We need to clean up the api types to support this typing
+    coll.add(
+        ids=["1", "2", "3"],
+        embeddings=[[1, 2, 3], [1, 2, 3], [1, 2, 3]],
+        metadatas=[{"a": 1}, None, {"a": 3}],  # type: ignore
+        documents=["a", "b", None],  # type: ignore
+    )
+
+    results = coll.get()
+    assert results["ids"] == ["1", "2", "3"]
+    assert results["metadatas"] == [{"a": 1}, None, {"a": 3}]
+    assert results["documents"] == ["a", "b", None]
```

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_collections.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_cross_version_persist.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_cross_version_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_embeddings.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_filtering.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_filtering.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/property/test_persist.py` & `chromadb-client-0.4.6.dev0/chromadb/test/property/test_persist.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/segment/test_metadata.py` & `chromadb-client-0.4.6.dev0/chromadb/test/segment/test_metadata.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/segment/test_vector.py` & `chromadb-client-0.4.6.dev0/chromadb/test/segment/test_vector.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/stress/test_many_collections.py` & `chromadb-client-0.4.6.dev0/chromadb/test/stress/test_many_collections.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/test_api.py` & `chromadb-client-0.4.6.dev0/chromadb/test/test_api.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/test_chroma.py` & `chromadb-client-0.4.6.dev0/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/test_client.py` & `chromadb-client-0.4.6.dev0/chromadb/test/test_client.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/test_config.py` & `chromadb-client-0.4.6.dev0/chromadb/test/test_config.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/test_multithreaded.py` & `chromadb-client-0.4.6.dev0/chromadb/test/test_multithreaded.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/test/utils/test_messagid.py` & `chromadb-client-0.4.6.dev0/chromadb/test/utils/test_messagid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/types.py` & `chromadb-client-0.4.6.dev0/chromadb/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/delete_file.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/delete_file.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/distance_functions.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/distance_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/embedding_functions.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/lru_cache.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/messageid.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/messageid.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb/utils/read_write_lock.py` & `chromadb-client-0.4.6.dev0/chromadb/utils/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/chromadb_client.egg-info/PKG-INFO` & `chromadb-client-0.4.6.dev0/chromadb_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb-client
-Version: 0.4.5.dev0
+Version: 0.4.6.dev0
 Summary: Chroma Client.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.5.dev0 Summary: Chroma
+Metadata-Version: 2.1 Name: chromadb-client Version: 0.4.6.dev0 Summary: Chroma
 Client. Author-email: Jeff Huber
 trychroma.com>, Anton Troynikov
 trychroma.com> Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `chromadb-client-0.4.5.dev0/chromadb_client.egg-info/SOURCES.txt` & `chromadb-client-0.4.6.dev0/chromadb_client.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -176,15 +176,22 @@
 clients/python/integration-test.sh
 clients/python/is_thin_client.py
 clients/python/pyproject.toml
 docs/CIP_Chroma_Improvment_Proposals.md
 examples/README.md
 examples/basic_functionality/alternative_embeddings.ipynb
 examples/basic_functionality/local_persistence.ipynb
+examples/basic_functionality/start_here.ipynb
 examples/basic_functionality/where_filtering.ipynb
+examples/chat_with_your_documents/README.md
+examples/chat_with_your_documents/load_data.py
+examples/chat_with_your_documents/main.py
+examples/chat_with_your_documents/requirements.txt
+examples/chat_with_your_documents/documents/state_of_the_union_2022.txt
+examples/chat_with_your_documents/documents/state_of_the_union_2023.txt
 examples/deployments/google-cloud-compute/README.md
 examples/deployments/google-cloud-compute/chroma.tf
 examples/deployments/google-cloud-compute/main.tf
 examples/deployments/google-cloud-compute/startup.sh
 examples/deployments/google-cloud-compute/variables.tf
 examples/use_with/cohere/cohere_js.js
 examples/use_with/cohere/cohere_python.ipynb
```

### Comparing `chromadb-client-0.4.5.dev0/clients/js/DEVELOP.md` & `chromadb-client-0.4.6.dev0/clients/js/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/LICENSE` & `chromadb-client-0.4.6.dev0/clients/js/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/README.md` & `chromadb-client-0.4.6.dev0/clients/js/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/examples/browser/app.ts` & `chromadb-client-0.4.6.dev0/clients/js/examples/browser/app.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/examples/browser/index.html` & `chromadb-client-0.4.6.dev0/clients/js/examples/browser/index.html`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/examples/browser/yarn.lock` & `chromadb-client-0.4.6.dev0/clients/js/examples/browser/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/examples/node/app.js` & `chromadb-client-0.4.6.dev0/clients/js/examples/node/app.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/examples/node/yarn.lock` & `chromadb-client-0.4.6.dev0/clients/js/examples/node/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/genapi.sh` & `chromadb-client-0.4.6.dev0/clients/js/genapi.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/package-lock.json` & `chromadb-client-0.4.6.dev0/clients/js/package-lock.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/package.json` & `chromadb-client-0.4.6.dev0/clients/js/package.json`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/ChromaClient.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/ChromaClient.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/Collection.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/Collection.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/embeddings/CohereEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/embeddings/OpenAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/embeddings/TransformersEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/embeddings/WebAIEmbeddingFunction.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/generated/README.md` & `chromadb-client-0.4.6.dev0/clients/js/src/generated/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/generated/api.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/generated/api.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/generated/configuration.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/generated/configuration.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/generated/models.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/generated/models.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/generated/runtime.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/generated/runtime.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/types.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/types.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/src/utils.ts` & `chromadb-client-0.4.6.dev0/clients/js/src/utils.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/add.collections.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/add.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/client.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/collection.client.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/collection.client.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/delete.collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/delete.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/get.collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/get.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/peek.collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/peek.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/query.collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/query.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/update.collection.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/update.collection.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/test/upsert.collections.test.ts` & `chromadb-client-0.4.6.dev0/clients/js/test/upsert.collections.test.ts`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/js/yarn.lock` & `chromadb-client-0.4.6.dev0/clients/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/python/README.md` & `chromadb-client-0.4.6.dev0/clients/python/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/python/build_python_thin_client.sh` & `chromadb-client-0.4.6.dev0/clients/python/build_python_thin_client.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/python/integration-test.sh` & `chromadb-client-0.4.6.dev0/clients/python/integration-test.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/clients/python/pyproject.toml` & `chromadb-client-0.4.6.dev0/clients/python/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/docker-compose.test.yml` & `chromadb-client-0.4.6.dev0/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/docs/CIP_Chroma_Improvment_Proposals.md` & `chromadb-client-0.4.6.dev0/docs/CIP_Chroma_Improvment_Proposals.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/README.md` & `chromadb-client-0.4.6.dev0/examples/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/basic_functionality/alternative_embeddings.ipynb` & `chromadb-client-0.4.6.dev0/examples/basic_functionality/alternative_embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/basic_functionality/local_persistence.ipynb` & `chromadb-client-0.4.6.dev0/examples/basic_functionality/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/basic_functionality/where_filtering.ipynb` & `chromadb-client-0.4.6.dev0/examples/basic_functionality/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/README.md` & `chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/README.md`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/chroma.tf` & `chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/chroma.tf`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/deployments/google-cloud-compute/startup.sh` & `chromadb-client-0.4.6.dev0/examples/deployments/google-cloud-compute/startup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/use_with/cohere/cohere_js.js` & `chromadb-client-0.4.6.dev0/examples/use_with/cohere/cohere_js.js`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/examples/use_with/cohere/cohere_python.ipynb` & `chromadb-client-0.4.6.dev0/examples/use_with/cohere/cohere_python.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-client-0.4.5.dev0/pyproject.toml` & `chromadb-client-0.4.6.dev0/pyproject.toml`

 * *Files identical despite different names*

