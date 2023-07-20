# Comparing `tmp/mezcla-1.3.9.1.tar.gz` & `tmp/mezcla-1.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.9.1.tar", last modified: Fri Jul  7 05:50:45 2023, max compression
+gzip compressed data, was "mezcla-1.3.9.2.tar", last modified: Thu Jul 20 19:27:33 2023, max compression
```

## Comparing `mezcla-1.3.9.1.tar` & `mezcla-1.3.9.2.tar`

### file list

```diff
@@ -1,166 +1,168 @@
--rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/.coveragerc
--rw-r--r--   0        0        0     1253 2023-07-04 06:24:29.977415 mezcla-1.3.9.1/.github/workflows/act.yml
--rw-r--r--   0        0        0     1138 2023-07-06 21:26:09.495920 mezcla-1.3.9.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1996 2023-07-05 22:24:53.748059 mezcla-1.3.9.1/.gitignore
--rw-r--r--   0        0        0     4950 2023-07-06 18:59:36.543927 mezcla-1.3.9.1/Dockerfile
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/LICENSE.txt
--rw-r--r--   0        0        0      777 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/README.txt
--rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/TODO.txt
--rw-r--r--   0        0        0      130 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/TODO.md
--rwxr-xr-x   0        0        0     2261 2023-07-06 23:03:45.553197 mezcla-1.3.9.1/mezcla/__init__.py
--rwxr-xr-x   0        0        0     1196 2023-07-06 23:04:24.377280 mezcla-1.3.9.1/mezcla/__main__.py
--rwxr-xr-x   0        0        0    10872 2023-07-01 01:05:14.785985 mezcla-1.3.9.1/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13025 2023-06-18 00:32:33.000000 mezcla-1.3.9.1/mezcla/audio.py
--rwxr-xr-x   0        0        0     4707 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.3.9.1/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25718 2023-07-01 01:12:47.735987 mezcla-1.3.9.1/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     9241 2023-06-29 05:58:21.372447 mezcla-1.3.9.1/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14284 2023-07-01 01:05:14.785985 mezcla-1.3.9.1/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0     3145 2023-07-02 23:54:56.761692 mezcla-1.3.9.1/mezcla/convert_emoticons.py
--rwxr-xr-x   0        0        0    22279 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/cut.py
--rwxr-xr-x   0        0        0     4307 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    49448 2023-07-06 18:32:47.183393 mezcla-1.3.9.1/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12874 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3644 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.3.9.1/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.3.9.1/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8811 2023-07-01 01:12:47.739987 mezcla-1.3.9.1/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    30001 2023-07-05 20:16:25.630128 mezcla-1.3.9.1/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3338 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3922 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.9.1/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.9.1/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.3.9.1/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    13004 2023-07-01 01:56:03.422567 mezcla-1.3.9.1/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     2068 2023-07-02 23:30:29.556473 mezcla-1.3.9.1/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     5070 2023-06-29 06:26:07.199936 mezcla-1.3.9.1/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     3617 2023-07-01 01:05:14.793985 mezcla-1.3.9.1/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     4031 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     7708 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.9.1/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32976 2023-07-01 21:43:17.040662 mezcla-1.3.9.1/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    33907 2023-07-06 18:39:58.553067 mezcla-1.3.9.1/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    35278 2023-07-05 20:22:18.399100 mezcla-1.3.9.1/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    46774 2023-07-02 23:33:30.418758 mezcla-1.3.9.1/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11648 2023-07-01 01:58:45.279182 mezcla-1.3.9.1/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9993 2023-07-02 23:34:27.331430 mezcla-1.3.9.1/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13776 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      737 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31508 2023-07-01 01:12:47.743987 mezcla-1.3.9.1/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7604 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.9.1/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.000000 mezcla-1.3.9.1/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19931 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3011 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.9.1/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    51914 2023-07-05 20:23:04.687235 mezcla-1.3.9.1/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5625 2023-07-02 23:50:24.908274 mezcla-1.3.9.1/mezcla/template.py
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/adhoc-tests.batspp
--rw-r--r--   0        0        0      204 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4836 2023-07-02 23:52:07.820771 mezcla-1.3.9.1/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     2489 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     4736 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0      834 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     1974 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_compute_tfidf.py
--rw-r--r--   0        0        0     3523 2023-07-02 23:26:56.041382 mezcla-1.3.9.1/mezcla/tests/test_convert_emoticons.py
--rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    16047 2023-07-01 02:00:52.582153 mezcla-1.3.9.1/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     1030 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     3449 2023-07-01 21:45:57.905414 mezcla-1.3.9.1/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15711 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0      892 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     2114 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8972 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2886 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0      916 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0      991 2023-07-01 01:12:47.747987 mezcla-1.3.9.1/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8297 2023-07-01 01:12:47.747987 mezcla-1.3.9.1/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1183 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0      854 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2873 2023-07-01 02:02:49.768496 mezcla-1.3.9.1/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0      916 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     2083 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33490 2023-07-04 06:33:21.263049 mezcla-1.3.9.1/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3714 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     7264 2023-04-30 22:47:21.000000 mezcla-1.3.9.1/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0      725 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0      686 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.3.9.1/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33820 2023-07-01 01:05:14.801984 mezcla-1.3.9.1/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    23204 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2023-04-30 22:44:00.000000 mezcla-1.3.9.1/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.000000 mezcla-1.3.9.1/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.000000 mezcla-1.3.9.1/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16168 2023-07-04 06:13:52.451491 mezcla-1.3.9.1/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59922 2023-07-01 01:05:14.805985 mezcla-1.3.9.1/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.9.1/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.9.1/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.9.1/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    13455 2023-07-02 23:53:11.409104 mezcla-1.3.9.1/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.9.1/mezcla/xml_utils.py
--rw-r--r--   0        0        0      753 2023-07-07 05:49:33.581744 mezcla-1.3.9.1/pyproject.toml
--rw-r--r--   0        0        0     2469 2023-07-01 05:11:48.148105 mezcla-1.3.9.1/requirements.txt
--rwxr-xr-x   0        0        0     1243 2023-07-06 23:03:45.553197 mezcla-1.3.9.1/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.3.9.1/temp/simple_batspp.py
--rw-r--r--   0        0        0      697 2023-07-01 19:46:38.387644 mezcla-1.3.9.1/tools/local-workflows.sh
--rwxr-xr-x   0        0        0      862 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.3.9.1/tox.ini
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 mezcla-1.3.9.1/PKG-INFO
+-rw-r--r--   0        0        0      542 2022-12-14 03:30:58.682619 mezcla-1.3.9.2/.coveragerc
+-rw-r--r--   0        0        0     1245 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/.github/workflows/act.yml
+-rw-r--r--   0        0        0     1138 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1996 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/.gitignore
+-rw-r--r--   0        0        0     4950 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/Dockerfile
+-rw-r--r--   0        0        0     7370 2022-12-14 03:30:58.682619 mezcla-1.3.9.2/LICENSE.txt
+-rw-r--r--   0        0        0      777 2022-12-14 03:30:58.682619 mezcla-1.3.9.2/README.txt
+-rw-r--r--   0        0        0      380 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/TODO.txt
+-rw-r--r--   0        0        0      130 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2292 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/__init__.py
+-rwxr-xr-x   0        0        0     1196 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/__main__.py
+-rwxr-xr-x   0        0        0    10872 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13025 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/audio.py
+-rwxr-xr-x   0        0        0     4707 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2022-12-14 03:30:58.686619 mezcla-1.3.9.2/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2022-12-14 03:30:58.686619 mezcla-1.3.9.2/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14284 2023-07-20 18:27:50.220562 mezcla-1.3.9.2/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     3145 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    22279 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4307 2023-04-30 22:12:05.681956 mezcla-1.3.9.2/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    49448 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-12-14 03:30:58.690619 mezcla-1.3.9.2/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    30001 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3338 2023-01-14 21:19:15.193369 mezcla-1.3.9.2/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-04-30 22:12:05.685956 mezcla-1.3.9.2/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    13004 2023-07-20 18:27:50.224562 mezcla-1.3.9.2/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2068 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     5070 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3617 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-04-30 22:12:05.685956 mezcla-1.3.9.2/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     7708 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2022-12-14 03:30:58.694619 mezcla-1.3.9.2/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    33907 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    35278 2023-07-20 18:27:50.228562 mezcla-1.3.9.2/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2022-12-14 03:30:58.698619 mezcla-1.3.9.2/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17844 2023-07-20 18:48:02.599951 mezcla-1.3.9.2/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    46774 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2022-12-14 03:30:58.698619 mezcla-1.3.9.2/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11648 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9993 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-04-30 22:12:05.689956 mezcla-1.3.9.2/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      737 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31508 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2022-12-22 20:10:10.050773 mezcla-1.3.9.2/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     3202 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/python_ast.py
+-rwxr-xr-x   0        0        0     7053 2022-12-14 03:30:58.702620 mezcla-1.3.9.2/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7604 2023-07-20 18:27:50.232562 mezcla-1.3.9.2/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2022-12-14 03:30:58.702620 mezcla-1.3.9.2/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2022-12-14 03:30:58.706620 mezcla-1.3.9.2/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2022-12-14 03:30:58.706620 mezcla-1.3.9.2/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2022-12-14 03:30:58.706620 mezcla-1.3.9.2/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-04-30 22:12:05.689956 mezcla-1.3.9.2/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-04-30 22:12:05.689956 mezcla-1.3.9.2/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2022-12-14 03:30:58.706620 mezcla-1.3.9.2/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    52665 2023-07-20 18:48:02.599951 mezcla-1.3.9.2/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2022-12-14 03:30:58.706620 mezcla-1.3.9.2/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5773 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      462 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1082 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/adhoc-tests.batspp
+-rw-r--r--   0        0        0      204 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      810 2023-04-30 22:12:05.705956 mezcla-1.3.9.2/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-04-30 22:12:05.693956 mezcla-1.3.9.2/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-04-30 22:12:05.693956 mezcla-1.3.9.2/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2022-12-14 03:30:58.710620 mezcla-1.3.9.2/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-04-30 22:12:05.693956 mezcla-1.3.9.2/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4831 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     2489 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     4736 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2022-12-22 20:10:10.054773 mezcla-1.3.9.2/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2022-12-22 20:10:10.054773 mezcla-1.3.9.2/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2022-12-22 20:10:10.054773 mezcla-1.3.9.2/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     3523 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-04-30 22:12:05.693956 mezcla-1.3.9.2/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-04-30 22:12:05.693956 mezcla-1.3.9.2/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    16047 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2022-12-22 20:10:10.054773 mezcla-1.3.9.2/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     3449 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15711 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2022-12-14 03:30:58.714620 mezcla-1.3.9.2/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2022-12-22 20:10:10.054773 mezcla-1.3.9.2/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     2114 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8972 2023-07-20 18:27:50.236562 mezcla-1.3.9.2/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2022-12-14 03:30:58.714620 mezcla-1.3.9.2/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2886 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      991 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8297 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0     2145 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_python_ast.py
+-rwxr-xr-x   0        0        0      854 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2873 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      916 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2083 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33490 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3714 2023-04-30 22:12:05.697956 mezcla-1.3.9.2/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7264 2023-04-30 22:12:05.697956 mezcla-1.3.9.2/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2022-12-22 20:10:10.058773 mezcla-1.3.9.2/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33820 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23204 2023-07-20 18:27:50.240563 mezcla-1.3.9.2/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2022-12-14 03:30:58.718620 mezcla-1.3.9.2/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2022-12-14 03:30:58.722621 mezcla-1.3.9.2/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16168 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59922 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2022-12-14 03:30:58.722621 mezcla-1.3.9.2/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2022-12-14 03:30:58.722621 mezcla-1.3.9.2/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2022-12-14 03:30:58.722621 mezcla-1.3.9.2/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    13455 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-12-14 03:30:58.722621 mezcla-1.3.9.2/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      753 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2489 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/requirements.txt
+-rwxr-xr-x   0        0        0     1243 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-12-14 03:30:58.726621 mezcla-1.3.9.2/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     1225 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0      862 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-07-20 18:27:50.244562 mezcla-1.3.9.2/tox.ini
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 mezcla-1.3.9.2/PKG-INFO
```

### Comparing `mezcla-1.3.9.1/.coveragerc` & `mezcla-1.3.9.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/.github/workflows/act.yml` & `mezcla-1.3.9.2/.github/workflows/act.yml`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,14 @@
       - name: Configure Environment
         run: |
           echo "PATH=$PATH" >> $GITHUB_ENV
           echo "PYTHONPATH=$PYTHONPATH:/usr/local/lib/python3.9/dist-packages" >> $GITHUB_ENV
 
       - name: Run Python Tests
         run: |
-          PYTHONPATH="$(pwd):$PYTHONPATH" python3 ./tools/run_tests.bash
+          PYTHONPATH="$(pwd):$PYTHONPATH" ./tools/run_tests.bash
 
       ## TODO:
       ## See https://github.com/tomasohara/shell-scripts/blob/main/tests/batspp_report.py
       ## - name: Run Bats-PP Alias Tests
       ##   run: |
       ##     PYTHONPATH="$(pwd):$PYTHONPATH" bash tests/summary_stats.bash
```

### Comparing `mezcla-1.3.9.1/.github/workflows/tests.yml` & `mezcla-1.3.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/.gitignore` & `mezcla-1.3.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/Dockerfile` & `mezcla-1.3.9.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/LICENSE.txt` & `mezcla-1.3.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/README.txt` & `mezcla-1.3.9.2/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/__init__.py` & `mezcla-1.3.9.2/mezcla/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.9.1'
+version = "1.3.9.2"
+__VERSION__ = version
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
@@ -51,15 +52,15 @@
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Constants
 TL = debug.TL
 
 # Expose commonly used modules
-__all__ = ["debug", "gh", "my_re", "system", "TL"]
+__all__ = ["debug", "gh", "my_re", "system", "TL", __VERSION__]
 
 ## OLD:
 ## if __name__ == '__main__':
 ##     debug.trace(TL.USUAL, f"Version: {__VERSION__}")
 ##     system.print_error(f"Warning: {__file__} is not intended to be run standalone\n")
 ## NOTE: See https://stackoverflow.com/questions/43393764/python-3-6-project-structure-leads-to-runtimewarning
 debug.trace(TL.DETAILED, f"mezcla version: {__VERSION__}")
```

### Comparing `mezcla-1.3.9.1/mezcla/__main__.py` & `mezcla-1.3.9.2/mezcla/__main__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/analyze_tfidf.py` & `mezcla-1.3.9.2/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/audio.py` & `mezcla-1.3.9.2/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/bash_ast.py` & `mezcla-1.3.9.2/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/bert_multi_classification.py` & `mezcla-1.3.9.2/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/bert_text_classification.py` & `mezcla-1.3.9.2/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/bing_search.py` & `mezcla-1.3.9.2/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/check_html_javascript.py` & `mezcla-1.3.9.2/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/compute_tfidf.py` & `mezcla-1.3.9.2/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/convert_emoticons.py` & `mezcla-1.3.9.2/mezcla/convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/cut.py` & `mezcla-1.3.9.2/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/data_utils.py` & `mezcla-1.3.9.2/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/debug.py` & `mezcla-1.3.9.2/mezcla/debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/docs/audio_uml.svg` & `mezcla-1.3.9.2/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.9.2/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.9.2/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.9.2/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/download_user_gist.py` & `mezcla-1.3.9.2/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.9.2/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.9.2/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/feature_importance.py` & `mezcla-1.3.9.2/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.9.2/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.3.9.2/mezcla/examples/hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.9.2/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.9.2/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.9.2/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/iris.csv` & `mezcla-1.3.9.2/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.9.2/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.9.2/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.9.2/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/template.py` & `mezcla-1.3.9.2/mezcla/examples/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.9.2/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.3.9.2/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.9.2/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/extract_document_text.py` & `mezcla-1.3.9.2/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/file_utils.py` & `mezcla-1.3.9.2/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/filter_random.py` & `mezcla-1.3.9.2/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/format_profile.py` & `mezcla-1.3.9.2/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/gensim_test.py` & `mezcla-1.3.9.2/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/glue_helpers.py` & `mezcla-1.3.9.2/mezcla/glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/html_utils.py` & `mezcla-1.3.9.2/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/kenlm_example.py` & `mezcla-1.3.9.2/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/keras_param_search.py` & `mezcla-1.3.9.2/mezcla/keras_param_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 ## TEST: try to set random number seed for TensorFlow (to get deterministic results)
 ## import numpy
 ## numpy.random.seed(7919)
 ## import tensorflow
 ## BAD: tensorflow.set_random_seed(7919)
 ## tensorflow.random.set_seed(7919)
 
-# Standard packages
+# Standard moduless
 import re
 import sys
 from collections import OrderedDict
 
-# Installed packages
+# Installed moduless
 # TODO: install kera dynamically???
 ## TEST: sys.stderr.write("here\n")
 ## BAD:
 from keras.models import Sequential
 ## See https://stackoverflow.com/questions/55496289/how-to-fix-attributeerror-module-tensorflow-has-no-attribute-get-default-gr
 ## TEST: from tensorflow.keras.models import Sequential
 
@@ -57,18 +57,19 @@
 from sklearn.model_selection import cross_val_score, GridSearchCV, KFold, RandomizedSearchCV
 from sklearn.preprocessing import LabelEncoder
 
 ## NOTE: This takes too long to load so postponed, in case usage just shown.
 ## OLD: import tensorflow as tf
 ## TEST: tf = None
 
-# Local packages
+# Local moduless
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla import system
+round3 = system.round3
 from mezcla import text_utils
 from mezcla.text_utils import getenv_ints
 
 # Note: python 3.6+ format strings are used
 assert((sys.version_info.major >= 3) and (sys.version_info.minor >= 6))
 
 #...............................................................................
@@ -113,18 +114,14 @@
 HIDDEN_UNIT_VARS = ["hidden_units{n}".format(n=(v + 1)) for v in range(MAX_HIDDEN_UNIT_VARS)]
 # note: DEFAULT_HIDDEN_UNITS is for use outside of grid search
 DEFAULT_HIDDEN_UNITS = getenv_ints("HIDDEN_UNITS", "20 30")
 
 #...............................................................................
 # Utility functions
 
-def round3(num):
-    """Round NUM using precision of 3"""
-    return system.round_num(num, 3)
-
 def non_negative(num):
     """Whether integer NUM > -1"""
     return (num > -1)
 
 # TODO: put following in new ml_utils.py module
 def create_feature_mapping(label_values):
     """Return hash mapping elements from LABEL_VALUES into integers"""
```

### Comparing `mezcla-1.3.9.1/mezcla/main.py` & `mezcla-1.3.9.2/mezcla/main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/merge_files.py` & `mezcla-1.3.9.2/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/merge_notes.py` & `mezcla-1.3.9.2/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/misc_utils.py` & `mezcla-1.3.9.2/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/my_regex.py` & `mezcla-1.3.9.2/mezcla/my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/ngram_tfidf.py` & `mezcla-1.3.9.2/mezcla/ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/os_utils.py` & `mezcla-1.3.9.2/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/pandas_sklearn.py` & `mezcla-1.3.9.2/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/plot_utils.py` & `mezcla-1.3.9.2/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/randomize_lines.py` & `mezcla-1.3.9.2/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/rgb_color_name.py` & `mezcla-1.3.9.2/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/run_albert_classifier.py` & `mezcla-1.3.9.2/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/run_bert_classifier.py` & `mezcla-1.3.9.2/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/show_bert_representation.py` & `mezcla-1.3.9.2/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/simple_main_example.py` & `mezcla-1.3.9.2/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/spacy_nlp.py` & `mezcla-1.3.9.2/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/spell.py` & `mezcla-1.3.9.2/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/sys_version_info_hack.py` & `mezcla-1.3.9.2/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/system.py` & `mezcla-1.3.9.2/mezcla/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,22 +140,30 @@
         option_info = sorted(option_info)
     entry_separator = "\n%s" % indent
     descriptions = entry_separator.join(["%s%s%s" % (opt, indent, (desc if desc else "n/a")) for (opt, desc) in option_info])
     debug.trace_fmt(6, "formatted_environment_option_descriptions() => {d}",
                     d=descriptions)
     return descriptions
 
+
 def getenv(var, default_value=None):
     """Simple wrapper around os.getenv, with tracing"""
     # Note: Use getenv_* for type-specific versions with env. option description
     result = os.getenv(var, default_value)
     debug.trace_fmt(5, "getenv({v}, {dv}) => {r}", v=var, dv=default_value, r=result)
     return result
 
 
+def setenv(var, value):
+    """Set environment VAR to VALUE"""
+    debug.trace_fmtd(5, "setenv({v}, {val})", v=var, val=value)
+    os.environ[var] = value
+    return
+
+
 def getenv_text(var, default=None, description=None, helper=False):
     """Returns textual value for environment variable VAR (or DEFAULT value, excluding None).
     Notes:
     - Use getenv_value if default can be None, as result is always a string.
     - HELPER indicates that this call is in support of another getenv-type function (e.g., getenv_bool), so that tracing is only shown at higher verbosity level (e.g., 6 not 5).
     - DESCRIPTION used for get_environment_option_descriptions."""
     # Note: default is empty string to ensure result is string (not NoneType)
@@ -246,40 +254,53 @@
     # Note: Convenience wrapper to avoid need to import sys in simple scripts.
     return sys.exc_info()
 
 def print_error(text):
     """Output TEXT to standard error
     Note: Use print_error_fmt to include format keyword arguments"
     """
+    debug.trace(7, f"print_error({text})")
     # ex: print_error("Fubar!")
     print(text, file=sys.stderr)
-    return
+    return None
 
-def print_stderr(text, **kwargs):
-    """Output TEXT to standard error, using KWARGS for formatting"""
-    # NOTE: Deprecated function: use print_error_fmt instead.
+def print_stderr_fmt(text, **kwargs):
+    """Output TEXT to standard error, using KWARGS for formatting"""       
     # ex: print_stderr("Error: F{oo}bar!", oo=("oo" if (time_in_secs() % 2) else "u"))
     # TODO: rename as print_error_fmt
     # TODO: weed out calls that use (text.format(...)) rather than (text, ...)
+    debug.trace(7, f"print_stderr_fmt({text}, kw={kwargs})")
     formatted_text = text
     try:
         # Note: to avoid interpolated text as being interpreted as variable
         # references, this function should do the formatting
         # ex: print_stderr("hey {you}".format(you="{u}")) => print_stderr("hey {you}".format(you="{u}"))
         debug.assertion(kwargs or (not re.search(r"{\S*}", text)))
         formatted_text = text.format(**kwargs)
     except(KeyError, ValueError, UnicodeEncodeError):
         sys.stderr.write("Warning: Problem in print_stderr: {exc}\n".format(
             exc=get_exception()))
         if debug.verbose_debugging():
             print_full_stack()
     print(formatted_text, file=sys.stderr)
-    return
+    return None
+#
 #
-print_error_fmt = print_stderr
+def print_stderr(text, **kwargs):
+    """Currently, an alias for print_stderr_fmt
+    Note: soon to be alias for print_error (i.e., kwargs will not supported)"""
+    debug.trace(7, f"print_stderr({text}, kw={kwargs})")
+    # TODO?: if kwargs: debug.trace(2, "Warning: kwargs no longer supported; use print_stderr_fmt
+    # NOTE: maldito pylint (see https://github.com/pylint-dev/pylint/issues/2332 [Don't issue assignment-from-none if None is returned explicitly]
+    # pylint: disable=assignment-from-none
+    if not kwargs:
+        result = print_error(text)
+    else:
+        result = print_stderr_fmt(text, **kwargs)
+    return result
 
 
 def print_exception_info(task, show_stack=None):
     """Output exception information to stderr regarding TASK (e.g., function);
     Note: Optionally includes stack trace (default when detailed debugging)"""
     # Note: used to simplify exception reporting of border conditions
     # ex: print_exception_info("read_csv")
@@ -291,33 +312,25 @@
         print_full_stack()
     return
 
 
 def exit(message=None, status_code=None, **namespace):    # pylint: disable=redefined-builtin
     """Display error MESSAGE to stderr and then exit, using optional
     NAMESPACE for format. The STATUS_CODE can be overrided (n.b., 0 if None)."""
-    # EX: exit("Error: {reason}!", reason="Whatever")
-    debug.trace(6, f"system.exit{(message, namespace)})")
+    # EX: exit("Error: {reason}!", status_code=123, reason="Whatever")
+    debug.trace(6, f"system.exit{(message, status_code, namespace)}")
     if namespace:
         message = message.format(**namespace)
     if message:
         print_stderr(message)
         if status_code is None:
             status_code = 1
     return sys.exit(status_code)
 
 
-def setenv(var, value):
-    """Set environment VAR to VALUE"""
-    debug.trace_fmtd(5, "setenv({v}, {val})", v=var, val=value)
-    os.environ[var] = value
-    return
-## TODO: move above (e.g., after getenv)
-
-
 def print_full_stack(stream=sys.stderr):
     """Prints stack trace (for use in error messages, etc.)"""
     # Notes: Developed originally for Android stack tracing support.
     # Based on http://blog.dscpl.com.au/2015/03/generating-full-stack-traces-for.html.
     # TODO: Update based on author's code update (e.g., ???)
     # TODO: Fix off-by-one error in display of offending statement!
     debug.trace_fmtd(7, "print_full_stack(stream={s})", s=stream)
@@ -1204,14 +1217,19 @@
     # EX: round_as_str(3.15914, 3) => "3.159"
     result = f"{round_num(value, precision):.{precision}f}"
     debug.trace_fmtd(8, "round_as_str({v}, [prec={p}]) => {r}",
                      v=value, p=precision, r=result)
     return result
 
 
+def round3(num):
+    """Round NUM using precision of 3"""
+    return round_num(num, 3)
+
+
 def sleep(num_seconds, trace_level=5):
     """Sleep for NUM_SECONDS"""
     # TODO: annotate num_seconds with float
     debug.trace_fmtd(trace_level, "sleep({ns}, [tl={tl}])",
                      ns=num_seconds, tl=trace_level)
     time.sleep(num_seconds)
     return
```

### Comparing `mezcla-1.3.9.1/mezcla/temp/simple_batspp.py` & `mezcla-1.3.9.2/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/template.py` & `mezcla-1.3.9.2/mezcla/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 TL = debug.TL
 
 # Environment options
 # Note: These are just intended for internal options, not for end users.
 # It also allows for enabling options in one place rather than four
 # (e.g., [Main member] initialization, run-time value, and argument spec., along
 # with string constant definition).
+# WARNING: To minimize environment comflicts with other programs make the names
+# longer such as two or more tokens (e.g., "FUBAR" => "FUBAR_LEVEL").
 #
 TODO_FUBAR = system.getenv_bool("TODO_FUBAR", False,
                                 description="TODO:Fouled Up Beyond All Recognition processing")
 
 
 class Script(Main):
     """Input processing class"""
@@ -136,10 +138,10 @@
     debug.assertion(not any(my_re.search(r"^TODO_", m, my_re.IGNORECASE)
                             for m in dir(app)))    
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_VERBOSE)
-    debug.trace(5, f"main __doc__: {main.__doc__}")
+    debug.trace(5, f"module __doc__: {___doc__}")
     debug.assertion("TODO:" not in __doc__)
     main()
```

### Comparing `mezcla-1.3.9.1/mezcla/tests/LICENSE.txt` & `mezcla-1.3.9.2/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.9.2/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/misc_doctests.py` & `mezcla-1.3.9.2/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.3.9.2/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.3.9.2/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/cars.csv` & `mezcla-1.3.9.2/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.9.2/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.9.2/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.9.2/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.9.2/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.9.2/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.9.2/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.9.2/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/template.py` & `mezcla-1.3.9.2/mezcla/tests/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #! /usr/bin/env python
 #
 # TODO: Test(s) for ../<module>.py
 #
 # Notes:
 # - Fill out TODO's below. Use numbered tests to order (e.g., test_1_usage).
+# - * See test_python_ast.py for simple example of customization.
 # - TODO: If any of the setup/cleanup methods defined, make sure to invoke base
 #   (see examples below for setUp and tearDown).
 # - For debugging the tested script, the ALLOW_SUBCOMMAND_TRACING environment
-#   option shows tracing output normally suppressed by  unittest_wrapper.py.
+#   option shows tracing output normally suppressed by unittest_wrapper.py.
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_<module>.py
 #
 
 """TODO: Tests for <module> module"""
 
 # Standard packages
@@ -44,17 +45,16 @@
 ## # It also allows for enabling options in one place.
 ## #
 ## FUBAR = system.getenv_bool("FUBAR", False,
 ##                            description="Fouled Up Beyond All Recognition processing")
 
 
 class TestIt(TestWrapper):
-    """Class for testcase definition"""
+    """Class for command-line based testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
-    # -or- non-mezcla: script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     #
     # TODO: use_temp_base_dir = True            # treat TEMP_BASE as directory
     # note: temp_file defined by parent (along with script_module, temp_base, and test_num)
 
     ## TODO: optional setup methods
     ##
     ## @classmethod
@@ -110,16 +110,16 @@
     ##     ...
     ##     return
 
 ## TODO:
 ## #...............................................................................
 ##
 ## class TestIt2:
-##     """Another class for testcase definition
-##     Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper"""
+##     """Class for API-based testcase definition
+##     Note: Separate class avoids error with pytest due to inheritance with unittest.TestCase via TestWrapper"""
 ##
 ##     def test_whatever(self):
 ##         """TODO: flesh out test for whatever"""
 ##         debug.trace(4, f"TestIt2.test_whatever(); self={self}")
 ##         assert False, "TODO: code test"
 ##         ## ex: assert THE_MODULE.fast_sort() == THE_MODULE.slow_sort()
 ##         return
```

### Comparing `mezcla-1.3.9.1/mezcla/tests/test___init__.py` & `mezcla-1.3.9.2/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_audio.py` & `mezcla-1.3.9.2/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.9.2/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_bing_search.py` & `mezcla-1.3.9.2/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.9.2/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_convert_emoticons.py` & `mezcla-1.3.9.2/mezcla/tests/test_convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_cut.py` & `mezcla-1.3.9.2/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_data_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_debug.py` & `mezcla-1.3.9.2/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.9.2/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_file_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_filter_random.py` & `mezcla-1.3.9.2/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.9.2/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.9.2/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_html_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.9.2/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.9.2/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_main.py` & `mezcla-1.3.9.2/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_merge_files.py` & `mezcla-1.3.9.2/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.9.2/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_my_regex.py` & `mezcla-1.3.9.2/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.9.2/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_os_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.9.2/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.9.2/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.9.2/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.9.2/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.9.2/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.9.2/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.9.2/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.9.2/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.9.2/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_system.py` & `mezcla-1.3.9.2/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_template.py` & `mezcla-1.3.9.2/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.9.2/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_text_processing.py` & `mezcla-1.3.9.2/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_text_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.9.2/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.9.2/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.9.2/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.9.2/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.9.2/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.9.2/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.9.2/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.9.2/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.9.2/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/text_categorizer.py` & `mezcla-1.3.9.2/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/text_processing.py` & `mezcla-1.3.9.2/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/text_utils.py` & `mezcla-1.3.9.2/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tfidf/corpus.py` & `mezcla-1.3.9.2/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.9.2/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tfidf/document.py` & `mezcla-1.3.9.2/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tfidf/preprocess.py` & `mezcla-1.3.9.2/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/tpo_common.py` & `mezcla-1.3.9.2/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/train_language_model.py` & `mezcla-1.3.9.2/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/train_text_categorizer.py` & `mezcla-1.3.9.2/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/transpose_data.py` & `mezcla-1.3.9.2/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/unittest_wrapper.py` & `mezcla-1.3.9.2/mezcla/unittest_wrapper.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/mezcla/xml_utils.py` & `mezcla-1.3.9.2/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/pyproject.toml` & `mezcla-1.3.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## TODO: eliminate redundancy
 
 [tool.poetry]
 name = "mezcla"
-version = "1.3.9.1"
+version = "1.3.9.2"
 description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
 authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `mezcla-1.3.9.1/requirements.txt` & `mezcla-1.3.9.2/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,21 @@
 # - check absl module ($ grep -r "absl" .)
 # - add support for this to setup.py
 #...............................................................................
 # Regular requirements
 #
 HTMLParser==0.0.2
 absl_py==1.2.0
-albert==1.3.1
 beautifulsoup4==4.11.1
-bert==2.2.0
 bs4
 cachetools
 cherrypy
 extcolors>=1.0.0
 git+https://github.com/tehabstract/textract.git
 gradio
-ibm_cloud_sdk_core==3.15.3
 lxml
 mako
 matplotlib
 nltk
 numpy>=1.18.5
 pandas>=1.3.0
 pyaml
@@ -72,14 +69,15 @@
 #opt# coverage
 #opt# datasets
 #opt# diffusers
 #opt# flask
 #opt# flit
 #opt# gensim
 #opt# ibm-watson
+#opt# ibm_cloud_sdk_core==3.15.3
 #opt# ipython
 #opt# jupyter
 #opt# kenlm
 #opt# librosa
 #opt# more_itertools
 #opt# pylint
 #opt# pyyaml
@@ -87,13 +85,15 @@
 #opt# spacy>=3.0.0
 #opt# torch
 #opt# transformers
 #...............................................................................
 # "Fully optional" requirements
 # Note: these generally involve large or long installations.
 #
+#full# bert==2.2.0
+#full# albert==1.3.1
 #full# bert-tensorflow
 #full# keras
 #full# lucene
 #full# sacremoses
 #full# sentencepiece
 #full# tensorflow
```

### Comparing `mezcla-1.3.9.1/setup.py` & `mezcla-1.3.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
       ## TODO2: import mezcla; version=mezcla.VERSION
-      version='1.3.9.1',
+      version="1.3.9.2",
       description-file="README.txt",
       dist-name="Mezcla",
       author="Tom O'Hara",
       # TODO3: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
       requires-python=">=3.8",
```

### Comparing `mezcla-1.3.9.1/temp/simple_batspp.py` & `mezcla-1.3.9.2/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/tools/run_tests.bash` & `mezcla-1.3.9.2/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/tox.ini` & `mezcla-1.3.9.2/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.1/PKG-INFO` & `mezcla-1.3.9.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.9.1
+Version: 1.3.9.2
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

