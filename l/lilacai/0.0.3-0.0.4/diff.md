# Comparing `tmp/lilacai-0.0.3.tar.gz` & `tmp/lilacai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilacai-0.0.3.tar", max compression
+gzip compressed data, was "lilacai-0.0.4.tar", max compression
```

## Comparing `lilacai-0.0.3.tar` & `lilacai-0.0.4.tar`

### file list

```diff
@@ -1,107 +1,222 @@
--rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.3/LICENSE
--rw-r--r--   0        0        0     4677 2023-07-17 18:14:48.513406 lilacai-0.0.3/README.md
--rw-r--r--   0        0        0     5618 2023-07-20 18:44:36.811954 lilacai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     1497 2023-07-19 23:03:22.224756 lilacai-0.0.3/src/auth.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.3/src/concepts/__init__.py
--rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.3/src/concepts/concept.py
--rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.3/src/concepts/concept_test.py
--rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.3/src/concepts/db_concept.py
--rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.3/src/concepts/db_concept_test.py
--rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.3/src/config.py
--rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.3/src/conftest.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.3/src/data/__init__.py
--rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.3/src/data/dataset.py
--rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.3/src/data/dataset_compute_signal_chain_test.py
--rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.3/src/data/dataset_compute_signal_test.py
--rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.3/src/data/dataset_duckdb.py
--rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.3/src/data/dataset_select_groups_test.py
--rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.3/src/data/dataset_select_rows_filter_test.py
--rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.3/src/data/dataset_select_rows_schema_test.py
--rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.3/src/data/dataset_select_rows_search_test.py
--rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.3/src/data/dataset_select_rows_sort_test.py
--rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.3/src/data/dataset_select_rows_udf_test.py
--rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.3/src/data/dataset_settings_test.py
--rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.3/src/data/dataset_stats_test.py
--rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.3/src/data/dataset_test.py
--rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.3/src/data/dataset_test_utils.py
--rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.3/src/data/dataset_utils.py
--rw-r--r--   0        0        0     3789 2023-07-17 19:50:29.960616 lilacai-0.0.3/src/data/dataset_utils_test.py
--rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.3/src/data/duckdb_utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.3/src/data/sources/__init__.py
--rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.3/src/data/sources/csv_source.py
--rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.3/src/data/sources/csv_source_test.py
--rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.3/src/data/sources/default_sources.py
--rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.3/src/data/sources/gmail_source.py
--rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.3/src/data/sources/huggingface_source.py
--rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.3/src/data/sources/huggingface_source_test.py
--rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.3/src/data/sources/json_source.py
--rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.3/src/data/sources/json_source_test.py
--rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.3/src/data/sources/pandas_source.py
--rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.3/src/data/sources/pandas_source_test.py
--rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.3/src/data/sources/reddit_hf_source.py
--rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.3/src/data/sources/source.py
--rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.3/src/data/sources/source_registry.py
--rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.3/src/data/sources/source_registry_test.py
--rw-r--r--   0        0        0     4518 2023-07-15 19:50:41.321817 lilacai-0.0.3/src/data_loader.py
--rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.3/src/data_loader_test.py
--rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.3/src/db_manager.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.3/src/embeddings/__init__.py
--rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.3/src/embeddings/cohere.py
--rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.3/src/embeddings/embedding.py
--rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.3/src/embeddings/embedding_test.py
--rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.3/src/embeddings/openai.py
--rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.3/src/embeddings/palm.py
--rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.3/src/embeddings/sbert.py
--rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.3/src/embeddings/vector_store.py
--rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.3/src/embeddings/vector_store_numpy.py
--rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.3/src/embeddings/vector_store_test.py
--rw-r--r--   0        0        0      769 2023-05-25 16:32:17.557576 lilacai-0.0.3/src/make_openapi.py
--rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.3/src/parquet_writer.py
--rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.3/src/router_concept.py
--rw-r--r--   0        0        0     2460 2023-07-19 23:03:22.228315 lilacai-0.0.3/src/router_data_loader.py
--rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.3/src/router_dataset.py
--rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.3/src/router_signal.py
--rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.3/src/router_tasks.py
--rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.3/src/router_utils.py
--rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.3/src/schema.py
--rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.3/src/schema_test.py
--rw-r--r--   0        0        0     4629 2023-07-19 23:03:22.228705 lilacai-0.0.3/src/server.py
--rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.3/src/server_concept_test.py
--rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.3/src/server_dataset_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.3/src/signals/__init__.py
--rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.3/src/signals/concept_labels.py
--rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.3/src/signals/concept_labels_test.py
--rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.3/src/signals/concept_scorer.py
--rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.3/src/signals/concept_scorer_test.py
--rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.3/src/signals/default_signals.py
--rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.3/src/signals/lang_detection.py
--rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.3/src/signals/lang_detection_test.py
--rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.3/src/signals/minhash_dup.py
--rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.3/src/signals/near_dup.py
--rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.3/src/signals/near_dup_test.py
--rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.3/src/signals/ner.py
--rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.3/src/signals/ner_test.py
--rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.3/src/signals/pii.py
--rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.3/src/signals/pii_ip_address.py
--rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.3/src/signals/pii_secrets.py
--rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.3/src/signals/pii_test.py
--rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.3/src/signals/semantic_similarity.py
--rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.3/src/signals/semantic_similarity_test.py
--rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.3/src/signals/signal.py
--rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.3/src/signals/signal_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.3/src/signals/splitters/__init__.py
--rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.3/src/signals/splitters/chunk_splitter.py
--rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.3/src/signals/splitters/chunk_splitter_test.py
--rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.3/src/signals/splitters/text_splitter_spacy.py
--rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.3/src/signals/splitters/text_splitter_spacy_test.py
--rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils.py
--rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils_test.py
--rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.3/src/signals/substring_search.py
--rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.3/src/signals/substring_search_test.py
--rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.3/src/signals/text_statistics.py
--rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.3/src/signals/text_statistics_test.py
--rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.3/src/tasks.py
--rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.3/src/test_utils.py
--rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.3/src/utils.py
--rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 lilacai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5378 2023-07-20 19:37:02.878837 lilacai-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.4/lilacai/__init__.py
+-rw-r--r--   0        0        0     1800 2023-07-20 19:37:02.879223 lilacai-0.0.4/lilacai/auth.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.4/lilacai/concepts/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-25 16:33:06.625432 lilacai-0.0.4/lilacai/concepts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    14978 2023-07-14 16:20:33.334816 lilacai-0.0.4/lilacai/concepts/__pycache__/concept.cpython-39.pyc
+-rw-r--r--   0        0        0     3741 2023-05-25 17:56:09.596012 lilacai-0.0.4/lilacai/concepts/__pycache__/concept_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3741 2023-06-29 20:36:35.530262 lilacai-0.0.4/lilacai/concepts/__pycache__/concept_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    14857 2023-07-13 13:55:47.960867 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept.cpython-39.pyc
+-rw-r--r--   0        0        0    26850 2023-06-29 18:31:03.929394 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    27675 2023-07-05 20:35:04.899345 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.4/lilacai/concepts/concept.py
+-rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.4/lilacai/concepts/concept_test.py
+-rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.4/lilacai/concepts/db_concept.py
+-rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.4/lilacai/concepts/db_concept_test.py
+-rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.4/lilacai/config.py
+-rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.4/lilacai/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.4/lilacai/data/__init__.py
+-rw-r--r--   0        0        0      138 2023-05-25 16:33:22.229970 lilacai-0.0.4/lilacai/data/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1286 2023-05-25 17:38:50.204350 lilacai-0.0.4/lilacai/data/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    16829 2023-07-20 12:27:57.956385 lilacai-0.0.4/lilacai/data/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     9781 2023-06-09 14:17:45.871161 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_chain_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     9819 2023-07-19 23:03:24.128430 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_chain_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    20740 2023-06-22 15:45:21.847855 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    20448 2023-07-19 23:03:24.145583 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    49358 2023-07-20 12:27:58.774666 lilacai-0.0.4/lilacai/data/__pycache__/dataset_duckdb.cpython-39.pyc
+-rw-r--r--   0        0        0     8732 2023-06-22 15:45:21.858435 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_groups_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     9482 2023-07-20 12:24:55.916581 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_groups_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     4070 2023-05-30 23:23:49.738222 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_filter_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     6802 2023-06-30 16:45:10.244985 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_filter_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    17328 2023-06-20 15:48:54.176929 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_schema_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    17328 2023-07-15 00:14:43.016746 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_schema_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    11793 2023-06-25 13:04:36.821457 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_search_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    11783 2023-07-05 20:35:04.929716 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_search_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    20762 2023-06-20 12:39:17.922849 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_sort_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    20955 2023-07-19 23:03:24.180529 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_sort_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    16029 2023-06-09 14:18:19.042372 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_udf_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    15916 2023-07-19 23:03:24.282234 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_udf_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2173 2023-07-18 17:21:20.479288 lilacai-0.0.4/lilacai/data/__pycache__/dataset_settings_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5621 2023-06-22 15:45:21.880636 lilacai-0.0.4/lilacai/data/__pycache__/dataset_stats_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7082 2023-07-20 12:24:55.947147 lilacai-0.0.4/lilacai/data/__pycache__/dataset_stats_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    21844 2023-06-20 15:48:54.211586 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    21673 2023-07-19 23:03:24.308993 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     4366 2023-07-20 12:27:59.227750 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    12560 2023-07-19 23:03:42.331879 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     4223 2023-05-30 23:23:49.825084 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7484 2023-07-20 19:55:49.769644 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0      960 2023-07-05 20:36:01.119393 lilacai-0.0.4/lilacai/data/__pycache__/duckdb_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.4/lilacai/data/dataset.py
+-rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.4/lilacai/data/dataset_compute_signal_chain_test.py
+-rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.4/lilacai/data/dataset_compute_signal_test.py
+-rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.4/lilacai/data/dataset_duckdb.py
+-rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.4/lilacai/data/dataset_select_groups_test.py
+-rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.4/lilacai/data/dataset_select_rows_filter_test.py
+-rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.4/lilacai/data/dataset_select_rows_schema_test.py
+-rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.4/lilacai/data/dataset_select_rows_search_test.py
+-rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.4/lilacai/data/dataset_select_rows_sort_test.py
+-rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.4/lilacai/data/dataset_select_rows_udf_test.py
+-rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.4/lilacai/data/dataset_settings_test.py
+-rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.4/lilacai/data/dataset_stats_test.py
+-rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.4/lilacai/data/dataset_test.py
+-rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.4/lilacai/data/dataset_test_utils.py
+-rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.4/lilacai/data/dataset_utils.py
+-rw-r--r--   0        0        0     3790 2023-07-20 19:55:47.509593 lilacai-0.0.4/lilacai/data/dataset_utils_test.py
+-rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.4/lilacai/data/duckdb_utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.4/lilacai/data/sources/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-25 16:33:22.230251 lilacai-0.0.4/lilacai/data/sources/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2948 2023-07-14 14:31:43.463140 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source.cpython-39.pyc
+-rw-r--r--   0        0        0     2147 2023-06-20 12:39:17.946669 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2147 2023-06-29 20:36:35.832119 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0      825 2023-06-06 15:27:08.044491 lilacai-0.0.4/lilacai/data/sources/__pycache__/default_sources.cpython-39.pyc
+-rw-r--r--   0        0        0     6891 2023-07-20 18:27:24.388906 lilacai-0.0.4/lilacai/data/sources/__pycache__/gmail_source.cpython-39.pyc
+-rw-r--r--   0        0        0     5156 2023-06-27 20:41:56.561276 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source.cpython-39.pyc
+-rw-r--r--   0        0        0     4478 2023-06-20 12:39:17.951391 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4478 2023-06-29 20:36:35.836672 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2382 2023-06-30 16:45:08.555862 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source.cpython-39.pyc
+-rw-r--r--   0        0        0     3354 2023-06-20 12:39:17.955342 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3354 2023-06-29 20:36:35.839834 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1991 2023-06-20 12:39:15.981892 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source.cpython-39.pyc
+-rw-r--r--   0        0        0     2786 2023-06-20 12:39:17.958635 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2786 2023-06-29 20:36:35.842951 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1981 2023-06-20 12:39:15.983117 lilacai-0.0.4/lilacai/data/sources/__pycache__/reddit_hf_source.cpython-39.pyc
+-rw-r--r--   0        0        0     4008 2023-06-30 16:45:08.343946 lilacai-0.0.4/lilacai/data/sources/__pycache__/source.cpython-39.pyc
+-rw-r--r--   0        0        0     1653 2023-05-25 16:33:43.625612 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry.cpython-39.pyc
+-rw-r--r--   0        0        0     3233 2023-06-20 12:39:17.961608 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3233 2023-06-29 20:36:35.845613 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     6975 2023-05-26 15:29:09.387029 lilacai-0.0.4/lilacai/data/sources/__pycache__/tfds_source.cpython-39.pyc
+-rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.4/lilacai/data/sources/csv_source.py
+-rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.4/lilacai/data/sources/csv_source_test.py
+-rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.4/lilacai/data/sources/default_sources.py
+-rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.4/lilacai/data/sources/gmail_source.py
+-rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.4/lilacai/data/sources/huggingface_source.py
+-rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.4/lilacai/data/sources/huggingface_source_test.py
+-rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.4/lilacai/data/sources/json_source.py
+-rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.4/lilacai/data/sources/json_source_test.py
+-rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.4/lilacai/data/sources/pandas_source.py
+-rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.4/lilacai/data/sources/pandas_source_test.py
+-rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.4/lilacai/data/sources/reddit_hf_source.py
+-rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.4/lilacai/data/sources/source.py
+-rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.4/lilacai/data/sources/source_registry.py
+-rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.4/lilacai/data/sources/source_registry_test.py
+-rw-r--r--   0        0        0     4522 2023-07-20 19:27:47.282556 lilacai-0.0.4/lilacai/data_loader.py
+-rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.4/lilacai/data_loader_test.py
+-rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.4/lilacai/db_manager.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.4/lilacai/embeddings/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-25 16:33:20.655912 lilacai-0.0.4/lilacai/embeddings/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2441 2023-07-20 18:27:24.660578 lilacai-0.0.4/lilacai/embeddings/__pycache__/cohere.cpython-39.pyc
+-rw-r--r--   0        0        0     3973 2023-07-14 16:20:33.697005 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding.cpython-39.pyc
+-rw-r--r--   0        0        0     4297 2023-06-19 15:55:32.925051 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     5238 2023-07-14 16:20:35.348301 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2955 2023-07-20 18:27:24.661645 lilacai-0.0.4/lilacai/embeddings/__pycache__/openai.cpython-39.pyc
+-rw-r--r--   0        0        0     2730 2023-07-20 18:27:24.667100 lilacai-0.0.4/lilacai/embeddings/__pycache__/palm.cpython-39.pyc
+-rw-r--r--   0        0        0     2560 2023-07-20 18:27:24.668638 lilacai-0.0.4/lilacai/embeddings/__pycache__/sbert.cpython-39.pyc
+-rw-r--r--   0        0        0     2097 2023-06-09 20:36:16.224765 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store.cpython-39.pyc
+-rw-r--r--   0        0        0     2983 2023-07-14 18:14:01.396374 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_numpy.cpython-39.pyc
+-rw-r--r--   0        0        0     5894 2023-06-09 20:45:02.896412 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     5894 2023-06-29 20:36:35.855642 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.4/lilacai/embeddings/cohere.py
+-rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.4/lilacai/embeddings/embedding.py
+-rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.4/lilacai/embeddings/embedding_test.py
+-rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.4/lilacai/embeddings/openai.py
+-rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.4/lilacai/embeddings/palm.py
+-rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.4/lilacai/embeddings/sbert.py
+-rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.4/lilacai/embeddings/vector_store.py
+-rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.4/lilacai/embeddings/vector_store_numpy.py
+-rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.4/lilacai/embeddings/vector_store_test.py
+-rw-r--r--   0        0        0      768 2023-07-20 19:28:06.306494 lilacai-0.0.4/lilacai/make_openapi.py
+-rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.4/lilacai/parquet_writer.py
+-rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.4/lilacai/router_concept.py
+-rw-r--r--   0        0        0     2464 2023-07-20 19:28:16.506968 lilacai-0.0.4/lilacai/router_data_loader.py
+-rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.4/lilacai/router_dataset.py
+-rw-r--r--   0        0        0     2142 2023-07-20 19:37:02.879424 lilacai-0.0.4/lilacai/router_google_login.py
+-rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.4/lilacai/router_signal.py
+-rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.4/lilacai/router_tasks.py
+-rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.4/lilacai/router_utils.py
+-rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.4/lilacai/schema.py
+-rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.4/lilacai/schema_test.py
+-rw-r--r--   0        0        0     5640 2023-07-20 19:37:02.879793 lilacai-0.0.4/lilacai/server.py
+-rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.4/lilacai/server_concept_test.py
+-rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.4/lilacai/server_dataset_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.4/lilacai/signals/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-25 16:33:21.312087 lilacai-0.0.4/lilacai/signals/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2538 2023-07-10 19:43:01.845713 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels.cpython-39.pyc
+-rw-r--r--   0        0        0     5338 2023-06-20 12:39:17.971321 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     5338 2023-06-29 20:36:35.861540 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3457 2023-07-15 00:15:39.697437 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer.cpython-39.pyc
+-rw-r--r--   0        0        0    12587 2023-06-20 12:39:17.981373 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    13294 2023-07-13 13:55:52.375098 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1135 2023-07-19 12:31:05.301162 lilacai-0.0.4/lilacai/signals/__pycache__/default_signals.cpython-39.pyc
+-rw-r--r--   0        0        0     2268 2023-07-20 18:27:22.466894 lilacai-0.0.4/lilacai/signals/__pycache__/lang_detection.cpython-39.pyc
+-rw-r--r--   0        0        0     1661 2023-07-20 18:27:22.465620 lilacai-0.0.4/lilacai/signals/__pycache__/lang_detection_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     7666 2023-07-18 17:21:19.902763 lilacai-0.0.4/lilacai/signals/__pycache__/minhash_dup.cpython-39.pyc
+-rw-r--r--   0        0        0     1865 2023-07-18 17:21:19.901110 lilacai-0.0.4/lilacai/signals/__pycache__/near_dup.cpython-39.pyc
+-rw-r--r--   0        0        0     2161 2023-07-18 17:21:20.505848 lilacai-0.0.4/lilacai/signals/__pycache__/near_dup_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2515 2023-07-20 18:27:22.470411 lilacai-0.0.4/lilacai/signals/__pycache__/ner.cpython-39.pyc
+-rw-r--r--   0        0        0     2080 2023-07-06 19:35:08.489259 lilacai-0.0.4/lilacai/signals/__pycache__/ner_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2515 2023-07-20 18:27:22.472352 lilacai-0.0.4/lilacai/signals/__pycache__/pii.cpython-39.pyc
+-rw-r--r--   0        0        0     3576 2023-07-20 15:05:48.248628 lilacai-0.0.4/lilacai/signals/__pycache__/pii_ip_address.cpython-39.pyc
+-rw-r--r--   0        0        0     3670 2023-07-20 15:06:14.959294 lilacai-0.0.4/lilacai/signals/__pycache__/pii_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2360 2023-05-31 19:20:42.595460 lilacai-0.0.4/lilacai/signals/__pycache__/pii_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3286 2023-07-17 16:27:30.928786 lilacai-0.0.4/lilacai/signals/__pycache__/pii_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2845 2023-05-25 17:54:37.709786 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_search.cpython-39.pyc
+-rw-r--r--   0        0        0     4418 2023-05-25 17:54:41.434136 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_search_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3472 2023-06-09 15:06:25.513033 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity.cpython-39.pyc
+-rw-r--r--   0        0        0     4598 2023-06-09 14:18:55.738564 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4598 2023-06-29 20:36:35.879375 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0    11402 2023-07-15 00:15:45.703610 lilacai-0.0.4/lilacai/signals/__pycache__/signal.cpython-39.pyc
+-rw-r--r--   0        0        0     8825 2023-06-01 14:18:45.547562 lilacai-0.0.4/lilacai/signals/__pycache__/signal_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     8825 2023-06-29 20:36:35.885373 lilacai-0.0.4/lilacai/signals/__pycache__/signal_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1876 2023-06-01 14:18:38.849669 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search.cpython-39.pyc
+-rw-r--r--   0        0        0     2129 2023-05-31 19:20:42.618860 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2129 2023-06-29 20:36:35.889481 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2781 2023-07-20 18:27:22.481788 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2023-06-20 12:39:17.996390 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2693 2023-06-29 20:36:35.891867 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.4/lilacai/signals/concept_labels.py
+-rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.4/lilacai/signals/concept_labels_test.py
+-rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.4/lilacai/signals/concept_scorer.py
+-rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.4/lilacai/signals/concept_scorer_test.py
+-rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.4/lilacai/signals/default_signals.py
+-rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.4/lilacai/signals/lang_detection.py
+-rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.4/lilacai/signals/lang_detection_test.py
+-rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.4/lilacai/signals/minhash_dup.py
+-rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.4/lilacai/signals/near_dup.py
+-rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.4/lilacai/signals/near_dup_test.py
+-rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.4/lilacai/signals/ner.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.4/lilacai/signals/ner_test.py
+-rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.4/lilacai/signals/pii.py
+-rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.4/lilacai/signals/pii_ip_address.py
+-rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.4/lilacai/signals/pii_secrets.py
+-rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.4/lilacai/signals/pii_test.py
+-rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.4/lilacai/signals/semantic_similarity.py
+-rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.4/lilacai/signals/semantic_similarity_test.py
+-rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.4/lilacai/signals/signal.py
+-rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.4/lilacai/signals/signal_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.4/lilacai/signals/splitters/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-25 16:33:51.092841 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5467 2023-06-19 15:55:31.667495 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter.cpython-39.pyc
+-rw-r--r--   0        0        0     3044 2023-05-29 23:27:31.978383 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3044 2023-06-29 20:36:35.895019 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2476 2023-07-20 18:27:22.487078 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy.cpython-39.pyc
+-rw-r--r--   0        0        0     2490 2023-05-25 17:38:57.381087 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2522 2023-07-20 18:27:22.486467 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1490 2023-07-06 19:35:08.490242 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1319 2023-05-25 17:38:57.382952 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils_test.cpython-39-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1319 2023-06-29 20:36:35.899964 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils_test.cpython-39-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter.py
+-rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter_test.py
+-rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy.py
+-rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy_test.py
+-rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils.py
+-rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils_test.py
+-rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.4/lilacai/signals/substring_search.py
+-rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.4/lilacai/signals/substring_search_test.py
+-rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.4/lilacai/signals/text_statistics.py
+-rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.4/lilacai/signals/text_statistics_test.py
+-rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.4/lilacai/tasks.py
+-rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.4/lilacai/test_utils.py
+-rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.4/lilacai/utils.py
+-rw-r--r--   0        0        0     5670 2023-07-20 20:06:39.642165 lilacai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8457 1970-01-01 00:00:00.000000 lilacai-0.0.4/PKG-INFO
```

### Comparing `lilacai-0.0.3/LICENSE` & `lilacai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/README.md` & `lilacai-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -77,14 +77,33 @@
 
 To run the docker image locally:
 
 ```sh
 docker run -p 5432:5432 lilac_blueprint
 ```
 
+#### Authentication
+
+Authentication is done via Google login. A Google Client token should be created
+from the Google API Console. Details can be found [here](https://developers.google.com/identity/protocols/oauth2).
+
+By default, the Lilac google client is used. The secret can be found in Google
+Cloud console, and should be defined under `GOOGLE_CLIENT_SECRET` in .env.local.
+
+For the session middleware, a random string should be created and defined as `LILAC_OAUTH_SECRET_KEY` in .env.local.
+
+You can generate a random secret key with:
+
+```py
+import string
+import random
+key = ''.join(random.choices(string.ascii_uppercase + string.digits, k=64))
+print(f"LILAC_OAUTH_SECRET_KEY='{key}'")
+```
+
 ### Configuration
 
 To use various API's, API keys need to be provided. Create a file named `.env.local` in the root, and add variables that are listed in `.env` with your own values.
 
 #### Testing
 
 Run all the checks before mailing:
@@ -106,15 +125,15 @@
 ```
 
 ### Ingesting datasets from CLI
 
 Datasets can be ingested entirely from the UI, however if you prefer to use the CLI you can ingest data with the following command:
 
 ```sh
-poetry run python -m src.data_loader \
+poetry run python -m lilacai.data_loader \
   --dataset_name=$DATASET \
   --output_dir=./data/ \
   --config_path=./datasets/the_movies_dataset.json
 ```
 
 NOTE: You have to have a JSON file that represents your sour configuration, in this case
 "the_movies_dataset.json".
```

### Comparing `lilacai-0.0.3/pyproject.toml` & `lilacai-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 [tool.poetry]
 authors = ["Lilac AI Inc. <info@lilacml.com>"]
 description = "Organize unstructured data"
+license = "Apache-2.0"
 name = "lilacai"
-packages = [{include = "src"}]
+packages = [{include = "lilacai"}]
 readme = "README.md"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 
 ### Required dependencies. ###
-dask = "^2023.3.2" 
-datasets = "^2.12.0" 
-distributed = "^2023.3.2.1" 
-duckdb = "^0.8.1" 
-fastapi = "^0.98.0" 
-gcsfs = "^2023.4.0" 
-google-cloud-storage = "^2.5.0" 
-gunicorn = "^20.1.0" 
-joblib = "^1.3.1" 
+authlib = "^1.2.1"
+dask = "^2023.3.2"
+datasets = "^2.12.0"
+distributed = "^2023.3.2.1"
+duckdb = "^0.8.1"
+fastapi = "^0.98.0"
+gcsfs = "^2023.4.0"
+google-cloud-storage = "^2.5.0"
+gunicorn = "^20.1.0"
+httpx = "^0.24.1"
+itsdangerous = "^2.1.2"
+joblib = "^1.3.1"
 openai-function-call = "^0.0.5" # Wraps OpenAI functions with Pydantic models.
 orjson = "^3.8.10" # Fast JSON serialization: https://fastapi.tiangolo.com/advanced/custom-response/#use-orjsonresponse
 pillow = "^9.3.0" # Image processing.
-psutil = "^5.9.5" 
-pyarrow = "^9.0.0" 
-pydantic = "^1.10.11" 
-python = ">=3.9,<4.0" 
-python-dotenv = "^1.0.0" 
-requests = "^2" 
-scikit-learn = "^1.3.0" 
-tenacity = "^8.2.2" 
-tqdm = "^4.65.0" 
-types-psutil = "^5.9.5.12" 
-typing-extensions = "^4.7.1" 
-uvicorn = {extras = ["standard"], version = "^0.22.0"} 
+psutil = "^5.9.5"
+pyarrow = "^9.0.0"
+pydantic = "^1.10.11"
+python = ">=3.9,<4.0"
+python-dotenv = "^1.0.0"
+requests = "^2"
+scikit-learn = "^1.3.0"
+tenacity = "^8.2.2"
+tqdm = "^4.65.0"
+types-psutil = "^5.9.5.12"
+typing-extensions = "^4.7.1"
+uvicorn = {extras = ["standard"], version = "^0.22.0"}
 
 ### Optional dependencies. ###
 
 # LLM providers.
 cohere = {version = "^3.7.0", optional = true}
 google-generativeai = {version = "^0.1.0", optional = true}# PaLM / MakerSuite.
 openai = {version = "^0.27.8", optional = true}
@@ -93,55 +97,55 @@
 text_stats = ["textacy", "spacy"] # Text statistics.
 
 [tool.poetry.group.dev] # Deps for development.
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 bokeh = ">=2.4.2,<3" # Required for Dask monitoring.
-click = "^8.1.3" 
-google-api-python-client-stubs = "^1.13.0" 
-httpx = "^0.24.0" 
-huggingface-hub = "^0.15.1" 
-isort = "^5.12.0" 
-matplotlib = "^3.7.1" 
-mypy = "^1.0.0" 
-notebook = "^6.5.4" 
-pytest = "^7.1.3" 
-pytest-asyncio = "^0.20.2" 
-pytest-cov = "^4.0.0" 
-pytest-mock = "^3.10.0" 
-ruff = "^0.0.219" 
-setuptools = "^65.5.0" 
-toml = "^0.10.2" 
-types-Pillow = "^9.3.0.4" 
-types-cachetools = "^5.3.0.5" 
-types-regex = "^2023.6.3.0" 
-types-requests = "^2.28.11.5" 
-types-tqdm = "^4.65.0.0" 
-watchdog = {extras = ["watchmedo"], version = "^3.0.0"} 
-wheel = "^0.37.1" 
-yapf = "^0.32.0" 
+click = "^8.1.3"
+google-api-python-client-stubs = "^1.13.0"
+httpx = "^0.24.0"
+huggingface-hub = "^0.15.1"
+isort = "^5.12.0"
+matplotlib = "^3.7.1"
+mypy = "^1.0.0"
+notebook = "^6.5.4"
+pytest = "^7.1.3"
+pytest-asyncio = "^0.20.2"
+pytest-cov = "^4.0.0"
+pytest-mock = "^3.10.0"
+ruff = "^0.0.219"
+setuptools = "^65.5.0"
+toml = "^0.10.2"
+types-Pillow = "^9.3.0.4"
+types-cachetools = "^5.3.0.5"
+types-regex = "^2023.6.3.0"
+types-requests = "^2.28.11.5"
+types-tqdm = "^4.65.0.0"
+watchdog = {extras = ["watchmedo"], version = "^3.0.0"}
+wheel = "^0.37.1"
+yapf = "^0.32.0"
 
 [tool.poetry.scripts]
 deploy-hf = "scripts.deploy_hf:main"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.pyright]
 exclude = [
   "**/node_modules",
   "**/__pycache__",
 ]
-include = ["src"]
+include = ["lilacai"]
 
 [tool.ruff]
 line-length = 100
-src = ["src"]
+src = ["lilacai"]
 
 # Enable Pyflakes `F`, pycodestyle "W" and `E`, "Q" quotes, "I" imports.
 fix = true
 ignore = [
   "D105", # Missing docstring in magic method.
   "D106", # Missing docstring in a public nested class.
   "D107", # Missing docstring in __init__.
```

### Comparing `lilacai-0.0.3/src/auth.py` & `lilacai-0.0.4/lilacai/auth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Authentication and ACL configuration."""
 
+from typing import Optional
+
 from pydantic import BaseModel
 
 from .config import CONFIG
 
 
 class DatasetUserAccess(BaseModel):
   """User access for datasets."""
@@ -28,14 +30,29 @@
   create_dataset: bool
 
   # TODO(nsthorat): Make this keyed to each dataset and concept.
   dataset: DatasetUserAccess
   concept: ConceptUserAccess
 
 
+class UserInfo(BaseModel):
+  """User information."""
+  email: str
+  name: str
+  given_name: str
+  family_name: str
+
+
+class AuthenticationInfo(BaseModel):
+  """Authentication information for the user."""
+  user: Optional[UserInfo]
+  access: UserAccess
+  auth_enabled: bool
+
+
 def get_user_access() -> UserAccess:
   """Get the user access."""
   auth_enabled = CONFIG.get('LILAC_AUTH_ENABLED', False)
   if isinstance(auth_enabled, str):
     auth_enabled = auth_enabled.lower() == 'true'
   if auth_enabled:
     return UserAccess(
```

### Comparing `lilacai-0.0.3/src/concepts/concept.py` & `lilacai-0.0.4/lilacai/concepts/concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/concepts/concept_test.py` & `lilacai-0.0.4/lilacai/concepts/concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/concepts/db_concept.py` & `lilacai-0.0.4/lilacai/concepts/db_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/concepts/db_concept_test.py` & `lilacai-0.0.4/lilacai/concepts/db_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/config.py` & `lilacai-0.0.4/lilacai/config.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/conftest.py` & `lilacai-0.0.4/lilacai/conftest.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset.py` & `lilacai-0.0.4/lilacai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_compute_signal_chain_test.py` & `lilacai-0.0.4/lilacai/data/dataset_compute_signal_chain_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_compute_signal_test.py` & `lilacai-0.0.4/lilacai/data/dataset_compute_signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_duckdb.py` & `lilacai-0.0.4/lilacai/data/dataset_duckdb.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_groups_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_groups_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_rows_filter_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_rows_filter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_rows_schema_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_rows_schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_rows_search_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_rows_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_rows_sort_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_rows_sort_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_select_rows_udf_test.py` & `lilacai-0.0.4/lilacai/data/dataset_select_rows_udf_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_settings_test.py` & `lilacai-0.0.4/lilacai/data/dataset_settings_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_stats_test.py` & `lilacai-0.0.4/lilacai/data/dataset_stats_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_test.py` & `lilacai-0.0.4/lilacai/data/dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_test_utils.py` & `lilacai-0.0.4/lilacai/data/dataset_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_utils.py` & `lilacai-0.0.4/lilacai/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/dataset_utils_test.py` & `lilacai-0.0.4/lilacai/data/dataset_utils_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
   def func(xs: Iterable[int]) -> Iterable[int]:
     for x in xs:
       yield x + 1
 
   out = sparse_to_dense_compute(sparse_input, func)
   assert list(out) == [None, 2, 8, None, None, 4, None, 6, None, None]
 
+
 def test_sparse_to_dense_compute_batching() -> None:
   sparse_input = iter([None, 1, 7, None, None, 3, None, 5, None, None])
 
   def func(xs: Iterable[int]) -> Iterable[int]:
     for batch in chunks(xs, 2):
       yield batch[0] + 1
       if len(batch) > 1:
```

### Comparing `lilacai-0.0.3/src/data/duckdb_utils.py` & `lilacai-0.0.4/lilacai/data/duckdb_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/csv_source.py` & `lilacai-0.0.4/lilacai/data/sources/csv_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/csv_source_test.py` & `lilacai-0.0.4/lilacai/data/sources/csv_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/default_sources.py` & `lilacai-0.0.4/lilacai/data/sources/default_sources.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/gmail_source.py` & `lilacai-0.0.4/lilacai/data/sources/gmail_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/huggingface_source.py` & `lilacai-0.0.4/lilacai/data/sources/huggingface_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/huggingface_source_test.py` & `lilacai-0.0.4/lilacai/data/sources/huggingface_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/json_source.py` & `lilacai-0.0.4/lilacai/data/sources/json_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/json_source_test.py` & `lilacai-0.0.4/lilacai/data/sources/json_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/pandas_source.py` & `lilacai-0.0.4/lilacai/data/sources/pandas_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/pandas_source_test.py` & `lilacai-0.0.4/lilacai/data/sources/pandas_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/reddit_hf_source.py` & `lilacai-0.0.4/lilacai/data/sources/reddit_hf_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/source.py` & `lilacai-0.0.4/lilacai/data/sources/source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/source_registry.py` & `lilacai-0.0.4/lilacai/data/sources/source_registry.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data/sources/source_registry_test.py` & `lilacai-0.0.4/lilacai/data/sources/source_registry_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/data_loader.py` & `lilacai-0.0.4/lilacai/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A data loader standalone binary. This should only be run as a script to load a dataset.
 
 To run the source loader as a binary directly:
 
-poetry run python -m src.data_loader \
+poetry run python -m lilacai.data_loader \
   --dataset_name=movies_dataset \
   --output_dir=./data/ \
   --config_path=./datasets/the_movies_dataset.json
 """
 import json
 import math
 import os
```

### Comparing `lilacai-0.0.3/src/data_loader_test.py` & `lilacai-0.0.4/lilacai/data_loader_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/db_manager.py` & `lilacai-0.0.4/lilacai/db_manager.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/cohere.py` & `lilacai-0.0.4/lilacai/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/embedding.py` & `lilacai-0.0.4/lilacai/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/embedding_test.py` & `lilacai-0.0.4/lilacai/embeddings/embedding_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/openai.py` & `lilacai-0.0.4/lilacai/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/palm.py` & `lilacai-0.0.4/lilacai/embeddings/palm.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/sbert.py` & `lilacai-0.0.4/lilacai/embeddings/sbert.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/vector_store.py` & `lilacai-0.0.4/lilacai/embeddings/vector_store.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/vector_store_numpy.py` & `lilacai-0.0.4/lilacai/embeddings/vector_store_numpy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/embeddings/vector_store_test.py` & `lilacai-0.0.4/lilacai/embeddings/vector_store_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/make_openapi.py` & `lilacai-0.0.4/lilacai/make_openapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Writes the openapi.json file to the specified output.
 
-This is meant to run as a standalone script. It lives in src/ so that we can import the FastAPI app.
+This is meant to run as a standalone script. It lives in lilacai/ so we can import the FastAPI app.
 """
 import json
 
 import click
 from fastapi.openapi.utils import get_openapi
 
 from .server import app
```

### Comparing `lilacai-0.0.3/src/parquet_writer.py` & `lilacai-0.0.4/lilacai/parquet_writer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/router_concept.py` & `lilacai-0.0.4/lilacai/router_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/router_data_loader.py` & `lilacai-0.0.4/lilacai/router_data_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The source loader runner which loads data into parquet files for the app.
 
 To run the source loader as a binary directly:
 
-poetry run python -m src.datasets.loader \
+poetry run python -m lilacai.datasets.loader \
   --dataset_name=$DATASET \
   --output_dir=./data/ \
   --config_path=./datasets/the_movies_dataset.json
 """
 from typing import Any
 
 from fastapi import APIRouter, HTTPException, Request
```

### Comparing `lilacai-0.0.3/src/router_dataset.py` & `lilacai-0.0.4/lilacai/router_dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/router_signal.py` & `lilacai-0.0.4/lilacai/router_signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/router_utils.py` & `lilacai-0.0.4/lilacai/router_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/schema.py` & `lilacai-0.0.4/lilacai/schema.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/schema_test.py` & `lilacai-0.0.4/lilacai/schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/server.py` & `lilacai-0.0.4/lilacai/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """Serves the Lilac server."""
 
 import logging
 import os
 import shutil
 import subprocess
-from typing import Any
+from typing import Any, Optional
 
-from fastapi import APIRouter, FastAPI
+from fastapi import APIRouter, FastAPI, Request
 from fastapi.responses import FileResponse, ORJSONResponse
 from fastapi.routing import APIRoute
 from fastapi.staticfiles import StaticFiles
+from starlette.middleware.sessions import SessionMiddleware
 
-from . import router_concept, router_data_loader, router_dataset, router_signal, router_tasks
-from .auth import UserAccess, get_user_access
+from . import (
+  router_concept,
+  router_data_loader,
+  router_dataset,
+  router_google_login,
+  router_signal,
+  router_tasks,
+)
+from .auth import AuthenticationInfo, UserInfo, get_user_access
 from .concepts.db_concept import DiskConceptDB, get_concept_output_dir
 from .config import CONFIG, data_path
 from .router_utils import RouteErrorHandler
 from .tasks import task_manager
 from .utils import get_dataset_output_dir, list_datasets
 
 DIST_PATH = os.path.abspath(os.path.join('web', 'blueprint', 'build'))
+LILAC_AUTH_ENABLED = CONFIG.get('LILAC_AUTH_ENABLED', False)
+LILAC_OAUTH_SECRET_KEY = CONFIG.get('LILAC_OAUTH_SECRET_KEY', None)
+if LILAC_AUTH_ENABLED and not LILAC_OAUTH_SECRET_KEY:
+  raise ValueError('`LILAC_OAUTH_SECRET_KEY` must be set if `LILAC_AUTH_ENABLED` is True.')
 
 tags_metadata: list[dict[str, Any]] = [{
   'name': 'datasets',
   'description': 'API for querying a dataset.',
 }, {
   'name': 'concepts',
   'description': 'API for managing concepts.',
@@ -41,30 +53,43 @@
   return route.name
 
 
 app = FastAPI(
   default_response_class=ORJSONResponse,
   generate_unique_id_function=custom_generate_unique_id,
   openapi_tags=tags_metadata)
+app.add_middleware(SessionMiddleware, secret_key=LILAC_OAUTH_SECRET_KEY)
+app.include_router(router_google_login.router, prefix='/google', tags=['google_login'])
 
 v1_router = APIRouter(route_class=RouteErrorHandler)
 v1_router.include_router(router_dataset.router, prefix='/datasets', tags=['datasets'])
 v1_router.include_router(router_concept.router, prefix='/concepts', tags=['concepts'])
 v1_router.include_router(router_data_loader.router, prefix='/data_loaders', tags=['data_loaders'])
 v1_router.include_router(router_signal.router, prefix='/signals', tags=['signals'])
 v1_router.include_router(router_tasks.router, prefix='/tasks', tags=['tasks'])
 
 
-@v1_router.get('/acl')
-def user_acls() -> UserAccess:
+@app.get('/auth_info')
+def auth_info(request: Request) -> AuthenticationInfo:
   """Returns the user's ACLs.
 
   NOTE: Validation happens server-side as well. This is just used for UI treatment.
   """
-  return get_user_access()
+  user_info: Optional[UserInfo] = None
+  if LILAC_AUTH_ENABLED:
+    session_user = request.session.get('user', None)
+    if session_user:
+      user_info = UserInfo(
+        email=session_user['email'],
+        name=session_user['name'],
+        given_name=session_user['given_name'],
+        family_name=session_user['family_name'])
+
+  return AuthenticationInfo(
+    user=user_info, access=get_user_access(), auth_enabled=LILAC_AUTH_ENABLED)
 
 
 app.include_router(v1_router, prefix='/api/v1')
 
 
 @app.api_route('/{path_name}', include_in_schema=False)
 def catch_all() -> FileResponse:
```

### Comparing `lilacai-0.0.3/src/server_concept_test.py` & `lilacai-0.0.4/lilacai/server_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/server_dataset_test.py` & `lilacai-0.0.4/lilacai/server_dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/concept_labels.py` & `lilacai-0.0.4/lilacai/signals/concept_labels.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/concept_labels_test.py` & `lilacai-0.0.4/lilacai/signals/concept_labels_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/concept_scorer.py` & `lilacai-0.0.4/lilacai/signals/concept_scorer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/concept_scorer_test.py` & `lilacai-0.0.4/lilacai/signals/concept_scorer_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/default_signals.py` & `lilacai-0.0.4/lilacai/signals/default_signals.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/lang_detection.py` & `lilacai-0.0.4/lilacai/signals/lang_detection.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/lang_detection_test.py` & `lilacai-0.0.4/lilacai/signals/lang_detection_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/minhash_dup.py` & `lilacai-0.0.4/lilacai/signals/minhash_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/near_dup.py` & `lilacai-0.0.4/lilacai/signals/near_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/near_dup_test.py` & `lilacai-0.0.4/lilacai/signals/near_dup_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/ner.py` & `lilacai-0.0.4/lilacai/signals/ner.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/ner_test.py` & `lilacai-0.0.4/lilacai/signals/ner_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/pii.py` & `lilacai-0.0.4/lilacai/signals/pii.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/pii_ip_address.py` & `lilacai-0.0.4/lilacai/signals/pii_ip_address.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/pii_secrets.py` & `lilacai-0.0.4/lilacai/signals/pii_secrets.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/pii_test.py` & `lilacai-0.0.4/lilacai/signals/pii_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/semantic_similarity.py` & `lilacai-0.0.4/lilacai/signals/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/semantic_similarity_test.py` & `lilacai-0.0.4/lilacai/signals/semantic_similarity_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/signal.py` & `lilacai-0.0.4/lilacai/signals/signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/signal_test.py` & `lilacai-0.0.4/lilacai/signals/signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/splitters/chunk_splitter.py` & `lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/splitters/chunk_splitter_test.py` & `lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/splitters/text_splitter_spacy.py` & `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/splitters/text_splitter_spacy_test.py` & `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils.py` & `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/substring_search.py` & `lilacai-0.0.4/lilacai/signals/substring_search.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/substring_search_test.py` & `lilacai-0.0.4/lilacai/signals/substring_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/text_statistics.py` & `lilacai-0.0.4/lilacai/signals/text_statistics.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/signals/text_statistics_test.py` & `lilacai-0.0.4/lilacai/signals/text_statistics_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/tasks.py` & `lilacai-0.0.4/lilacai/tasks.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/test_utils.py` & `lilacai-0.0.4/lilacai/test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/src/utils.py` & `lilacai-0.0.4/lilacai/utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.3/PKG-INFO` & `lilacai-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: lilacai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Organize unstructured data
+License: Apache-2.0
 Author: Lilac AI Inc.
 Author-email: info@lilacml.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: embeddings
 Provides-Extra: gmail
 Provides-Extra: lang-detection
 Provides-Extra: llms
 Provides-Extra: ner
 Provides-Extra: pii
 Provides-Extra: signals
 Provides-Extra: text-stats
+Requires-Dist: authlib (>=1.2.1,<2.0.0)
 Requires-Dist: cohere (>=3.7.0,<4.0.0) ; extra == "all" or extra == "embeddings"
 Requires-Dist: dask (>=2023.3.2,<2024.0.0)
 Requires-Dist: datasets (>=2.12.0,<3.0.0)
 Requires-Dist: detect-secrets (>=1.4.0,<2.0.0) ; extra == "all" or extra == "signals" or extra == "pii"
 Requires-Dist: distributed (>=2023.3.2.1,<2024.0.0.0)
 Requires-Dist: duckdb (>=0.8.1,<0.9.0)
 Requires-Dist: email-reply-parser (>=0.5.12,<0.6.0) ; extra == "all" or extra == "gmail"
@@ -29,14 +32,16 @@
 Requires-Dist: gcsfs (>=2023.4.0,<2024.0.0)
 Requires-Dist: google-api-python-client (>=2.88.0,<3.0.0) ; extra == "all" or extra == "gmail"
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0) ; extra == "all" or extra == "gmail"
 Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0) ; extra == "all" or extra == "gmail"
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
 Requires-Dist: google-generativeai (>=0.1.0,<0.2.0) ; extra == "all" or extra == "embeddings"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
 Requires-Dist: joblib (>=1.3.1,<2.0.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0) ; extra == "all" or extra == "signals" or extra == "lang-detection"
 Requires-Dist: openai (>=0.27.8,<0.28.0) ; extra == "all" or extra == "embeddings" or extra == "llms"
 Requires-Dist: openai-function-call (>=0.0.5,<0.0.6)
 Requires-Dist: orjson (>=3.8.10,<4.0.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
@@ -135,14 +140,33 @@
 
 To run the docker image locally:
 
 ```sh
 docker run -p 5432:5432 lilac_blueprint
 ```
 
+#### Authentication
+
+Authentication is done via Google login. A Google Client token should be created
+from the Google API Console. Details can be found [here](https://developers.google.com/identity/protocols/oauth2).
+
+By default, the Lilac google client is used. The secret can be found in Google
+Cloud console, and should be defined under `GOOGLE_CLIENT_SECRET` in .env.local.
+
+For the session middleware, a random string should be created and defined as `LILAC_OAUTH_SECRET_KEY` in .env.local.
+
+You can generate a random secret key with:
+
+```py
+import string
+import random
+key = ''.join(random.choices(string.ascii_uppercase + string.digits, k=64))
+print(f"LILAC_OAUTH_SECRET_KEY='{key}'")
+```
+
 ### Configuration
 
 To use various API's, API keys need to be provided. Create a file named `.env.local` in the root, and add variables that are listed in `.env` with your own values.
 
 #### Testing
 
 Run all the checks before mailing:
@@ -164,15 +188,15 @@
 ```
 
 ### Ingesting datasets from CLI
 
 Datasets can be ingested entirely from the UI, however if you prefer to use the CLI you can ingest data with the following command:
 
 ```sh
-poetry run python -m src.data_loader \
+poetry run python -m lilacai.data_loader \
   --dataset_name=$DATASET \
   --output_dir=./data/ \
   --config_path=./datasets/the_movies_dataset.json
 ```
 
 NOTE: You have to have a JSON file that represents your sour configuration, in this case
 "the_movies_dataset.json".
```

