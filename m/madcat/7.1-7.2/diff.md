# Comparing `tmp/madcat-7.1.tar.gz` & `tmp/madcat-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madcat-7.1.tar", last modified: Wed Jul 19 14:18:20 2023, max compression
+gzip compressed data, was "madcat-7.2.tar", last modified: Thu Jul 20 13:52:06 2023, max compression
```

## Comparing `madcat-7.1.tar` & `madcat-7.2.tar`

### file list

```diff
@@ -1,173 +1,172 @@
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.184746 madcat-7.1/
--rw-r--r--   0 amitosi    (501) staff       (20)      189 2023-07-19 14:18:20.184587 madcat-7.1/PKG-INFO
--rw-r--r--   0 amitosi    (501) staff       (20)     1367 2023-03-22 15:02:11.000000 madcat-7.1/README.md
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.156184 madcat-7.1/chester/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.157139 madcat-7.1/chester/cleaning/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/cleaning/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1726 2023-02-14 11:01:28.000000 madcat-7.1/chester/cleaning/cleaner_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     8913 2023-02-14 11:10:19.000000 madcat-7.1/chester/cleaning/cleaning_func.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.157475 madcat-7.1/chester/data/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-16 07:01:02.000000 madcat-7.1/chester/data/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.157710 madcat-7.1/chester/data_loader/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/data_loader/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      693 2023-02-10 12:03:58.000000 madcat-7.1/chester/data_loader/webtext_data.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.158090 madcat-7.1/chester/feature_analyzing/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/feature_analyzing/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     7767 2023-02-12 13:00:40.000000 madcat-7.1/chester/feature_analyzing/feature_correlation.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.159704 madcat-7.1/chester/feature_stats/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/feature_stats/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6113 2023-05-28 15:36:04.000000 madcat-7.1/chester/feature_stats/categorical_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)      214 2023-02-08 10:13:48.000000 madcat-7.1/chester/feature_stats/feature_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5521 2023-02-14 12:45:27.000000 madcat-7.1/chester/feature_stats/numeric_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2152 2023-03-21 07:33:39.000000 madcat-7.1/chester/feature_stats/text_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)     7292 2023-02-20 17:02:27.000000 madcat-7.1/chester/feature_stats/time_series_stats.py
--rw-r--r--   0 amitosi    (501) staff       (20)      646 2023-02-14 14:21:02.000000 madcat-7.1/chester/feature_stats/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.161360 madcat-7.1/chester/features_engineering/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/features_engineering/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2222 2023-02-05 11:09:58.000000 madcat-7.1/chester/features_engineering/bag_of_words.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2218 2023-03-07 08:09:18.000000 madcat-7.1/chester/features_engineering/corex.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6275 2023-03-07 06:57:19.000000 madcat-7.1/chester/features_engineering/fe_nlp.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4745 2023-03-21 07:33:39.000000 madcat-7.1/chester/features_engineering/feature_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3355 2023-03-07 07:20:49.000000 madcat-7.1/chester/features_engineering/features_handler.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1970 2023-02-05 11:09:58.000000 madcat-7.1/chester/features_engineering/tfidf.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.163905 madcat-7.1/chester/features_engineering/time_series/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-15 07:10:16.000000 madcat-7.1/chester/features_engineering/time_series/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1829 2023-02-17 09:22:41.000000 madcat-7.1/chester/features_engineering/time_series/cyclic_features_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4455 2023-02-16 13:45:22.000000 madcat-7.1/chester/features_engineering/time_series/event_counter.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1909 2023-02-27 19:09:23.000000 madcat-7.1/chester/features_engineering/time_series/feature_elimination_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5324 2023-02-16 14:23:15.000000 madcat-7.1/chester/features_engineering/time_series/frequencies_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5317 2023-02-18 11:46:20.000000 madcat-7.1/chester/features_engineering/time_series/get_time_freqeuency_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4379 2023-02-16 14:20:54.000000 madcat-7.1/chester/features_engineering/time_series/moving_metric_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4129 2023-02-16 10:20:17.000000 madcat-7.1/chester/features_engineering/time_series/static_features_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4907 2023-02-20 16:14:11.000000 madcat-7.1/chester/features_engineering/time_series/ts_feature_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1013 2023-02-17 13:51:59.000000 madcat-7.1/chester/features_engineering/time_series/ts_features_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)      379 2023-02-17 14:38:52.000000 madcat-7.1/chester/features_engineering/time_series/ts_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.164265 madcat-7.1/chester/model_analyzer/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/model_analyzer/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    11364 2023-02-19 08:56:08.000000 madcat-7.1/chester/model_analyzer/model_analysis.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.165246 madcat-7.1/chester/model_monitor/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/model_monitor/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      887 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_monitor/calculate_scores_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5339 2023-07-19 14:00:30.000000 madcat-7.1/chester/model_monitor/error_prediction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4219 2023-07-19 14:00:30.000000 madcat-7.1/chester/model_monitor/model_boostrap.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.165982 madcat-7.1/chester/model_training/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/model_training/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3427 2023-02-05 19:57:36.000000 madcat-7.1/chester/model_training/data_preparation.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2149 2023-02-11 16:14:05.000000 madcat-7.1/chester/model_training/model_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.166730 madcat-7.1/chester/model_training/models/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/model_training/models/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.169294 madcat-7.1/chester/model_training/models/chester_models/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/model_training/models/chester_models/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1977 2023-02-11 10:13:40.000000 madcat-7.1/chester/model_training/models/chester_models/base_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2160 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_training/models/chester_models/base_model_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.169963 madcat-7.1/chester/model_training/models/chester_models/baseline/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/model_training/models/chester_models/baseline/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1012 2023-02-12 12:18:36.000000 madcat-7.1/chester/model_training/models/chester_models/baseline/baseline_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3519 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_training/models/chester_models/baseline/baseline_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1965 2023-02-12 12:18:36.000000 madcat-7.1/chester/model_training/models/chester_models/best_baseline_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1769 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_training/models/chester_models/best_linear_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1917 2023-02-14 15:09:08.000000 madcat-7.1/chester/model_training/models/chester_models/best_logistic_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2354 2023-07-19 14:09:20.000000 madcat-7.1/chester/model_training/models/chester_models/best_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5160 2023-07-19 14:09:20.000000 madcat-7.1/chester/model_training/models/chester_models/compare_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1750 2023-02-10 12:10:30.000000 madcat-7.1/chester/model_training/models/chester_models/hp_generator.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.170463 madcat-7.1/chester/model_training/models/chester_models/linear_regression/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/model_training/models/chester_models/linear_regression/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2429 2023-02-17 12:12:20.000000 madcat-7.1/chester/model_training/models/chester_models/linear_regression/linear_regression.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6891 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.171027 madcat-7.1/chester/model_training/models/chester_models/logistic_regression/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/model_training/models/chester_models/logistic_regression/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2542 2023-02-14 15:54:46.000000 madcat-7.1/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6637 2023-02-10 12:10:10.000000 madcat-7.1/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2040 2023-02-05 11:09:58.000000 madcat-7.1/chester/model_training/models/cv_training.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4764 2023-02-05 11:09:58.000000 madcat-7.1/chester/model_training/models/lstm.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1155 2023-02-10 12:20:48.000000 madcat-7.1/chester/model_training/models/scoring.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.171662 madcat-7.1/chester/post_model_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/post_model_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    12668 2023-02-23 10:52:06.000000 madcat-7.1/chester/post_model_analysis/post_model_analysis_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1492 2023-02-11 16:14:05.000000 madcat-7.1/chester/post_model_analysis/post_regression.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.172833 madcat-7.1/chester/pre_model_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/pre_model_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)    15538 2023-03-11 12:30:17.000000 madcat-7.1/chester/pre_model_analysis/categorical.py
--rw-r--r--   0 amitosi    (501) staff       (20)    15136 2023-03-21 11:25:00.000000 madcat-7.1/chester/pre_model_analysis/numerics.py
--rw-r--r--   0 amitosi    (501) staff       (20)     9856 2023-02-19 19:27:25.000000 madcat-7.1/chester/pre_model_analysis/target.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3383 2023-02-20 16:04:59.000000 madcat-7.1/chester/pre_model_analysis/time_series.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.173477 madcat-7.1/chester/preprocessing/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/preprocessing/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5096 2023-02-14 11:12:55.000000 madcat-7.1/chester/preprocessing/preprocessing_func.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1661 2023-03-07 06:13:34.000000 madcat-7.1/chester/preprocessing/preprocessor_handler.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.174495 madcat-7.1/chester/run/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-08 09:40:57.000000 madcat-7.1/chester/run/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1786 2023-02-11 11:52:10.000000 madcat-7.1/chester/run/chapter_titles.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2779 2023-02-08 21:21:02.000000 madcat-7.1/chester/run/feature_attention_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)    16206 2023-03-21 07:53:41.000000 madcat-7.1/chester/run/full_run.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5035 2023-03-21 07:33:39.000000 madcat-7.1/chester/run/user_classes.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.175515 madcat-7.1/chester/run_manual_chester/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 13:32:50.000000 madcat-7.1/chester/run_manual_chester/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3638 2023-05-29 14:23:09.000000 madcat-7.1/chester/run_manual_chester/bad_data.py
--rw-r--r--   0 amitosi    (501) staff       (20)      602 2023-06-10 12:20:58.000000 madcat-7.1/chester/run_manual_chester/bad_data2.py
--rw-r--r--   0 amitosi    (501) staff       (20)    19306 2023-03-21 07:53:41.000000 madcat-7.1/chester/run_manual_chester/manual_run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.177629 madcat-7.1/chester/text_stats_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/text_stats_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1261 2023-02-14 11:53:21.000000 madcat-7.1/chester/text_stats_analysis/common_words.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3708 2023-03-07 08:42:30.000000 madcat-7.1/chester/text_stats_analysis/corex_topics.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4446 2023-03-21 07:33:39.000000 madcat-7.1/chester/text_stats_analysis/data_quality.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3466 2023-02-14 12:12:27.000000 madcat-7.1/chester/text_stats_analysis/key_sentences.py
--rw-r--r--   0 amitosi    (501) staff       (20)     3663 2023-02-14 12:20:36.000000 madcat-7.1/chester/text_stats_analysis/keywords_extraction.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1951 2023-02-14 14:04:54.000000 madcat-7.1/chester/text_stats_analysis/sentiment.py
--rw-r--r--   0 amitosi    (501) staff       (20)    10355 2023-03-21 07:33:39.000000 madcat-7.1/chester/text_stats_analysis/smart_text_analyzer.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4118 2023-03-21 07:33:39.000000 madcat-7.1/chester/text_stats_analysis/text_summary.py
--rw-r--r--   0 amitosi    (501) staff       (20)      526 2023-02-11 16:14:05.000000 madcat-7.1/chester/text_stats_analysis/word_cloud.py
--rw-r--r--   0 amitosi    (501) staff       (20)     5304 2023-02-19 09:26:17.000000 madcat-7.1/chester/util.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.177895 madcat-7.1/chester/utils/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.1/chester/utils/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.178513 madcat-7.1/chester/zero_break/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.1/chester/zero_break/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)       89 2023-02-05 11:09:58.000000 madcat-7.1/chester/zero_break/get_or_else.py
--rw-r--r--   0 amitosi    (501) staff       (20)     8904 2023-07-19 14:09:20.000000 madcat-7.1/chester/zero_break/problem_specification.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1694 2023-03-11 12:21:56.000000 madcat-7.1/chester/zero_break/text_detector.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.178841 madcat-7.1/example_notebooks/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-11 13:38:57.000000 madcat-7.1/example_notebooks/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2981 2023-03-11 15:08:39.000000 madcat-7.1/example_notebooks/main.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.179489 madcat-7.1/madcat.egg-info/
--rw-r--r--   0 amitosi    (501) staff       (20)      189 2023-07-19 14:18:20.000000 madcat-7.1/madcat.egg-info/PKG-INFO
--rw-r--r--   0 amitosi    (501) staff       (20)     5812 2023-07-19 14:18:20.000000 madcat-7.1/madcat.egg-info/SOURCES.txt
--rw-r--r--   0 amitosi    (501) staff       (20)        1 2023-07-19 14:18:20.000000 madcat-7.1/madcat.egg-info/dependency_links.txt
--rw-r--r--   0 amitosi    (501) staff       (20)      273 2023-07-19 14:18:20.000000 madcat-7.1/madcat.egg-info/requires.txt
--rw-r--r--   0 amitosi    (501) staff       (20)       33 2023-07-19 14:18:20.000000 madcat-7.1/madcat.egg-info/top_level.txt
--rw-r--r--   0 amitosi    (501) staff       (20)       38 2023-07-19 14:18:20.184819 madcat-7.1/setup.cfg
--rw-r--r--   0 amitosi    (501) staff       (20)      559 2023-07-19 14:17:52.000000 madcat-7.1/setup.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.179911 madcat-7.1/tamtam/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:37:31.000000 madcat-7.1/tamtam/__init__.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.180891 madcat-7.1/tamtam/ab_feature_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 10:02:44.000000 madcat-7.1/tamtam/ab_feature_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)      541 2023-02-23 10:19:25.000000 madcat-7.1/tamtam/ab_feature_analysis/ab_catboost.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1923 2023-03-21 07:53:41.000000 madcat-7.1/tamtam/ab_feature_analysis/ab_feature_analysis_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)      348 2023-02-23 10:19:25.000000 madcat-7.1/tamtam/ab_feature_analysis/ab_partial_plot.py
--rw-r--r--   0 amitosi    (501) staff       (20)      402 2023-02-23 10:19:25.000000 madcat-7.1/tamtam/ab_feature_analysis/ab_tree_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.181258 madcat-7.1/tamtam/ab_info/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:44:45.000000 madcat-7.1/tamtam/ab_info/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     4011 2023-02-23 21:52:11.000000 madcat-7.1/tamtam/ab_info/ab_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.181685 madcat-7.1/tamtam/allocation_calculation/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 13:01:46.000000 madcat-7.1/tamtam/allocation_calculation/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1937 2023-02-22 14:13:02.000000 madcat-7.1/tamtam/allocation_calculation/bias_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.182005 madcat-7.1/tamtam/delta_analysis/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 07:37:32.000000 madcat-7.1/tamtam/delta_analysis/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     6199 2023-02-23 21:48:17.000000 madcat-7.1/tamtam/delta_analysis/delta_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2517 2023-02-23 21:45:56.000000 madcat-7.1/tamtam/manual_run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.182324 madcat-7.1/tamtam/metrics_correlation/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 14:27:03.000000 madcat-7.1/tamtam/metrics_correlation/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2350 2023-02-23 14:45:57.000000 madcat-7.1/tamtam/metrics_correlation/metric_class.py
--rw-r--r--   0 amitosi    (501) staff       (20)      964 2023-02-23 14:45:57.000000 madcat-7.1/tamtam/run.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.182647 madcat-7.1/tamtam/user_class/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:41:13.000000 madcat-7.1/tamtam/user_class/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)     1895 2023-02-23 11:53:41.000000 madcat-7.1/tamtam/user_class/user_class.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.183208 madcat-7.1/tamtam/utils/
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 10:08:15.000000 madcat-7.1/tamtam/utils/__init__.py
--rw-r--r--   0 amitosi    (501) staff       (20)       54 2023-02-22 16:12:56.000000 madcat-7.1/tamtam/utils/column_utils.py
--rw-r--r--   0 amitosi    (501) staff       (20)       59 2023-02-22 16:24:31.000000 madcat-7.1/tamtam/utils/utils.py
-drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-19 14:18:20.184158 madcat-7.1/tests/
--rw-r--r--   0 amitosi    (501) staff       (20)     2501 2023-02-05 11:09:51.000000 madcat-7.1/tests/test_cleaning.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2119 2023-02-05 11:09:51.000000 madcat-7.1/tests/test_preprocessing.py
--rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:51.000000 madcat-7.1/tests/test_util.py
--rw-r--r--   0 amitosi    (501) staff       (20)     2843 2023-02-05 11:09:58.000000 madcat-7.1/tests/test_zero_break.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.644204 madcat-7.2/
+-rw-r--r--   0 amitosi    (501) staff       (20)      189 2023-07-20 13:52:06.644066 madcat-7.2/PKG-INFO
+-rw-r--r--   0 amitosi    (501) staff       (20)     1367 2023-03-22 15:02:11.000000 madcat-7.2/README.md
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.616498 madcat-7.2/chester/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.617478 madcat-7.2/chester/cleaning/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/cleaning/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1726 2023-02-14 11:01:28.000000 madcat-7.2/chester/cleaning/cleaner_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     8913 2023-02-14 11:10:19.000000 madcat-7.2/chester/cleaning/cleaning_func.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.617795 madcat-7.2/chester/data/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-16 07:01:02.000000 madcat-7.2/chester/data/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.618044 madcat-7.2/chester/data_loader/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/data_loader/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      693 2023-02-10 12:03:58.000000 madcat-7.2/chester/data_loader/webtext_data.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.618470 madcat-7.2/chester/feature_analyzing/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/feature_analyzing/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     7767 2023-02-12 13:00:40.000000 madcat-7.2/chester/feature_analyzing/feature_correlation.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.620101 madcat-7.2/chester/feature_stats/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/feature_stats/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6078 2023-07-20 13:21:31.000000 madcat-7.2/chester/feature_stats/categorical_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      214 2023-02-08 10:13:48.000000 madcat-7.2/chester/feature_stats/feature_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5521 2023-02-14 12:45:27.000000 madcat-7.2/chester/feature_stats/numeric_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2152 2023-03-21 07:33:39.000000 madcat-7.2/chester/feature_stats/text_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     7362 2023-07-20 13:46:16.000000 madcat-7.2/chester/feature_stats/time_series_stats.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      646 2023-02-14 14:21:02.000000 madcat-7.2/chester/feature_stats/utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.621585 madcat-7.2/chester/features_engineering/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/features_engineering/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2222 2023-02-05 11:09:58.000000 madcat-7.2/chester/features_engineering/bag_of_words.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2218 2023-03-07 08:09:18.000000 madcat-7.2/chester/features_engineering/corex.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6275 2023-03-07 06:57:19.000000 madcat-7.2/chester/features_engineering/fe_nlp.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4745 2023-03-21 07:33:39.000000 madcat-7.2/chester/features_engineering/feature_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3355 2023-03-07 07:20:49.000000 madcat-7.2/chester/features_engineering/features_handler.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1970 2023-02-05 11:09:58.000000 madcat-7.2/chester/features_engineering/tfidf.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.624077 madcat-7.2/chester/features_engineering/time_series/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-15 07:10:16.000000 madcat-7.2/chester/features_engineering/time_series/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1829 2023-02-17 09:22:41.000000 madcat-7.2/chester/features_engineering/time_series/cyclic_features_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4455 2023-02-16 13:45:22.000000 madcat-7.2/chester/features_engineering/time_series/event_counter.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1909 2023-02-27 19:09:23.000000 madcat-7.2/chester/features_engineering/time_series/feature_elimination_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5399 2023-07-20 13:34:44.000000 madcat-7.2/chester/features_engineering/time_series/frequencies_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5317 2023-02-18 11:46:20.000000 madcat-7.2/chester/features_engineering/time_series/get_time_freqeuency_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4379 2023-02-16 14:20:54.000000 madcat-7.2/chester/features_engineering/time_series/moving_metric_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3355 2023-07-20 13:32:39.000000 madcat-7.2/chester/features_engineering/time_series/static_features_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4977 2023-07-20 13:40:26.000000 madcat-7.2/chester/features_engineering/time_series/ts_feature_extraction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1103 2023-07-20 13:41:21.000000 madcat-7.2/chester/features_engineering/time_series/ts_features_extraction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      379 2023-02-17 14:38:52.000000 madcat-7.2/chester/features_engineering/time_series/ts_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.624400 madcat-7.2/chester/model_analyzer/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/model_analyzer/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    11364 2023-02-19 08:56:08.000000 madcat-7.2/chester/model_analyzer/model_analysis.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.625366 madcat-7.2/chester/model_monitor/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/model_monitor/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      887 2023-02-10 12:10:10.000000 madcat-7.2/chester/model_monitor/calculate_scores_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5339 2023-07-19 14:00:30.000000 madcat-7.2/chester/model_monitor/error_prediction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4219 2023-07-19 14:00:30.000000 madcat-7.2/chester/model_monitor/model_boostrap.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.626059 madcat-7.2/chester/model_training/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/model_training/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3427 2023-02-05 19:57:36.000000 madcat-7.2/chester/model_training/data_preparation.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2149 2023-02-11 16:14:05.000000 madcat-7.2/chester/model_training/model_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.626831 madcat-7.2/chester/model_training/models/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/model_training/models/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.628872 madcat-7.2/chester/model_training/models/chester_models/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/model_training/models/chester_models/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1977 2023-02-11 10:13:40.000000 madcat-7.2/chester/model_training/models/chester_models/base_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2160 2023-02-10 12:10:10.000000 madcat-7.2/chester/model_training/models/chester_models/base_model_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.629535 madcat-7.2/chester/model_training/models/chester_models/baseline/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/model_training/models/chester_models/baseline/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1012 2023-02-12 12:18:36.000000 madcat-7.2/chester/model_training/models/chester_models/baseline/baseline_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3519 2023-02-10 12:10:10.000000 madcat-7.2/chester/model_training/models/chester_models/baseline/baseline_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1965 2023-02-12 12:18:36.000000 madcat-7.2/chester/model_training/models/chester_models/best_baseline_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1659 2023-07-20 13:04:51.000000 madcat-7.2/chester/model_training/models/chester_models/best_linear_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1917 2023-02-14 15:09:08.000000 madcat-7.2/chester/model_training/models/chester_models/best_logistic_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2354 2023-07-19 14:09:20.000000 madcat-7.2/chester/model_training/models/chester_models/best_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5160 2023-07-19 14:09:20.000000 madcat-7.2/chester/model_training/models/chester_models/compare_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1750 2023-02-10 12:10:30.000000 madcat-7.2/chester/model_training/models/chester_models/hp_generator.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.630056 madcat-7.2/chester/model_training/models/chester_models/linear_regression/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/model_training/models/chester_models/linear_regression/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2429 2023-02-17 12:12:20.000000 madcat-7.2/chester/model_training/models/chester_models/linear_regression/linear_regression.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6891 2023-02-10 12:10:10.000000 madcat-7.2/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.630571 madcat-7.2/chester/model_training/models/chester_models/logistic_regression/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/model_training/models/chester_models/logistic_regression/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2542 2023-02-14 15:54:46.000000 madcat-7.2/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6637 2023-02-10 12:10:10.000000 madcat-7.2/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2040 2023-02-05 11:09:58.000000 madcat-7.2/chester/model_training/models/cv_training.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4764 2023-02-05 11:09:58.000000 madcat-7.2/chester/model_training/models/lstm.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1155 2023-02-10 12:20:48.000000 madcat-7.2/chester/model_training/models/scoring.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.631087 madcat-7.2/chester/post_model_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/post_model_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    12668 2023-02-23 10:52:06.000000 madcat-7.2/chester/post_model_analysis/post_model_analysis_class.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1492 2023-02-11 16:14:05.000000 madcat-7.2/chester/post_model_analysis/post_regression.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.632262 madcat-7.2/chester/pre_model_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/pre_model_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    15538 2023-03-11 12:30:17.000000 madcat-7.2/chester/pre_model_analysis/categorical.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    15136 2023-03-21 11:25:00.000000 madcat-7.2/chester/pre_model_analysis/numerics.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     9856 2023-02-19 19:27:25.000000 madcat-7.2/chester/pre_model_analysis/target.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3383 2023-02-20 16:04:59.000000 madcat-7.2/chester/pre_model_analysis/time_series.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.632914 madcat-7.2/chester/preprocessing/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/preprocessing/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5096 2023-02-14 11:12:55.000000 madcat-7.2/chester/preprocessing/preprocessing_func.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1661 2023-03-07 06:13:34.000000 madcat-7.2/chester/preprocessing/preprocessor_handler.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.633900 madcat-7.2/chester/run/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-08 09:40:57.000000 madcat-7.2/chester/run/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1786 2023-02-11 11:52:10.000000 madcat-7.2/chester/run/chapter_titles.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2779 2023-02-08 21:21:02.000000 madcat-7.2/chester/run/feature_attention_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    16206 2023-03-21 07:53:41.000000 madcat-7.2/chester/run/full_run.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5035 2023-03-21 07:33:39.000000 madcat-7.2/chester/run/user_classes.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.634715 madcat-7.2/chester/run_manual_chester/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 13:32:50.000000 madcat-7.2/chester/run_manual_chester/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    19378 2023-07-20 13:06:20.000000 madcat-7.2/chester/run_manual_chester/manual_run.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      399 2023-07-20 10:55:05.000000 madcat-7.2/chester/run_manual_chester/pg.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.636764 madcat-7.2/chester/text_stats_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/text_stats_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1261 2023-02-14 11:53:21.000000 madcat-7.2/chester/text_stats_analysis/common_words.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3708 2023-07-20 11:01:12.000000 madcat-7.2/chester/text_stats_analysis/corex_topics.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4446 2023-03-21 07:33:39.000000 madcat-7.2/chester/text_stats_analysis/data_quality.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3466 2023-02-14 12:12:27.000000 madcat-7.2/chester/text_stats_analysis/key_sentences.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     3663 2023-02-14 12:20:36.000000 madcat-7.2/chester/text_stats_analysis/keywords_extraction.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1951 2023-02-14 14:04:54.000000 madcat-7.2/chester/text_stats_analysis/sentiment.py
+-rw-r--r--   0 amitosi    (501) staff       (20)    10355 2023-03-21 07:33:39.000000 madcat-7.2/chester/text_stats_analysis/smart_text_analyzer.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4118 2023-03-21 07:33:39.000000 madcat-7.2/chester/text_stats_analysis/text_summary.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      526 2023-02-11 16:14:05.000000 madcat-7.2/chester/text_stats_analysis/word_cloud.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     5304 2023-02-19 09:26:17.000000 madcat-7.2/chester/util.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.637262 madcat-7.2/chester/utils/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:59.000000 madcat-7.2/chester/utils/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.637855 madcat-7.2/chester/zero_break/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:58.000000 madcat-7.2/chester/zero_break/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)       89 2023-02-05 11:09:58.000000 madcat-7.2/chester/zero_break/get_or_else.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     8904 2023-07-19 14:09:20.000000 madcat-7.2/chester/zero_break/problem_specification.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1694 2023-03-11 12:21:56.000000 madcat-7.2/chester/zero_break/text_detector.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.638175 madcat-7.2/example_notebooks/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-03-11 13:38:57.000000 madcat-7.2/example_notebooks/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2981 2023-03-11 15:08:39.000000 madcat-7.2/example_notebooks/main.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.638857 madcat-7.2/madcat.egg-info/
+-rw-r--r--   0 amitosi    (501) staff       (20)      189 2023-07-20 13:52:06.000000 madcat-7.2/madcat.egg-info/PKG-INFO
+-rw-r--r--   0 amitosi    (501) staff       (20)     5766 2023-07-20 13:52:06.000000 madcat-7.2/madcat.egg-info/SOURCES.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)        1 2023-07-20 13:52:06.000000 madcat-7.2/madcat.egg-info/dependency_links.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)      273 2023-07-20 13:52:06.000000 madcat-7.2/madcat.egg-info/requires.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)       33 2023-07-20 13:52:06.000000 madcat-7.2/madcat.egg-info/top_level.txt
+-rw-r--r--   0 amitosi    (501) staff       (20)       38 2023-07-20 13:52:06.644258 madcat-7.2/setup.cfg
+-rw-r--r--   0 amitosi    (501) staff       (20)      559 2023-07-20 13:51:32.000000 madcat-7.2/setup.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.639263 madcat-7.2/tamtam/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:37:31.000000 madcat-7.2/tamtam/__init__.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.640326 madcat-7.2/tamtam/ab_feature_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 10:02:44.000000 madcat-7.2/tamtam/ab_feature_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      541 2023-02-23 10:19:25.000000 madcat-7.2/tamtam/ab_feature_analysis/ab_catboost.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1923 2023-03-21 07:53:41.000000 madcat-7.2/tamtam/ab_feature_analysis/ab_feature_analysis_class.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      348 2023-02-23 10:19:25.000000 madcat-7.2/tamtam/ab_feature_analysis/ab_partial_plot.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      402 2023-02-23 10:19:25.000000 madcat-7.2/tamtam/ab_feature_analysis/ab_tree_class.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.640710 madcat-7.2/tamtam/ab_info/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:44:45.000000 madcat-7.2/tamtam/ab_info/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     4011 2023-02-23 21:52:11.000000 madcat-7.2/tamtam/ab_info/ab_class.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.641240 madcat-7.2/tamtam/allocation_calculation/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 13:01:46.000000 madcat-7.2/tamtam/allocation_calculation/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1937 2023-02-22 14:13:02.000000 madcat-7.2/tamtam/allocation_calculation/bias_class.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.641637 madcat-7.2/tamtam/delta_analysis/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-23 07:37:32.000000 madcat-7.2/tamtam/delta_analysis/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     6199 2023-02-23 21:48:17.000000 madcat-7.2/tamtam/delta_analysis/delta_class.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2517 2023-02-23 21:45:56.000000 madcat-7.2/tamtam/manual_run.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.641975 madcat-7.2/tamtam/metrics_correlation/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 14:27:03.000000 madcat-7.2/tamtam/metrics_correlation/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2350 2023-02-23 14:45:57.000000 madcat-7.2/tamtam/metrics_correlation/metric_class.py
+-rw-r--r--   0 amitosi    (501) staff       (20)      964 2023-02-23 14:45:57.000000 madcat-7.2/tamtam/run.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.642332 madcat-7.2/tamtam/user_class/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 07:41:13.000000 madcat-7.2/tamtam/user_class/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     1895 2023-02-23 11:53:41.000000 madcat-7.2/tamtam/user_class/user_class.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.642917 madcat-7.2/tamtam/utils/
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-22 10:08:15.000000 madcat-7.2/tamtam/utils/__init__.py
+-rw-r--r--   0 amitosi    (501) staff       (20)       54 2023-02-22 16:12:56.000000 madcat-7.2/tamtam/utils/column_utils.py
+-rw-r--r--   0 amitosi    (501) staff       (20)       59 2023-02-22 16:24:31.000000 madcat-7.2/tamtam/utils/utils.py
+drwxr-xr-x   0 amitosi    (501) staff       (20)        0 2023-07-20 13:52:06.643839 madcat-7.2/tests/
+-rw-r--r--   0 amitosi    (501) staff       (20)     2501 2023-02-05 11:09:51.000000 madcat-7.2/tests/test_cleaning.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2119 2023-02-05 11:09:51.000000 madcat-7.2/tests/test_preprocessing.py
+-rw-r--r--   0 amitosi    (501) staff       (20)        0 2023-02-05 11:09:51.000000 madcat-7.2/tests/test_util.py
+-rw-r--r--   0 amitosi    (501) staff       (20)     2843 2023-02-05 11:09:58.000000 madcat-7.2/tests/test_zero_break.py
```

### Comparing `madcat-7.1/README.md` & `madcat-7.2/README.md`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/cleaning/cleaner_handler.py` & `madcat-7.2/chester/cleaning/cleaner_handler.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/cleaning/cleaning_func.py` & `madcat-7.2/chester/cleaning/cleaning_func.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/data_loader/webtext_data.py` & `madcat-7.2/chester/data_loader/webtext_data.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/feature_analyzing/feature_correlation.py` & `madcat-7.2/chester/feature_analyzing/feature_correlation.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/feature_stats/categorical_stats.py` & `madcat-7.2/chester/feature_stats/categorical_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,78 +30,94 @@
         sorted_cardinalities = sorted(cardinalities, key=lambda x: x[1], reverse=True)
         return [x[0] for x in sorted_cardinalities]
 
     def sample_top_features(self, n):
         top_features = self.cols_sorted[:3 * n]
         return top_features
 
-    def plot_value_counts(self, n=25, plot=True):
+    def plot_data(self, ax, count_data, col):
+        ax1 = ax
+        ax1.bar(count_data.iloc[:, 0], count_data['count'].to_list(), color='gray')
+        ax2 = ax1.twinx()
+        ax2.plot(count_data.iloc[:, 0], count_data['percentage'].to_list(), marker='o', color='red')
+        ax1.set_ylabel('Counts', color='gray')
+        ax2.set_ylabel('Percentages', color='red')
+        ax1.set_xlabel(None)
+        ax1.set_title(f"{col}")
+
+    def plot_value_counts(self, plot, n=25):
         if not self.any_categorical():
             return None
         if not plot:
             return None
         top_n = self.cols_sorted[:min(len(self.cols_sorted), n)]
-        num_plots = len(top_n)
-        if num_plots == 1:
-            col = top_n[0]
-            fig, ax1 = plt.subplots(1, 1, figsize=(10, 5))
-            cat_col = self.data[col].apply(lambda x: "cat " + str(x))
-            count_data = cat_col.value_counts()
-            percent_data = count_data / count_data.sum() * 100
-            ax1.bar(count_data.index[:5], count_data.values[:5], color='gray')
-            ax2 = ax1.twinx()
-            ax2.plot(percent_data.index[:5], percent_data.values[:5], color='red', marker='o')
-            ax1.set_ylabel('Counts', color='gray')
-            ax2.set_ylabel('Percentages', color='red')
-            ax1.set_xlabel(None)
-            ax1.set_title(f"{col}")
-            return None
-        else:
-            dim = max(math.floor(math.sqrt(len(top_n))), 2)
-            fig, ax = plt.subplots(dim, dim, figsize=(18, 3 + 3 * dim))
-            fig.tight_layout()
+
+        # Compute grid size
+        dim = max(math.floor(math.sqrt(len(top_n))), 2)
+
+        # Always make subplots, even when there is only one
+        fig, ax = plt.subplots(dim, dim, figsize=(18, 3 + 3 * dim))
+        fig.tight_layout()
+
+        # Iterate over the categorical columns and create plots
+        for i, col in enumerate(top_n):
+            if i >= dim * dim:
+                break
+
+            count_data = self.data[col].value_counts().reset_index()
+            count_data.columns = [col, 'count']
+            count_data['percentage'] = (count_data['count'] / count_data['count'].sum()) * 100
+
+            # Flatten axes array, if there is only one plot, ax does not need to be indexed
+            ax_i = ax.flatten()[i]
+
+            self.plot_data(ax_i, count_data, col)
+
+        # Add super title for all subplots, if there are more than one
+        if len(top_n) > 1:
             fig.suptitle("Top 5 Value Counts and Percentages for Each Feature")
-            for i, col in enumerate(top_n):
-                if i >= dim * dim:
-                    break
-                count_data = pd.DataFrame(self.data[col].value_counts().head(5)).reset_index(drop=False)
-                total_count = self.data[col].count()
-                percent_data = count_data.copy()
-                percent_data[col] = percent_data[col] / total_count * 100
-                percent_data.rename(columns={col: 'percentage', 'index': col}, inplace=True)
-
-                plot_title = f"{col}"
-                ax_i = ax[i // dim, i % dim]
-                ax1_i = ax_i
-                ax1_i.bar(count_data.iloc[:, 0], count_data.iloc[:, 1].to_list(), color='gray')
-                ax2_i = ax1_i.twinx()
-                ax2_i.plot(percent_data.iloc[:, 0], percent_data.iloc[:, 1].to_list(), marker='o', color='red')
-                ax1_i.set_ylabel('Counts', color='gray')
-                ax2_i.set_ylabel('Percentages', color='red')
-                ax1_i.set_xlabel(None)
-                ax1_i.set_title(plot_title)
-            plt.show()
-            plt.close()
+
+        plt.show()
+        plt.close()
 
     def calculate_stats(self, is_print=True):
         from chester.util import ReportCollector, REPORT_PATH
         rc = ReportCollector(REPORT_PATH)
         if not self.any_categorical():
             return None
         result_dicts = []
         for col in self.cols:
             data = self.data[col]
             unique_values = data.nunique()
             missing_values = data.isnull().sum()
-            value_counts = data.value_counts().rename("count").reset_index()
+
+            value_counts = data.value_counts().reset_index()
+            value_counts.columns = ["index", "count"]
             value_counts["percentage"] = 100 * value_counts["count"] / value_counts["count"].sum()
             value_counts = value_counts.sort_values("count", ascending=False)
+
             dist_str = ', '.join([f"{row['index']}: {row['percentage']:.0f}%" for _, row in value_counts.iterrows()])
-            result_dicts.append(
-                {'col': col, '# unique': unique_values, '# missing': missing_values, 'Distribution': dist_str})
+
+            # Find sample values
+            data_unique_values = data.dropna().drop_duplicates()
+            sample_values = ', '.join(
+                str(value) for value in data_unique_values.sample(min(3, len(data_unique_values))))
+
+            # Calculate top 5 values coverage
+            top_5_coverage = 100 * value_counts.head(5)["count"].sum() / value_counts["count"].sum()
+
+            result_dicts.append({
+                'col': col,
+                '# unique': unique_values,
+                '# missing': missing_values,
+                'Distribution': dist_str,
+                'Sample': sample_values,
+                'Top 5 values coverage': f"{top_5_coverage:.0f}%"
+            })
+
             data_unique_values = data.dropna().drop_duplicates()
             col_len = len(data_unique_values)
             values_to_sample = 3
             if col_len < values_to_sample:
                 values_to_sample = col_len
             sample_values = [str(value) for value in data_unique_values.sample(min(col_len, values_to_sample)).values]
             result_dicts[-1]['Sample'] = ', '.join(sample_values)
```

### Comparing `madcat-7.1/chester/feature_stats/numeric_stats.py` & `madcat-7.2/chester/feature_stats/numeric_stats.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/feature_stats/text_stats.py` & `madcat-7.2/chester/feature_stats/text_stats.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/feature_stats/time_series_stats.py` & `madcat-7.2/chester/feature_stats/time_series_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,10 +164,13 @@
         plt.close()
 
     def run_single(self, time_col, plot=True):
         self.plot_dates(time_col=time_col, time_freq=self.time_frequency, plot=plot)
 
     def run(self, plot=True):
         for time_col in self.time_cols:
-            self.run_single(time_col, plot)
-            self.plot_date_parts(time_col, plot)
-            self.plot_time_between_events(time_col, plot)
+            try:
+                self.run_single(time_col, plot)
+                self.plot_date_parts(time_col, plot)
+                self.plot_time_between_events(time_col, plot)
+            except:
+                pass
```

### Comparing `madcat-7.1/chester/feature_stats/utils.py` & `madcat-7.2/chester/feature_stats/utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/bag_of_words.py` & `madcat-7.2/chester/features_engineering/bag_of_words.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/corex.py` & `madcat-7.2/chester/features_engineering/corex.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/fe_nlp.py` & `madcat-7.2/chester/features_engineering/fe_nlp.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/feature_handler.py` & `madcat-7.2/chester/features_engineering/feature_handler.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/features_handler.py` & `madcat-7.2/chester/features_engineering/features_handler.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/tfidf.py` & `madcat-7.2/chester/features_engineering/tfidf.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/cyclic_features_utils.py` & `madcat-7.2/chester/features_engineering/time_series/cyclic_features_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/event_counter.py` & `madcat-7.2/chester/features_engineering/time_series/event_counter.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/feature_elimination_utils.py` & `madcat-7.2/chester/features_engineering/time_series/feature_elimination_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/frequencies_utils.py` & `madcat-7.2/chester/features_engineering/time_series/frequencies_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,18 @@
                  col_name,
                  time_series_handler: TimeSeriesHandler = None,
                  data_info: DataInfo = None):
         self.date_col_name = col_name  # the name of the date col
         # self.date_column = column
         self.time_series_handler = time_series_handler or TimeSeriesHandler()
         self.data_info = data_info
-        self.df = self.data_info.data.sort_values(self.date_col_name)
+        try:
+            self.df = self.data_info.data.sort_values(self.date_col_name)
+        except:
+            self.df = self.data_info.data
         self.id_cols = self.time_series_handler.id_cols or []
         self.lag_values = time_series_handler.lag_values
         self.df[self.date_col_name] = pd.to_datetime(self.df[self.date_col_name])  # convert to datetime
         self.time_between_events = None
         self.calculate_time_between_events()
         # self.target = self.df[self.data_info.target]
```

### Comparing `madcat-7.1/chester/features_engineering/time_series/get_time_freqeuency_utils.py` & `madcat-7.2/chester/features_engineering/time_series/get_time_freqeuency_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/moving_metric_utils.py` & `madcat-7.2/chester/features_engineering/time_series/moving_metric_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/features_engineering/time_series/ts_feature_extraction.py` & `madcat-7.2/chester/features_engineering/time_series/ts_feature_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,23 @@
         self.data_info.feature_types_val["numeric"].extend(target_df.columns)  # update features
 
     def freq_features(self):
         ff = FrequenciesFeatures(column=self.column,
                                  col_name=self.col_name,
                                  time_series_handler=self.time_series_handler,
                                  data_info=self.data_info)
-        df_ff, names = ff.run()
-        df_ff = FeatureEliminationUtils(df=df_ff[names]).run()  # Elimination for the relevant features only
-        self.data_info.data = pd.concat([self.data_info.data, df_ff], axis=1)  # update data
-        self.data_info.feature_types_val["numeric"] = list(
-            self.data_info.feature_types_val["numeric"])  # convert set to list
-        self.data_info.feature_types_val["numeric"].extend(df_ff.columns)  # update features
+        try:
+            df_ff, names = ff.run()
+            df_ff = FeatureEliminationUtils(df=df_ff[names]).run()  # Elimination for the relevant features only
+            self.data_info.data = pd.concat([self.data_info.data, df_ff], axis=1)  # update data
+            self.data_info.feature_types_val["numeric"] = list(
+                self.data_info.feature_types_val["numeric"])  # convert set to list
+            self.data_info.feature_types_val["numeric"].extend(df_ff.columns)  # update features
+        except:
+            pass
 
     def cyclic_features(self):
         cf = CyclicFeatures(column=self.column,
                             col_name=self.col_name,
                             time_series_handler=self.time_series_handler,
                             data_info=self.data_info)
         df_cf, names = cf.run()
```

### Comparing `madcat-7.1/chester/features_engineering/time_series/ts_features_extraction.py` & `madcat-7.2/chester/features_engineering/time_series/ts_features_extraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,19 @@
                  ):
         self.time_series_handler = time_series_handler or TimeSeriesHandler()
         self.data_info = data_info
         self.cols = self.data_info.feature_types_val["time"]
 
     def run(self):
         for col in self.cols:
-            ts_fe = TimeSeriesFeatureExtraction(
-                data_info=self.data_info,
-                time_series_handler=self.time_series_handler,
-                col_name=col,
-                column=self.data_info.data[col]
-            )
-            ts_fe.run()
-            self.data_info = ts_fe.data_info
+            try:
+                ts_fe = TimeSeriesFeatureExtraction(
+                    data_info=self.data_info,
+                    time_series_handler=self.time_series_handler,
+                    col_name=col,
+                    column=self.data_info.data[col]
+                )
+                ts_fe.run()
+                self.data_info = ts_fe.data_info
+            except:
+                pass
             # print("updated data info after ts", self.data_info)
```

### Comparing `madcat-7.1/chester/model_analyzer/model_analysis.py` & `madcat-7.2/chester/model_analyzer/model_analysis.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_monitor/calculate_scores_utils.py` & `madcat-7.2/chester/model_monitor/calculate_scores_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_monitor/error_prediction.py` & `madcat-7.2/chester/model_monitor/error_prediction.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_monitor/model_boostrap.py` & `madcat-7.2/chester/model_monitor/model_boostrap.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/data_preparation.py` & `madcat-7.2/chester/model_training/data_preparation.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/model_utils.py` & `madcat-7.2/chester/model_training/model_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/base_model.py` & `madcat-7.2/chester/model_training/models/chester_models/base_model.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/base_model_utils.py` & `madcat-7.2/chester/model_training/models/chester_models/base_model_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/baseline/baseline_model.py` & `madcat-7.2/chester/model_training/models/chester_models/baseline/baseline_model.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/baseline/baseline_utils.py` & `madcat-7.2/chester/model_training/models/chester_models/baseline/baseline_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/best_baseline_model.py` & `madcat-7.2/chester/model_training/models/chester_models/best_baseline_model.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/best_linear_regression.py` & `madcat-7.2/chester/model_training/models/chester_models/best_linear_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
     def get_best_model(self):
         models = self.data_info.model_selection_val
         metrics = self.get_metrics_functions()
         if models is None:
             return None
         else:
-            models = [model for model in models if "catboost" in model]
-            # print("models", models)
             if len(models) == 0:
                 return None
             else:
                 results = []
                 for _ in models:
                     for params in self.hp_list:
                         base_res, model = linear_regression_with_outputs(
```

### Comparing `madcat-7.1/chester/model_training/models/chester_models/best_logistic_regression.py` & `madcat-7.2/chester/model_training/models/chester_models/best_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/best_model.py` & `madcat-7.2/chester/model_training/models/chester_models/best_model.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/compare_utils.py` & `madcat-7.2/chester/model_training/models/chester_models/compare_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/hp_generator.py` & `madcat-7.2/chester/model_training/models/chester_models/hp_generator.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/linear_regression/linear_regression.py` & `madcat-7.2/chester/model_training/models/chester_models/linear_regression/linear_regression.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py` & `madcat-7.2/chester/model_training/models/chester_models/linear_regression/linear_regression_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py` & `madcat-7.2/chester/model_training/models/chester_models/logistic_regression/logistic_regression_model.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py` & `madcat-7.2/chester/model_training/models/chester_models/logistic_regression/logistic_regression_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/cv_training.py` & `madcat-7.2/chester/model_training/models/cv_training.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/lstm.py` & `madcat-7.2/chester/model_training/models/lstm.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/model_training/models/scoring.py` & `madcat-7.2/chester/model_training/models/scoring.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/post_model_analysis/post_model_analysis_class.py` & `madcat-7.2/chester/post_model_analysis/post_model_analysis_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/post_model_analysis/post_regression.py` & `madcat-7.2/chester/post_model_analysis/post_regression.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/pre_model_analysis/categorical.py` & `madcat-7.2/chester/pre_model_analysis/categorical.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/pre_model_analysis/numerics.py` & `madcat-7.2/chester/pre_model_analysis/numerics.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/pre_model_analysis/target.py` & `madcat-7.2/chester/pre_model_analysis/target.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/pre_model_analysis/time_series.py` & `madcat-7.2/chester/pre_model_analysis/time_series.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/preprocessing/preprocessing_func.py` & `madcat-7.2/chester/preprocessing/preprocessing_func.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/preprocessing/preprocessor_handler.py` & `madcat-7.2/chester/preprocessing/preprocessor_handler.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/run/chapter_titles.py` & `madcat-7.2/chester/run/chapter_titles.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/run/feature_attention_utils.py` & `madcat-7.2/chester/run/feature_attention_utils.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/run/full_run.py` & `madcat-7.2/chester/run/full_run.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/run/user_classes.py` & `madcat-7.2/chester/run/user_classes.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/run_manual_chester/manual_run.py` & `madcat-7.2/chester/run_manual_chester/manual_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-import random
 from collections import Counter
 
-import matplotlib
 import pandas as pd
-from chester.data_loader.webtext_data import load_data_pirates, load_data_king_arthur, load_data_chat_logs
-from flatbuffers.builder import np
-from sklearn.datasets import fetch_20newsgroups, fetch_openml
+from sklearn.datasets import fetch_20newsgroups
+from matplotlib import pyplot as plt
 
+from chester.data_loader.webtext_data import load_data_pirates, load_data_king_arthur, load_data_chat_logs
 from chester.run.full_run import run
-from chester.run.user_classes import Data, ModelRun, TimeSeriesHandler, TextFeatureExtraction, TextSummary
-import yfinance as yf
-import ml_datasets
+from chester.run.user_classes import Data, TextSummary, ModelRun
 
 # matplotlib.use('TkAgg')
 target_column = 'target'
-import matplotlib.pyplot as plt
-
+import numpy as np
 # Disable interactive mode
 # plt.ioff()
 
 
 ################################################################################################
-df1 = load_data_pirates().assign(target='pirate').sample(300, replace=True)
-df2 = load_data_king_arthur().assign(target='arthur').sample(300, replace=True)
-df3 = load_data_chat_logs().assign(target='chat').sample(300, replace=True)
-df = pd.concat([
-    df1, df2,
-    df3
-])
+# df1 = load_data_pirates().assign(target='pirate').sample(300, replace=True)
+# df2 = load_data_king_arthur().assign(target='arthur').sample(300, replace=True)
+# df3 = load_data_chat_logs().assign(target='chat').sample(300, replace=True)
+# df = pd.concat([
+#     df1, df2,
+#     df3
+# ])
+
+
 #
 # df['target'] = df['target'].apply(lambda x: 0 if "pirate" in x else 1)  # can do with or without
 ################################################################################################
 
 
 ################################################################################################
 # url = "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data"
@@ -384,15 +381,15 @@
 # df = load_dataset('tae')
 # df = load_dataset('heart-c')
 # df = load_dataset('tic-tac-toe')
 # df = load_dataset('heart-h')
 # df = load_dataset('trains')
 # df = load_dataset('heart-statlog')
 # df = load_dataset('vehicle')
-# df = load_dataset('hepatitis')
+df = load_dataset('hepatitis')
 # df = load_dataset('vote')
 # df = load_dataset('hypothyroid')
 
 
 # df = load_dataset('ionosphere')
 # df = load_dataset('waveform-5000')
 # df = load_dataset('iris')
@@ -428,22 +425,25 @@
 # df = load_dataset('yokohoma2')
 # df = load_dataset('cpu_small')
 
 # top_10 = df['ProductId'].value_counts().nlargest(10).index
 # filtered_df = df[df['ProductId'].isin(top_10)]
 
 
-chester_collector = run(Data(df=df),
-                        is_feature_stats=True,
-                        is_pre_model=True,
-                        text_summary=TextSummary(summary_num_sentences=3, max_terms=5),
+# df = pd.read_csv("/Users/amitosi/PycharmProjects/databot_aws/example_app/static/iris_data.csv")
+# df['target'] = df.apply(lambda x: str(x['target']) + "class", axis=1)
+
+chester_collector = run(Data(df=df, target_column='target'),
+                        # is_feature_stats=True,
+                        # is_pre_model=True,
+                        # text_summary=TextSummary(summary_num_sentences=3, max_terms=5),
                         # feature_types={'numeric': [], 'boolean': [], 'text': ['Text', 'Summary'],
                         #                'categorical': [], 'time': [], 'id': ['ProductId']}
                         # text_summary=TextSummary(summary_num_sentences=3, max_terms=20),
-                        # model_run=ModelRun(n_models=1),
+                        model_run=ModelRun(n_models=2),
                         )
 # madcat_collector = run_madcat(Data(df=df, target_column='target'),
 #                               is_feature_stats=True,
 #                               # text_feature_extraction=TextFeatureExtraction(corex_dim=2, anchor_words=anchors),
 #                               # time_series_handler=TimeSeriesHandler(id_cols=["id"]),
 #                               is_pre_model=False,
 #                               is_model_training=False,
```

### Comparing `madcat-7.1/chester/text_stats_analysis/common_words.py` & `madcat-7.2/chester/text_stats_analysis/common_words.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/corex_topics.py` & `madcat-7.2/chester/text_stats_analysis/corex_topics.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/data_quality.py` & `madcat-7.2/chester/text_stats_analysis/data_quality.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/key_sentences.py` & `madcat-7.2/chester/text_stats_analysis/key_sentences.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/keywords_extraction.py` & `madcat-7.2/chester/text_stats_analysis/keywords_extraction.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/sentiment.py` & `madcat-7.2/chester/text_stats_analysis/sentiment.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/smart_text_analyzer.py` & `madcat-7.2/chester/text_stats_analysis/smart_text_analyzer.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/text_summary.py` & `madcat-7.2/chester/text_stats_analysis/text_summary.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/text_stats_analysis/word_cloud.py` & `madcat-7.2/chester/text_stats_analysis/word_cloud.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/util.py` & `madcat-7.2/chester/util.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/zero_break/problem_specification.py` & `madcat-7.2/chester/zero_break/problem_specification.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/chester/zero_break/text_detector.py` & `madcat-7.2/chester/zero_break/text_detector.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/example_notebooks/main.py` & `madcat-7.2/example_notebooks/main.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/madcat.egg-info/SOURCES.txt` & `madcat-7.2/madcat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,16 @@
 chester/preprocessing/preprocessor_handler.py
 chester/run/__init__.py
 chester/run/chapter_titles.py
 chester/run/feature_attention_utils.py
 chester/run/full_run.py
 chester/run/user_classes.py
 chester/run_manual_chester/__init__.py
-chester/run_manual_chester/bad_data.py
-chester/run_manual_chester/bad_data2.py
 chester/run_manual_chester/manual_run.py
+chester/run_manual_chester/pg.py
 chester/text_stats_analysis/__init__.py
 chester/text_stats_analysis/common_words.py
 chester/text_stats_analysis/corex_topics.py
 chester/text_stats_analysis/data_quality.py
 chester/text_stats_analysis/key_sentences.py
 chester/text_stats_analysis/keywords_extraction.py
 chester/text_stats_analysis/sentiment.py
```

### Comparing `madcat-7.1/setup.py` & `madcat-7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('requirements.txt') as f:
     install_requires = f.read().strip().split('\n')
 
 setuptools.setup(
     name="madcat",
-    version="7.01",
+    version="7.02",
     author="Amit Osi",
     author_email="amitosi6666@gmail.com",
     description=open('README.md').read(),
     url="https://github.com/amito-ds/chester",
     packages=setuptools.find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.8",
```

### Comparing `madcat-7.1/tamtam/ab_feature_analysis/ab_catboost.py` & `madcat-7.2/tamtam/ab_feature_analysis/ab_catboost.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/ab_feature_analysis/ab_feature_analysis_class.py` & `madcat-7.2/tamtam/ab_feature_analysis/ab_feature_analysis_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/ab_info/ab_class.py` & `madcat-7.2/tamtam/ab_info/ab_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/allocation_calculation/bias_class.py` & `madcat-7.2/tamtam/allocation_calculation/bias_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/delta_analysis/delta_class.py` & `madcat-7.2/tamtam/delta_analysis/delta_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/manual_run.py` & `madcat-7.2/tamtam/manual_run.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/metrics_correlation/metric_class.py` & `madcat-7.2/tamtam/metrics_correlation/metric_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/run.py` & `madcat-7.2/tamtam/run.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tamtam/user_class/user_class.py` & `madcat-7.2/tamtam/user_class/user_class.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tests/test_cleaning.py` & `madcat-7.2/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tests/test_preprocessing.py` & `madcat-7.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `madcat-7.1/tests/test_zero_break.py` & `madcat-7.2/tests/test_zero_break.py`

 * *Files identical despite different names*

