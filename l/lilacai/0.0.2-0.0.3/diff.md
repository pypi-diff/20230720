# Comparing `tmp/lilacai-0.0.2.tar.gz` & `tmp/lilacai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilacai-0.0.2.tar", max compression
+gzip compressed data, was "lilacai-0.0.3.tar", max compression
```

## Comparing `lilacai-0.0.2.tar` & `lilacai-0.0.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.2/LICENSE
--rw-r--r--   0        0        0     4677 2023-07-17 18:14:48.513406 lilacai-0.0.2/README.md
--rw-r--r--   0        0        0     5623 2023-07-20 18:37:25.884635 lilacai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     1497 2023-07-19 23:03:22.224756 lilacai-0.0.2/src/auth.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.2/src/concepts/__init__.py
--rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.2/src/concepts/concept.py
--rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.2/src/concepts/concept_test.py
--rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.2/src/concepts/db_concept.py
--rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.2/src/concepts/db_concept_test.py
--rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.2/src/config.py
--rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.2/src/conftest.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.2/src/data/__init__.py
--rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.2/src/data/dataset.py
--rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.2/src/data/dataset_compute_signal_chain_test.py
--rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.2/src/data/dataset_compute_signal_test.py
--rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.2/src/data/dataset_duckdb.py
--rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.2/src/data/dataset_select_groups_test.py
--rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.2/src/data/dataset_select_rows_filter_test.py
--rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.2/src/data/dataset_select_rows_schema_test.py
--rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.2/src/data/dataset_select_rows_search_test.py
--rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.2/src/data/dataset_select_rows_sort_test.py
--rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.2/src/data/dataset_select_rows_udf_test.py
--rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.2/src/data/dataset_settings_test.py
--rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.2/src/data/dataset_stats_test.py
--rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.2/src/data/dataset_test.py
--rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.2/src/data/dataset_test_utils.py
--rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.2/src/data/dataset_utils.py
--rw-r--r--   0        0        0     3789 2023-07-17 19:50:29.960616 lilacai-0.0.2/src/data/dataset_utils_test.py
--rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.2/src/data/duckdb_utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.2/src/data/sources/__init__.py
--rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.2/src/data/sources/csv_source.py
--rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.2/src/data/sources/csv_source_test.py
--rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.2/src/data/sources/default_sources.py
--rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.2/src/data/sources/gmail_source.py
--rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.2/src/data/sources/huggingface_source.py
--rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.2/src/data/sources/huggingface_source_test.py
--rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.2/src/data/sources/json_source.py
--rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.2/src/data/sources/json_source_test.py
--rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.2/src/data/sources/pandas_source.py
--rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.2/src/data/sources/pandas_source_test.py
--rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.2/src/data/sources/reddit_hf_source.py
--rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.2/src/data/sources/source.py
--rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.2/src/data/sources/source_registry.py
--rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.2/src/data/sources/source_registry_test.py
--rw-r--r--   0        0        0     4518 2023-07-15 19:50:41.321817 lilacai-0.0.2/src/data_loader.py
--rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.2/src/data_loader_test.py
--rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.2/src/db_manager.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.2/src/embeddings/__init__.py
--rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.2/src/embeddings/cohere.py
--rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.2/src/embeddings/embedding.py
--rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.2/src/embeddings/embedding_test.py
--rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.2/src/embeddings/openai.py
--rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.2/src/embeddings/palm.py
--rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.2/src/embeddings/sbert.py
--rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.2/src/embeddings/vector_store.py
--rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.2/src/embeddings/vector_store_numpy.py
--rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.2/src/embeddings/vector_store_test.py
--rw-r--r--   0        0        0      769 2023-05-25 16:32:17.557576 lilacai-0.0.2/src/make_openapi.py
--rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.2/src/parquet_writer.py
--rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.2/src/router_concept.py
--rw-r--r--   0        0        0     2460 2023-07-19 23:03:22.228315 lilacai-0.0.2/src/router_data_loader.py
--rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.2/src/router_dataset.py
--rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.2/src/router_signal.py
--rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.2/src/router_tasks.py
--rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.2/src/router_utils.py
--rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.2/src/schema.py
--rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.2/src/schema_test.py
--rw-r--r--   0        0        0     4629 2023-07-19 23:03:22.228705 lilacai-0.0.2/src/server.py
--rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.2/src/server_concept_test.py
--rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.2/src/server_dataset_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.2/src/signals/__init__.py
--rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.2/src/signals/concept_labels.py
--rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.2/src/signals/concept_labels_test.py
--rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.2/src/signals/concept_scorer.py
--rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.2/src/signals/concept_scorer_test.py
--rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.2/src/signals/default_signals.py
--rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.2/src/signals/lang_detection.py
--rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.2/src/signals/lang_detection_test.py
--rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.2/src/signals/minhash_dup.py
--rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.2/src/signals/near_dup.py
--rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.2/src/signals/near_dup_test.py
--rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.2/src/signals/ner.py
--rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.2/src/signals/ner_test.py
--rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.2/src/signals/pii.py
--rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.2/src/signals/pii_ip_address.py
--rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.2/src/signals/pii_secrets.py
--rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.2/src/signals/pii_test.py
--rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.2/src/signals/semantic_similarity.py
--rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.2/src/signals/semantic_similarity_test.py
--rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.2/src/signals/signal.py
--rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.2/src/signals/signal_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.2/src/signals/splitters/__init__.py
--rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.2/src/signals/splitters/chunk_splitter.py
--rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.2/src/signals/splitters/chunk_splitter_test.py
--rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.2/src/signals/splitters/text_splitter_spacy.py
--rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.2/src/signals/splitters/text_splitter_spacy_test.py
--rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.2/src/signals/splitters/text_splitter_test_utils.py
--rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.2/src/signals/splitters/text_splitter_test_utils_test.py
--rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.2/src/signals/substring_search.py
--rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.2/src/signals/substring_search_test.py
--rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.2/src/signals/text_statistics.py
--rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.2/src/signals/text_statistics_test.py
--rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.2/src/tasks.py
--rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.2/src/test_utils.py
--rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.2/src/utils.py
--rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 lilacai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4677 2023-07-17 18:14:48.513406 lilacai-0.0.3/README.md
+-rw-r--r--   0        0        0     5618 2023-07-20 18:44:36.811954 lilacai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     1497 2023-07-19 23:03:22.224756 lilacai-0.0.3/src/auth.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.3/src/concepts/__init__.py
+-rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.3/src/concepts/concept.py
+-rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.3/src/concepts/concept_test.py
+-rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.3/src/concepts/db_concept.py
+-rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.3/src/concepts/db_concept_test.py
+-rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.3/src/config.py
+-rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.3/src/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.3/src/data/__init__.py
+-rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.3/src/data/dataset.py
+-rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.3/src/data/dataset_compute_signal_chain_test.py
+-rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.3/src/data/dataset_compute_signal_test.py
+-rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.3/src/data/dataset_duckdb.py
+-rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.3/src/data/dataset_select_groups_test.py
+-rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.3/src/data/dataset_select_rows_filter_test.py
+-rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.3/src/data/dataset_select_rows_schema_test.py
+-rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.3/src/data/dataset_select_rows_search_test.py
+-rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.3/src/data/dataset_select_rows_sort_test.py
+-rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.3/src/data/dataset_select_rows_udf_test.py
+-rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.3/src/data/dataset_settings_test.py
+-rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.3/src/data/dataset_stats_test.py
+-rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.3/src/data/dataset_test.py
+-rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.3/src/data/dataset_test_utils.py
+-rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.3/src/data/dataset_utils.py
+-rw-r--r--   0        0        0     3789 2023-07-17 19:50:29.960616 lilacai-0.0.3/src/data/dataset_utils_test.py
+-rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.3/src/data/duckdb_utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.3/src/data/sources/__init__.py
+-rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.3/src/data/sources/csv_source.py
+-rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.3/src/data/sources/csv_source_test.py
+-rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.3/src/data/sources/default_sources.py
+-rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.3/src/data/sources/gmail_source.py
+-rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.3/src/data/sources/huggingface_source.py
+-rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.3/src/data/sources/huggingface_source_test.py
+-rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.3/src/data/sources/json_source.py
+-rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.3/src/data/sources/json_source_test.py
+-rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.3/src/data/sources/pandas_source.py
+-rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.3/src/data/sources/pandas_source_test.py
+-rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.3/src/data/sources/reddit_hf_source.py
+-rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.3/src/data/sources/source.py
+-rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.3/src/data/sources/source_registry.py
+-rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.3/src/data/sources/source_registry_test.py
+-rw-r--r--   0        0        0     4518 2023-07-15 19:50:41.321817 lilacai-0.0.3/src/data_loader.py
+-rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.3/src/data_loader_test.py
+-rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.3/src/db_manager.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.3/src/embeddings/__init__.py
+-rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.3/src/embeddings/cohere.py
+-rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.3/src/embeddings/embedding.py
+-rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.3/src/embeddings/embedding_test.py
+-rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.3/src/embeddings/openai.py
+-rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.3/src/embeddings/palm.py
+-rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.3/src/embeddings/sbert.py
+-rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.3/src/embeddings/vector_store.py
+-rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.3/src/embeddings/vector_store_numpy.py
+-rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.3/src/embeddings/vector_store_test.py
+-rw-r--r--   0        0        0      769 2023-05-25 16:32:17.557576 lilacai-0.0.3/src/make_openapi.py
+-rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.3/src/parquet_writer.py
+-rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.3/src/router_concept.py
+-rw-r--r--   0        0        0     2460 2023-07-19 23:03:22.228315 lilacai-0.0.3/src/router_data_loader.py
+-rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.3/src/router_dataset.py
+-rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.3/src/router_signal.py
+-rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.3/src/router_tasks.py
+-rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.3/src/router_utils.py
+-rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.3/src/schema.py
+-rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.3/src/schema_test.py
+-rw-r--r--   0        0        0     4629 2023-07-19 23:03:22.228705 lilacai-0.0.3/src/server.py
+-rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.3/src/server_concept_test.py
+-rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.3/src/server_dataset_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.3/src/signals/__init__.py
+-rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.3/src/signals/concept_labels.py
+-rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.3/src/signals/concept_labels_test.py
+-rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.3/src/signals/concept_scorer.py
+-rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.3/src/signals/concept_scorer_test.py
+-rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.3/src/signals/default_signals.py
+-rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.3/src/signals/lang_detection.py
+-rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.3/src/signals/lang_detection_test.py
+-rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.3/src/signals/minhash_dup.py
+-rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.3/src/signals/near_dup.py
+-rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.3/src/signals/near_dup_test.py
+-rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.3/src/signals/ner.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.3/src/signals/ner_test.py
+-rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.3/src/signals/pii.py
+-rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.3/src/signals/pii_ip_address.py
+-rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.3/src/signals/pii_secrets.py
+-rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.3/src/signals/pii_test.py
+-rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.3/src/signals/semantic_similarity.py
+-rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.3/src/signals/semantic_similarity_test.py
+-rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.3/src/signals/signal.py
+-rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.3/src/signals/signal_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.3/src/signals/splitters/__init__.py
+-rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.3/src/signals/splitters/chunk_splitter.py
+-rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.3/src/signals/splitters/chunk_splitter_test.py
+-rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.3/src/signals/splitters/text_splitter_spacy.py
+-rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.3/src/signals/splitters/text_splitter_spacy_test.py
+-rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils.py
+-rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils_test.py
+-rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.3/src/signals/substring_search.py
+-rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.3/src/signals/substring_search_test.py
+-rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.3/src/signals/text_statistics.py
+-rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.3/src/signals/text_statistics_test.py
+-rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.3/src/tasks.py
+-rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.3/src/test_utils.py
+-rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.3/src/utils.py
+-rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 lilacai-0.0.3/PKG-INFO
```

### Comparing `lilacai-0.0.2/LICENSE` & `lilacai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/README.md` & `lilacai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/pyproject.toml` & `lilacai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Lilac AI Inc. <info@lilacml.com>"]
 description = "Organize unstructured data"
 name = "lilacai"
 packages = [{include = "src"}]
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 
 [tool.poetry.dependencies]
 
 ### Required dependencies. ###
 dask = "^2023.3.2" 
 datasets = "^2.12.0" 
 distributed = "^2023.3.2.1" 
@@ -22,15 +22,15 @@
 orjson = "^3.8.10" # Fast JSON serialization: https://fastapi.tiangolo.com/advanced/custom-response/#use-orjsonresponse
 pillow = "^9.3.0" # Image processing.
 psutil = "^5.9.5" 
 pyarrow = "^9.0.0" 
 pydantic = "^1.10.11" 
 python = ">=3.9,<4.0" 
 python-dotenv = "^1.0.0" 
-requests = "^2.28.1" 
+requests = "^2" 
 scikit-learn = "^1.3.0" 
 tenacity = "^8.2.2" 
 tqdm = "^4.65.0" 
 types-psutil = "^5.9.5.12" 
 typing-extensions = "^4.7.1" 
 uvicorn = {extras = ["standard"], version = "^0.22.0"}
```

### Comparing `lilacai-0.0.2/src/auth.py` & `lilacai-0.0.3/src/auth.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/concepts/concept.py` & `lilacai-0.0.3/src/concepts/concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/concepts/concept_test.py` & `lilacai-0.0.3/src/concepts/concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/concepts/db_concept.py` & `lilacai-0.0.3/src/concepts/db_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/concepts/db_concept_test.py` & `lilacai-0.0.3/src/concepts/db_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/config.py` & `lilacai-0.0.3/src/config.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/conftest.py` & `lilacai-0.0.3/src/conftest.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset.py` & `lilacai-0.0.3/src/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_compute_signal_chain_test.py` & `lilacai-0.0.3/src/data/dataset_compute_signal_chain_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_compute_signal_test.py` & `lilacai-0.0.3/src/data/dataset_compute_signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_duckdb.py` & `lilacai-0.0.3/src/data/dataset_duckdb.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_groups_test.py` & `lilacai-0.0.3/src/data/dataset_select_groups_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_rows_filter_test.py` & `lilacai-0.0.3/src/data/dataset_select_rows_filter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_rows_schema_test.py` & `lilacai-0.0.3/src/data/dataset_select_rows_schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_rows_search_test.py` & `lilacai-0.0.3/src/data/dataset_select_rows_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_rows_sort_test.py` & `lilacai-0.0.3/src/data/dataset_select_rows_sort_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_select_rows_udf_test.py` & `lilacai-0.0.3/src/data/dataset_select_rows_udf_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_settings_test.py` & `lilacai-0.0.3/src/data/dataset_settings_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_stats_test.py` & `lilacai-0.0.3/src/data/dataset_stats_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_test.py` & `lilacai-0.0.3/src/data/dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_test_utils.py` & `lilacai-0.0.3/src/data/dataset_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_utils.py` & `lilacai-0.0.3/src/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/dataset_utils_test.py` & `lilacai-0.0.3/src/data/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/duckdb_utils.py` & `lilacai-0.0.3/src/data/duckdb_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/csv_source.py` & `lilacai-0.0.3/src/data/sources/csv_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/csv_source_test.py` & `lilacai-0.0.3/src/data/sources/csv_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/default_sources.py` & `lilacai-0.0.3/src/data/sources/default_sources.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/gmail_source.py` & `lilacai-0.0.3/src/data/sources/gmail_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/huggingface_source.py` & `lilacai-0.0.3/src/data/sources/huggingface_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/huggingface_source_test.py` & `lilacai-0.0.3/src/data/sources/huggingface_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/json_source.py` & `lilacai-0.0.3/src/data/sources/json_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/json_source_test.py` & `lilacai-0.0.3/src/data/sources/json_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/pandas_source.py` & `lilacai-0.0.3/src/data/sources/pandas_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/pandas_source_test.py` & `lilacai-0.0.3/src/data/sources/pandas_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/reddit_hf_source.py` & `lilacai-0.0.3/src/data/sources/reddit_hf_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/source.py` & `lilacai-0.0.3/src/data/sources/source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/source_registry.py` & `lilacai-0.0.3/src/data/sources/source_registry.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data/sources/source_registry_test.py` & `lilacai-0.0.3/src/data/sources/source_registry_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data_loader.py` & `lilacai-0.0.3/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/data_loader_test.py` & `lilacai-0.0.3/src/data_loader_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/db_manager.py` & `lilacai-0.0.3/src/db_manager.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/cohere.py` & `lilacai-0.0.3/src/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/embedding.py` & `lilacai-0.0.3/src/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/embedding_test.py` & `lilacai-0.0.3/src/embeddings/embedding_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/openai.py` & `lilacai-0.0.3/src/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/palm.py` & `lilacai-0.0.3/src/embeddings/palm.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/sbert.py` & `lilacai-0.0.3/src/embeddings/sbert.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/vector_store.py` & `lilacai-0.0.3/src/embeddings/vector_store.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/vector_store_numpy.py` & `lilacai-0.0.3/src/embeddings/vector_store_numpy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/embeddings/vector_store_test.py` & `lilacai-0.0.3/src/embeddings/vector_store_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/make_openapi.py` & `lilacai-0.0.3/src/make_openapi.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/parquet_writer.py` & `lilacai-0.0.3/src/parquet_writer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/router_concept.py` & `lilacai-0.0.3/src/router_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/router_data_loader.py` & `lilacai-0.0.3/src/router_data_loader.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/router_dataset.py` & `lilacai-0.0.3/src/router_dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/router_signal.py` & `lilacai-0.0.3/src/router_signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/router_utils.py` & `lilacai-0.0.3/src/router_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/schema.py` & `lilacai-0.0.3/src/schema.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/schema_test.py` & `lilacai-0.0.3/src/schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/server.py` & `lilacai-0.0.3/src/server.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/server_concept_test.py` & `lilacai-0.0.3/src/server_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/server_dataset_test.py` & `lilacai-0.0.3/src/server_dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/concept_labels.py` & `lilacai-0.0.3/src/signals/concept_labels.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/concept_labels_test.py` & `lilacai-0.0.3/src/signals/concept_labels_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/concept_scorer.py` & `lilacai-0.0.3/src/signals/concept_scorer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/concept_scorer_test.py` & `lilacai-0.0.3/src/signals/concept_scorer_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/default_signals.py` & `lilacai-0.0.3/src/signals/default_signals.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/lang_detection.py` & `lilacai-0.0.3/src/signals/lang_detection.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/lang_detection_test.py` & `lilacai-0.0.3/src/signals/lang_detection_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/minhash_dup.py` & `lilacai-0.0.3/src/signals/minhash_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/near_dup.py` & `lilacai-0.0.3/src/signals/near_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/near_dup_test.py` & `lilacai-0.0.3/src/signals/near_dup_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/ner.py` & `lilacai-0.0.3/src/signals/ner.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/ner_test.py` & `lilacai-0.0.3/src/signals/ner_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/pii.py` & `lilacai-0.0.3/src/signals/pii.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/pii_ip_address.py` & `lilacai-0.0.3/src/signals/pii_ip_address.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/pii_secrets.py` & `lilacai-0.0.3/src/signals/pii_secrets.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/pii_test.py` & `lilacai-0.0.3/src/signals/pii_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/semantic_similarity.py` & `lilacai-0.0.3/src/signals/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/semantic_similarity_test.py` & `lilacai-0.0.3/src/signals/semantic_similarity_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/signal.py` & `lilacai-0.0.3/src/signals/signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/signal_test.py` & `lilacai-0.0.3/src/signals/signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/splitters/chunk_splitter.py` & `lilacai-0.0.3/src/signals/splitters/chunk_splitter.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/splitters/chunk_splitter_test.py` & `lilacai-0.0.3/src/signals/splitters/chunk_splitter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/splitters/text_splitter_spacy.py` & `lilacai-0.0.3/src/signals/splitters/text_splitter_spacy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/splitters/text_splitter_spacy_test.py` & `lilacai-0.0.3/src/signals/splitters/text_splitter_spacy_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/splitters/text_splitter_test_utils.py` & `lilacai-0.0.3/src/signals/splitters/text_splitter_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/substring_search.py` & `lilacai-0.0.3/src/signals/substring_search.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/substring_search_test.py` & `lilacai-0.0.3/src/signals/substring_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/text_statistics.py` & `lilacai-0.0.3/src/signals/text_statistics.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/signals/text_statistics_test.py` & `lilacai-0.0.3/src/signals/text_statistics_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/tasks.py` & `lilacai-0.0.3/src/tasks.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/test_utils.py` & `lilacai-0.0.3/src/test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/src/utils.py` & `lilacai-0.0.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.2/PKG-INFO` & `lilacai-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilacai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Organize unstructured data
 Author: Lilac AI Inc.
 Author-email: info@lilacml.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,15 +40,15 @@
 Requires-Dist: orjson (>=3.8.10,<4.0.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyarrow (>=9.0.0,<10.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0) ; extra == "pii"
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2,<3)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all" or extra == "embeddings"
 Requires-Dist: spacy (>=3.5.1,<4.0.0) ; extra == "all" or extra == "signals" or extra == "ner" or extra == "text-stats"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: textacy (>=0.13.0,<0.14.0) ; extra == "all" or extra == "signals" or extra == "text-stats"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: types-psutil (>=5.9.5.12,<6.0.0.0)
```

