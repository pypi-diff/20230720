# Comparing `tmp/chroma_migrate-0.0.4.tar.gz` & `tmp/chroma_migrate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma_migrate-0.0.4.tar", last modified: Tue Jul 18 21:43:35 2023, max compression
+gzip compressed data, was "chroma_migrate-0.0.5.tar", last modified: Thu Jul 20 00:42:18 2023, max compression
```

## Comparing `chroma_migrate-0.0.4.tar` & `chroma_migrate-0.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.267164 chroma_migrate-0.0.4/
--rw-r--r--   0 hammad     (501) staff       (20)     3077 2023-07-13 19:12:18.000000 chroma_migrate-0.0.4/.gitignore
--rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-07-14 01:27:39.000000 chroma_migrate-0.0.4/LICENSE
--rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-18 21:43:35.267030 chroma_migrate-0.0.4/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     2746 2023-07-17 23:28:10.000000 chroma_migrate-0.0.4/README.md
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.254885 chroma_migrate-0.0.4/chroma_migrate/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2023-07-14 05:20:59.000000 chroma_migrate-0.0.4/chroma_migrate/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-14 05:21:57.000000 chroma_migrate-0.0.4/chroma_migrate/__main__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8422 2023-07-17 04:18:11.000000 chroma_migrate-0.0.4/chroma_migrate/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     2382 2023-07-17 04:18:11.000000 chroma_migrate-0.0.4/chroma_migrate/import_chromadb.py
--rw-r--r--   0 hammad     (501) staff       (20)     2409 2023-07-17 04:18:11.000000 chroma_migrate-0.0.4/chroma_migrate/import_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)     3031 2023-07-17 04:18:11.000000 chroma_migrate-0.0.4/chroma_migrate/import_duckdb.py
--rw-r--r--   0 hammad     (501) staff       (20)      846 2023-07-17 04:18:11.000000 chroma_migrate-0.0.4/chroma_migrate/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.255898 chroma_migrate-0.0.4/chroma_migrate.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     3752 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       62 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/entry_points.txt
--rw-r--r--   0 hammad     (501) staff       (20)       90 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2023-07-18 21:43:35.000000 chroma_migrate-0.0.4/chroma_migrate.egg-info/top_level.txt
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.256695 chroma_migrate-0.0.4/examples/
--rw-r--r--   0 hammad     (501) staff       (20)      561 2023-07-17 04:16:54.000000 chroma_migrate-0.0.4/examples/from_chroma.py
--rw-r--r--   0 hammad     (501) staff       (20)      508 2023-07-17 04:15:07.000000 chroma_migrate-0.0.4/examples/from_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)      484 2023-07-17 04:13:58.000000 chroma_migrate-0.0.4/examples/from_duckdb.py
--rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-14 05:33:16.000000 chroma_migrate-0.0.4/main.py
--rw-r--r--   0 hammad     (501) staff       (20)      886 2023-07-18 21:38:25.000000 chroma_migrate-0.0.4/pyproject.toml
--rw-r--r--   0 hammad     (501) staff       (20)      105 2023-07-18 21:38:06.000000 chroma_migrate-0.0.4/requirements.txt
--rw-r--r--   0 hammad     (501) staff       (20)       12 2023-07-14 20:19:32.000000 chroma_migrate-0.0.4/requirements_dev.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-18 21:43:35.267202 chroma_migrate-0.0.4/setup.cfg
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.257309 chroma_migrate-0.0.4/test_data_duckdb/
--rw-r--r--   0 hammad     (501) staff       (20)     1013 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/chroma-collections.parquet
--rw-r--r--   0 hammad     (501) staff       (20)   215734 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/chroma-embeddings.parquet
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.266574 chroma_migrate-0.0.4/test_data_duckdb/index/
--rw-r--r--   0 hammad     (501) staff       (20)     1452 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2897 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      318 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1515 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1138 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      820 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2360 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2798 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      256 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3004 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
--rw-r--r--   0 hammad     (501) staff       (20)    16972 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin
--rw-r--r--   0 hammad     (501) staff       (20)    39816 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin
--rw-r--r--   0 hammad     (501) staff       (20)     2468 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin
--rw-r--r--   0 hammad     (501) staff       (20)    19032 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin
--rw-r--r--   0 hammad     (501) staff       (20)    15352 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin
--rw-r--r--   0 hammad     (501) staff       (20)     6132 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin
--rw-r--r--   0 hammad     (501) staff       (20)    15168 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin
--rw-r--r--   0 hammad     (501) staff       (20)    33944 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin
--rw-r--r--   0 hammad     (501) staff       (20)     2768 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin
--rw-r--r--   0 hammad     (501) staff       (20)    21936 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/index_metadata_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1681 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3383 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      349 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1755 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     1311 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      941 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     2754 2023-07-13 21:50:23.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3272 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
--rw-r--r--   0 hammad     (501) staff       (20)      275 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
--rw-r--r--   0 hammad     (501) staff       (20)     3494 2023-07-13 21:50:22.000000 chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-18 21:43:35.266845 chroma_migrate-0.0.4/test_scripts/
--rw-r--r--   0 hammad     (501) staff       (20)      961 2023-07-13 23:36:16.000000 chroma_migrate-0.0.4/test_scripts/generate_test_clickhouse.py
--rw-r--r--   0 hammad     (501) staff       (20)     1008 2023-07-13 21:49:24.000000 chroma_migrate-0.0.4/test_scripts/generate_test_duckdb.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.492907 chroma_migrate-0.0.5/
+-rw-r--r--   0 hammad     (501) staff       (20)     3077 2023-07-13 19:12:18.000000 chroma_migrate-0.0.5/.gitignore
+-rw-r--r--   0 hammad     (501) staff       (20)    11357 2023-07-14 01:27:39.000000 chroma_migrate-0.0.5/LICENSE
+-rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-20 00:42:18.492758 chroma_migrate-0.0.5/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     2746 2023-07-17 23:28:10.000000 chroma_migrate-0.0.5/README.md
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.481728 chroma_migrate-0.0.5/chroma_migrate/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/__main__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8422 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2382 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/import_chromadb.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2409 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/import_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3288 2023-07-20 00:40:06.000000 chroma_migrate-0.0.5/chroma_migrate/import_duckdb.py
+-rw-r--r--   0 hammad     (501) staff       (20)      846 2023-07-20 00:21:44.000000 chroma_migrate-0.0.5/chroma_migrate/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.482568 chroma_migrate-0.0.5/chroma_migrate.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)     3215 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     3752 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       62 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       90 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2023-07-20 00:42:18.000000 chroma_migrate-0.0.5/chroma_migrate.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.483498 chroma_migrate-0.0.5/examples/
+-rw-r--r--   0 hammad     (501) staff       (20)      561 2023-07-17 04:16:54.000000 chroma_migrate-0.0.5/examples/from_chroma.py
+-rw-r--r--   0 hammad     (501) staff       (20)      508 2023-07-17 04:15:07.000000 chroma_migrate-0.0.5/examples/from_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)      484 2023-07-17 04:13:58.000000 chroma_migrate-0.0.5/examples/from_duckdb.py
+-rw-r--r--   0 hammad     (501) staff       (20)       80 2023-07-14 05:33:16.000000 chroma_migrate-0.0.5/main.py
+-rw-r--r--   0 hammad     (501) staff       (20)      886 2023-07-18 21:38:25.000000 chroma_migrate-0.0.5/pyproject.toml
+-rw-r--r--   0 hammad     (501) staff       (20)      105 2023-07-18 21:38:06.000000 chroma_migrate-0.0.5/requirements.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       12 2023-07-14 20:19:32.000000 chroma_migrate-0.0.5/requirements_dev.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2023-07-20 00:42:18.492944 chroma_migrate-0.0.5/setup.cfg
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.483886 chroma_migrate-0.0.5/test_data_duckdb/
+-rw-r--r--   0 hammad     (501) staff       (20)     1013 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/chroma-collections.parquet
+-rw-r--r--   0 hammad     (501) staff       (20)   215734 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/chroma-embeddings.parquet
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.492234 chroma_migrate-0.0.5/test_data_duckdb/index/
+-rw-r--r--   0 hammad     (501) staff       (20)     1452 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2897 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      318 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1515 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1138 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      820 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2360 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2798 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      256 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3004 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)    16972 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    39816 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     2468 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    19032 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    15352 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     6132 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    15168 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    33944 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin
+-rw-r--r--   0 hammad     (501) staff       (20)     2768 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin
+-rw-r--r--   0 hammad     (501) staff       (20)    21936 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      102 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/index_metadata_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1681 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3383 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      349 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_71c07377-67be-4e5d-9270-2c71ec881f59.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1755 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     1311 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      941 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     2754 2023-07-13 21:50:23.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3272 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)      275 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_f29adc7f-4178-4c82-8fb2-1ae513520fe8.pkl
+-rw-r--r--   0 hammad     (501) staff       (20)     3494 2023-07-13 21:50:22.000000 chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2023-07-20 00:42:18.492572 chroma_migrate-0.0.5/test_scripts/
+-rw-r--r--   0 hammad     (501) staff       (20)      961 2023-07-13 23:36:16.000000 chroma_migrate-0.0.5/test_scripts/generate_test_clickhouse.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1008 2023-07-13 21:49:24.000000 chroma_migrate-0.0.5/test_scripts/generate_test_duckdb.py
```

### Comparing `chroma_migrate-0.0.4/.gitignore` & `chroma_migrate-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/LICENSE` & `chroma_migrate-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/PKG-INFO` & `chroma_migrate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma_migrate
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for migrating to chroma versions >= 0.4.0
 Author-email: Jeff Huber <jeff@trychroma.com>, Hammad Bashir <hammad@trychroma.com>
 Keywords: chroma,migrate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `chroma_migrate-0.0.4/README.md` & `chroma_migrate-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/chroma_migrate/cli.py` & `chroma_migrate-0.0.5/chroma_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/chroma_migrate/import_chromadb.py` & `chroma_migrate-0.0.5/chroma_migrate/import_chromadb.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/chroma_migrate/import_clickhouse.py` & `chroma_migrate-0.0.5/chroma_migrate/import_clickhouse.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/chroma_migrate/import_duckdb.py` & `chroma_migrate-0.0.5/chroma_migrate/import_duckdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,15 +61,21 @@
 
     # Read the embeddings from duckdb
     embeddings = conn.execute("SELECT uuid, collection_uuid, id, embedding, document, metadata FROM embeddings").fetch_df()
 
     # Add the embeddings to the collections
     for record in tqdm(embeddings.itertuples(index=False), total=embeddings.shape[0]):
         uuid, collection_uuid, id, embedding, document, metadata = record
-        metadata = json.loads(metadata)
+        if isinstance(metadata, str):
+            try:
+                metadata = json.loads(metadata)
+            except Exception as e:
+                print(f"Failed to load metadata for embedding {id} in collection {collection_uuid}. Malformed JSON")
+        else:
+            metadata = None
         metadata = migrate_embedding_metadata(metadata)
         collection = collection_uuid_to_chroma_collection[collection_uuid]
         collection.add(id, embedding, metadata, document)
 
     print(f"Migrated {len(collections)} collections and {embeddings.shape[0]} embeddings")
```

### Comparing `chroma_migrate-0.0.4/chroma_migrate/utils.py` & `chroma_migrate-0.0.5/chroma_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/chroma_migrate.egg-info/PKG-INFO` & `chroma_migrate-0.0.5/chroma_migrate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chroma-migrate
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for migrating to chroma versions >= 0.4.0
 Author-email: Jeff Huber <jeff@trychroma.com>, Hammad Bashir <hammad@trychroma.com>
 Keywords: chroma,migrate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `chroma_migrate-0.0.4/chroma_migrate.egg-info/SOURCES.txt` & `chroma_migrate-0.0.5/chroma_migrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/examples/from_chroma.py` & `chroma_migrate-0.0.5/examples/from_chroma.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/pyproject.toml` & `chroma_migrate-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/chroma-collections.parquet` & `chroma_migrate-0.0.5/test_data_duckdb/chroma-collections.parquet`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/chroma-embeddings.parquet` & `chroma_migrate-0.0.5/test_data_duckdb/chroma-embeddings.parquet`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/id_to_uuid_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_6c666f15-6c80-4a18-b955-5b4da3e25d77.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_71c07377-67be-4e5d-9270-2c71ec881f59.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_e13ac20a-0baa-47e7-a9ef-87280069d2d2.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_e7bb06ac-f659-4389-9e11-e9730efeca85.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_e8170c78-f675-4f1a-ab37-0dc436d64257.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_f29adc7f-4178-4c82-8fb2-1ae513520fe8.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin` & `chroma_migrate-0.0.5/test_data_duckdb/index/index_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.bin`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_3eccf5ff-7ecb-4312-940f-7f93b64b3c9c.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_6c666f15-6c80-4a18-b955-5b4da3e25d77.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_89b468b4-1082-40d6-a057-fe4ab2e2bcc7.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e13ac20a-0baa-47e7-a9ef-87280069d2d2.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e3eeb25a-6b54-4efc-885e-1be28f1e4c94.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e7bb06ac-f659-4389-9e11-e9730efeca85.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_e8170c78-f675-4f1a-ab37-0dc436d64257.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl` & `chroma_migrate-0.0.5/test_data_duckdb/index/uuid_to_id_f97e7bdb-bf55-4ecb-afb0-f7f96456068d.pkl`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_scripts/generate_test_clickhouse.py` & `chroma_migrate-0.0.5/test_scripts/generate_test_clickhouse.py`

 * *Files identical despite different names*

### Comparing `chroma_migrate-0.0.4/test_scripts/generate_test_duckdb.py` & `chroma_migrate-0.0.5/test_scripts/generate_test_duckdb.py`

 * *Files identical despite different names*

