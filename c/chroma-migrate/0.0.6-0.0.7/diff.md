# Comparing `tmp/chroma_migrate-0.0.6.tar.gz` & `tmp/chroma_migrate-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma_migrate-0.0.6.tar", last modified: Thu Jul 20 15:45:29 2023, max compression
+gzip compressed data, was "chroma_migrate-0.0.7.tar", last modified: Fri Aug  4 03:20:11 2023, max compression
```

## Comparing `chroma_migrate-0.0.6.tar` & `chroma_migrate-0.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.677683 chroma_migrate-0.0.6/
--rw-r--r--   0 hammad     (501) staff       (20)     3077 2023-07-13 19:12:18.000000 chroma_migrate-0.0.6/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-07-14 01:27:39.000000 chroma_migrate-0.0.6/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-20 15:45:29.677538 chroma_migrate-0.0.6/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     2746 2023-07-17 23:28:10.000000 chroma_migrate-0.0.6/README.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.669624 chroma_migrate-0.0.6/chroma_migrate/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/__main__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8422 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     2382 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/import_chromadb.py
--rw-r--r--   0 hammad     (501) staff       (20)     2409 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/import_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)     3358 2023-07-20 15:45:15.000000 chroma_migrate-0.0.6/chroma_migrate/import_duckdb.py
--rw-r--r--   0 hammad     (501) staff       (20)      846 2023-07-20 00:21:44.000000 chroma_migrate-0.0.6/chroma_migrate/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.670519 chroma_migrate-0.0.6/chroma_migrate.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     3752 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       62 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/entry_points.txt
--rw-r--r--   0 hammad     (501) staff       (20)       90 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2023-07-20 15:45:29.000000 chroma_migrate-0.0.6/chroma_migrate.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.670903 chroma_migrate-0.0.6/examples/
--rw-r--r--   0 hammad     (501) staff       (20)      561 2023-07-17 04:16:54.000000 chroma_migrate-0.0.6/examples/from_chroma.py
--rw-r--r--   0 hammad     (501) staff       (20)      508 2023-07-17 04:15:07.000000 chroma_migrate-0.0.6/examples/from_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)      484 2023-07-17 04:13:58.000000 chroma_migrate-0.0.6/examples/from_duckdb.py
--rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-14 05:33:16.000000 chroma_migrate-0.0.6/main.py
--rw-r--r--   0 hammad     (501) staff       (20)      886 2023-07-18 21:38:25.000000 chroma_migrate-0.0.6/pyproject.toml
--rw-r--r--   0 hammad     (501) staff       (20)      105 2023-07-18 21:38:06.000000 chroma_migrate-0.0.6/requirements.txt
--rw-r--r--   0 hammad     (501) staff       (20)       12 2023-07-14 20:19:32.000000 chroma_migrate-0.0.6/requirements_dev.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-20 15:45:29.677716 chroma_migrate-0.0.6/setup.cfg
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.671171 chroma_migrate-0.0.6/test_data_duckdb/
--rw-r--r--   0 hammad     (501) staff       (20)     1013 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/chroma-collections.parquet
--rw-r--r--   0 hammad     (501) staff       (20)   215734 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/chroma-embeddings.parquet
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.677073 chroma_migrate-0.0.6/test_data_duckdb/index/
--rw-r--r--   0 hammad     (501) staff       (20)     1452 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2897 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      318 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1515 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1138 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      820 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2360 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2798 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      256 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3004 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
--rw-r--r--   0 hammad     (501) staff       (20)    16972 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin
--rw-r--r--   0 hammad     (501) staff       (20)    39816 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin
--rw-r--r--   0 hammad     (501) staff       (20)     2468 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin
--rw-r--r--   0 hammad     (501) staff       (20)    19032 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin
--rw-r--r--   0 hammad     (501) staff       (20)    15352 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin
--rw-r--r--   0 hammad     (501) staff       (20)     6132 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin
--rw-r--r--   0 hammad     (501) staff       (20)    15168 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin
--rw-r--r--   0 hammad     (501) staff       (20)    33944 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin
--rw-r--r--   0 hammad     (501) staff       (20)     2768 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin
--rw-r--r--   0 hammad     (501) staff       (20)    21936 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/index_metadata_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1681 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3383 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      349 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1755 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1311 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      941 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2754 2023-07-13 21:50:23.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3272 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      275 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3494 2023-07-13 21:50:22.000000 chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 15:45:29.677346 chroma_migrate-0.0.6/test_scripts/
--rw-r--r--   0 hammad     (501) staff       (20)      961 2023-07-13 23:36:16.000000 chroma_migrate-0.0.6/test_scripts/generate_test_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)     1008 2023-07-13 21:49:24.000000 chroma_migrate-0.0.6/test_scripts/generate_test_duckdb.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.328294 chroma_migrate-0.0.7/
+-rw-r--r--   0 hammad     (501) staff       (20)     3077 2023-07-13 19:12:18.000000 chroma_migrate-0.0.7/.gitignore
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-07-14 01:27:39.000000 chroma_migrate-0.0.7/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-08-04 03:20:11.328153 chroma_migrate-0.0.7/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     2746 2023-07-17 23:28:10.000000 chroma_migrate-0.0.7/README.md
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.319922 chroma_migrate-0.0.7/chroma_migrate/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2023-08-04 02:51:27.000000 chroma_migrate-0.0.7/chroma_migrate/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)       80 2023-08-04 02:51:38.000000 chroma_migrate-0.0.7/chroma_migrate/__main__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8702 2023-08-04 03:18:44.000000 chroma_migrate-0.0.7/chroma_migrate/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2403 2023-08-04 03:18:44.000000 chroma_migrate-0.0.7/chroma_migrate/import_chromadb.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2431 2023-08-04 03:18:44.000000 chroma_migrate-0.0.7/chroma_migrate/import_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3380 2023-08-04 03:18:44.000000 chroma_migrate-0.0.7/chroma_migrate/import_duckdb.py
+-rw-r--r--   0 hammad     (501) staff       (20)      846 2023-08-04 02:51:47.000000 chroma_migrate-0.0.7/chroma_migrate/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.320834 chroma_migrate-0.0.7/chroma_migrate.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     3752 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       62 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       90 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2023-08-04 03:20:11.000000 chroma_migrate-0.0.7/chroma_migrate.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.321314 chroma_migrate-0.0.7/examples/
+-rw-r--r--   0 hammad     (501) staff       (20)      561 2023-07-17 04:16:54.000000 chroma_migrate-0.0.7/examples/from_chroma.py
+-rw-r--r--   0 hammad     (501) staff       (20)      508 2023-07-17 04:15:07.000000 chroma_migrate-0.0.7/examples/from_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)      484 2023-07-17 04:13:58.000000 chroma_migrate-0.0.7/examples/from_duckdb.py
+-rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-14 05:33:16.000000 chroma_migrate-0.0.7/main.py
+-rw-r--r--   0 hammad     (501) staff       (20)      886 2023-07-18 21:38:25.000000 chroma_migrate-0.0.7/pyproject.toml
+-rw-r--r--   0 hammad     (501) staff       (20)      105 2023-07-18 21:38:06.000000 chroma_migrate-0.0.7/requirements.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       12 2023-07-14 20:19:32.000000 chroma_migrate-0.0.7/requirements_dev.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2023-08-04 03:20:11.328329 chroma_migrate-0.0.7/setup.cfg
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.321605 chroma_migrate-0.0.7/test_data_duckdb/
+-rw-r--r--   0 hammad     (501) staff       (20)     1013 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/chroma-collections.parquet
+-rw-r--r--   0 hammad     (501) staff       (20)   215734 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/chroma-embeddings.parquet
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.327653 chroma_migrate-0.0.7/test_data_duckdb/index/
+-rw-r--r--   0 hammad     (501) staff       (20)     1452 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2897 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      318 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1515 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1138 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      820 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2360 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2798 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      256 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3004 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)    16972 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    39816 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     2468 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    19032 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    15352 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     6132 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    15168 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    33944 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     2768 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    21936 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/index_metadata_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1681 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3383 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      349 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1755 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1311 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      941 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2754 2023-07-13 21:50:23.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3272 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      275 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3494 2023-07-13 21:50:22.000000 chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-08-04 03:20:11.327934 chroma_migrate-0.0.7/test_scripts/
+-rw-r--r--   0 hammad     (501) staff       (20)      961 2023-07-13 23:36:16.000000 chroma_migrate-0.0.7/test_scripts/generate_test_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1008 2023-07-13 21:49:24.000000 chroma_migrate-0.0.7/test_scripts/generate_test_duckdb.py
```

### Comparing `chroma_migrate-0.0.6/.gitignore` & `chroma_migrate-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/LICENSE` & `chroma_migrate-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/PKG-INFO` & `chroma_migrate-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma_migrate
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for migrating to chroma versions >= 0.4.0
 Author-email: Jeff Huber <jeff@trychroma.com>, Hammad Bashir <hammad@trychroma.com>
 Keywords: chroma,migrate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `chroma_migrate-0.0.6/README.md` & `chroma_migrate-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/chroma_migrate/cli.py` & `chroma_migrate-0.0.7/chroma_migrate/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,23 +75,23 @@
         prompts.append(clickhouse_port)
 
     if "DuckDB" in current_config:
         duckdb_path = Input("What is the path to the persist directory your data is currently stored in?", default = "./chroma", word_color = colors.foreground["yellow"])
         prompts.append(duckdb_path)
     
     if "Chroma server" in current_config:
-        chroma_host = Input("What is the ip/hostname of your chroma server", default = "localhost", word_color = colors.foreground["yellow"])
-        chroma_port = Input("What is the port of your chroma server", default = "8000", word_color = colors.foreground["yellow"])
+        chroma_host = Input("What is the ip/hostname of your source chroma server", default = "localhost", word_color = colors.foreground["yellow"])
+        chroma_port = Input("What is the port of your source chroma server", default = "8000", word_color = colors.foreground["yellow"])
         prompts.append(chroma_host)
         prompts.append(chroma_port)
 
     if target_config == "A chroma server that I can access via HTTP":
-        chroma_host = Input("What is the ip/hostname of your chroma server", default = "localhost", word_color = colors.foreground["yellow"])
-        chroma_port = Input("What is the port of your chroma server", default = "8000", word_color = colors.foreground["yellow"])
-        chroma_headers = Input("What headers would you like to use to authenticate with your chroma server? (JSON format)", default = "{}", word_color = colors.foreground["yellow"])
+        chroma_host = Input("What is the ip/hostname of your destination chroma server", default = "localhost", word_color = colors.foreground["yellow"])
+        chroma_port = Input("What is the port of your destination chroma server", default = "8000", word_color = colors.foreground["yellow"])
+        chroma_headers = Input("What headers would you like to use to authenticate with your destination chroma server? (JSON format)", default = "{}", word_color = colors.foreground["yellow"])
         target_chroma = "REMOTE"
         prompts.append(chroma_host)
         prompts.append(chroma_port)
         prompts.append(chroma_headers)
 
     if target_config == "Files I can use on my local machine with chroma, or upload to a remote server that runs chroma":
         chroma_persist_directory = Input("What is the path you would like your data to be stored in?", default = "./chroma_migrated", word_color = colors.foreground["yellow"])
@@ -107,56 +107,58 @@
         for prompt, answer in result:
             if prompt == "What is the path you would like your data to be stored in?":
                 persist_directory = answer
         api = chromadb.PersistentClient(path=persist_directory)
 
     if target_chroma == "REMOTE":
         for prompt, answer in result:
-            if prompt == "What is the ip/hostname of your chroma server":
+            if prompt == "What is the ip/hostname of your destination chroma server":
                 chroma_host = answer
-            if prompt == "What is the port of your chroma server":
+            if prompt == "What is the port of your destination chroma server":
                 chroma_port = answer
-            if prompt == "What headers would you like to use to authenticate with your chroma server? (JSON format)":
+            if prompt == "What headers would you like to use to authenticate with your destination chroma server? (JSON format)":
                 try:
                     chroma_headers = json.loads(answer)
                 except Exception:
                     print("Invalid JSON format for headers")
                     exit(1)
         api = chromadb.HttpClient(host=chroma_host, port=chroma_port, headers=chroma_headers)
 
+    did_migration = False
     if "DuckDB" in current_config:
         for prompt, answer in result:
             if prompt == "What is the path to the persist directory your data is currently stored in?":
                 persist_directory = answer
-        migrate_from_duckdb(api, persist_directory)
+        did_migration = migrate_from_duckdb(api, persist_directory)
 
     if "Clickhouse" in current_config:
         for prompt, answer in result:
             if prompt == "What is the ip/hostname of your clickhouse server":
                 clickhouse_host = answer
             if prompt == "What is the port of your clickhouse server":
                 clickhouse_port = answer
-        migrate_from_clickhouse(api, clickhouse_host, clickhouse_port)
+        did_migration = migrate_from_clickhouse(api, clickhouse_host, clickhouse_port)
     
     if "Chroma server" in current_config:
         for prompt, answer in result:
-            if prompt == "What is the ip/hostname of your chroma server":
-                chroma_host = answer
-            if prompt == "What is the port of your chroma server":
-                chroma_port = answer
-        from_chroma = chromadb.HttpClient(host=chroma_host, port=chroma_port)
-        migrate_from_remote_chroma(from_chroma, api)
-
-    if target_chroma == "LOCAL":
-        print(f"Your data has been migrated to: {persist_directory}!")
-        print("\n")
-        print("You can now instantiate a chroma client with the following code:")
-        print("import chromadb")
-        print("api = chromadb.PersistentClient(path=\"" + persist_directory + "\")")
+            if prompt == "What is the ip/hostname of your source chroma server":
+                chroma_source_host = answer
+            if prompt == "What is the port of your source chroma server":
+                chroma_source_port = answer
+        from_chroma = chromadb.HttpClient(host=chroma_source_host, port=chroma_source_port)
+        did_migration = migrate_from_remote_chroma(from_chroma, api)
     
-    if target_chroma == "REMOTE":
-        print(f"Your data has been migrated to: {chroma_host}:{chroma_port}!")
-        print("\n")
-        print("You can now instantiate a chroma client with the following code:")
-        print("import chromadb")
-        print("api = chromadb.HttpClient(host=\"" + chroma_host + "\", port=\"" + chroma_port + "\")")
+    if did_migration:
+        if target_chroma == "LOCAL":
+            print(f"Your data has been migrated to: {persist_directory}!")
+            print("\n")
+            print("You can now instantiate a chroma client with the following code:")
+            print("import chromadb")
+            print("api = chromadb.PersistentClient(path=\"" + persist_directory + "\")")
+        
+        if target_chroma == "REMOTE":
+            print(f"Your data has been migrated to: {chroma_host}:{chroma_port}!")
+            print("\n")
+            print("You can now instantiate a chroma client with the following code:")
+            print("import chromadb")
+            print("api = chromadb.HttpClient(host=\"" + chroma_host + "\", port=\"" + chroma_port + "\")")
```

### Comparing `chroma_migrate-0.0.6/chroma_migrate/import_chromadb.py` & `chroma_migrate-0.0.7/chroma_migrate/import_chromadb.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def migrate_from_remote_chroma(from_api: API, to_api: API):
     
     print("Loading Existing Collections...")
     from_collections = from_api.list_collections()
 
     if len(from_collections) == 0:
         print("No collections found, exiting...")
-        return
+        return False
 
     print("Validating collection metadata...")
     from_collection_to_metadata = {}
     for collection in from_collections:
         from_collection_to_metadata[collection.name] = validate_collection_metadata(collection.metadata)
 
     print("Migrating existing collections...")
@@ -46,7 +46,8 @@
 
                 documents = data["documents"][absolute_position:absolute_position+chunk_size]
                 to_collection.add(ids, embeddings, metadatas, documents)
                 pbar.update(len(chunk))
                 absolute_position += len(chunk)
     
     print(f"Migrated {len(from_collections)} collections and {total_embeddings} embeddings")
+    return True
```

### Comparing `chroma_migrate-0.0.6/chroma_migrate/import_clickhouse.py` & `chroma_migrate-0.0.7/chroma_migrate/import_clickhouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     print("Loading existing collections...")
     # Read the collections from clickhouse
     collections = conn.query("SELECT uuid, name, metadata FROM collections").result_rows
 
     if len(collections) == 0:
         print("No collections found, exiting...")
-        return
+        return False
 
     print("Validating collection metadata...")
     from_collection_to_metadata = {}
     for collection in collections:
         metadata = json.loads(collection[2])
         from_collection_to_metadata[collection[1]] = validate_collection_metadata(metadata)
 
@@ -53,8 +53,9 @@
                     document = record[4]
                     metadata = json.loads(record[5])
                     metadata = migrate_embedding_metadata(metadata)
                     collection = collection_uuid_to_chroma_collection[collection_uuid]
                     collection.add(id, embedding, metadata, document)
                     pbar.update(1)
     
-    print(f"Migrated {len(collections)} collections and {pbar.n} embeddings")
+    print(f"Migrated {len(collections)} collections and {pbar.n} embeddings")
+    return True
```

### Comparing `chroma_migrate-0.0.6/chroma_migrate/import_duckdb.py` & `chroma_migrate-0.0.7/chroma_migrate/import_duckdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     )
 
     # Read the collections from duckdb
     collections = conn.execute("SELECT uuid, name, metadata FROM collections").fetchall()
 
     if len(collections) == 0:
         print("No collections found, exiting...")
-        return
+        return False
 
     print("Validating collection metadata...")
     from_collection_to_metadata = {}
     for collection in collections:
         uuid, name, metadata = collection
         metadata = json.loads(metadata)
         from_collection_to_metadata[name] = validate_collection_metadata(metadata)
@@ -76,8 +76,9 @@
             document = None
         metadata = migrate_embedding_metadata(metadata)
         collection = collection_uuid_to_chroma_collection[collection_uuid]
         collection.add(id, embedding, metadata, document)
 
     print(f"Migrated {len(collections)} collections and {embeddings.shape[0]} embeddings")
 
+    return True
```

### Comparing `chroma_migrate-0.0.6/chroma_migrate/utils.py` & `chroma_migrate-0.0.7/chroma_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/chroma_migrate.egg-info/PKG-INFO` & `chroma_migrate-0.0.7/chroma_migrate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma-migrate
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for migrating to chroma versions >= 0.4.0
 Author-email: Jeff Huber <jeff@trychroma.com>, Hammad Bashir <hammad@trychroma.com>
 Keywords: chroma,migrate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `chroma_migrate-0.0.6/chroma_migrate.egg-info/SOURCES.txt` & `chroma_migrate-0.0.7/chroma_migrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/examples/from_chroma.py` & `chroma_migrate-0.0.7/examples/from_chroma.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/pyproject.toml` & `chroma_migrate-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/chroma-collections.parquet` & `chroma_migrate-0.0.7/test_data_duckdb/chroma-collections.parquet`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/chroma-embeddings.parquet` & `chroma_migrate-0.0.7/test_data_duckdb/chroma-embeddings.parquet`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin` & `chroma_migrate-0.0.7/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl` & `chroma_migrate-0.0.7/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_scripts/generate_test_clickhouse.py` & `chroma_migrate-0.0.7/test_scripts/generate_test_clickhouse.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.6/test_scripts/generate_test_duckdb.py` & `chroma_migrate-0.0.7/test_scripts/generate_test_duckdb.py`

 * *Files identical despite different names*

