# Comparing `tmp/dataquality-0.9.7.tar.gz` & `tmp/dataquality-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataquality-0.9.7.tar", last modified: Fri Jul 14 21:09:18 2023, max compression
+gzip compressed data, was "dataquality-0.9.8.tar", last modified: Thu Jul 20 19:02:14 2023, max compression
```

## Comparing `dataquality-0.9.7.tar` & `dataquality-0.9.8.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 21:08:51.000000 dataquality-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-14 21:09:18.336846 dataquality-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-14 21:08:51.000000 dataquality-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/clients/objectstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/core/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/dq_auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/base_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/ner_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/tc_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_auto/text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/dq_start/
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dq_start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/torch_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/transformers_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/integrations/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/base_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.324846 dataquality-0.9.7/dataquality/loggers/data_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/base_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/data_logger/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/loggers/logger_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/base_logger_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/logger_config/text_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/loggers/model_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/base_model_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/loggers/model_logger/text_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.328846 dataquality-0.9.7/dataquality/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/schemas/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/dataquality/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ampli.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/auto_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/dq_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/dqyolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hdf5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hf_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/hf_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/od.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/dataquality/utils/semantic_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/semantic_segmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/setfit.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/ultralytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/vaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 21:08:51.000000 dataquality-0.9.7/dataquality/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.320846 dataquality-0.9.7/dataquality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 21:09:18.000000 dataquality-0.9.7/dataquality.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-14 21:08:51.000000 dataquality-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 21:09:18.336846 dataquality-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:08:51.000000 dataquality-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_dataquality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_telemetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:09:18.336846 dataquality-0.9.7/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_integration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/hf_integration_constants_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/ner_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/pt_datasets_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-14 21:08:51.000000 dataquality-0.9.7/tests/test_utils/tc_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.914943 dataquality-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-20 19:00:44.000000 dataquality-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-20 19:02:14.914943 dataquality-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-20 19:00:44.000000 dataquality-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.838934 dataquality-0.9.8/dataquality/
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.838934 dataquality-0.9.8/dataquality/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/clients/objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.842935 dataquality-0.9.8/dataquality/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/core/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.846935 dataquality-0.9.8/dataquality/dq_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/base_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/ner_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/tc_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_auto/text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.846935 dataquality-0.9.8/dataquality/dq_start/
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dq_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.850936 dataquality-0.9.8/dataquality/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/torch_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/transformers_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/integrations/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.850936 dataquality-0.9.8/dataquality/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/base_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.854936 dataquality-0.9.8/dataquality/loggers/data_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27255 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/base_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/data_logger/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.874938 dataquality-0.9.8/dataquality/loggers/logger_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/base_logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/logger_config/text_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.882939 dataquality-0.9.8/dataquality/loggers/model_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/base_model_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/text_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32097 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/loggers/model_logger/text_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.886940 dataquality-0.9.8/dataquality/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/schemas/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.902942 dataquality-0.9.8/dataquality/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/ampli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/auto_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/dq_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/dqyolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/hf_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/hf_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/od.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.906942 dataquality-0.9.8/dataquality/utils/semantic_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/semantic_segmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/setfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25812 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/ultralytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/vaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 19:00:44.000000 dataquality-0.9.8/dataquality/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.838934 dataquality-0.9.8/dataquality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 19:02:14.000000 dataquality-0.9.8/dataquality.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-20 19:00:44.000000 dataquality-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 19:02:14.914943 dataquality-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:00:44.000000 dataquality-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.910943 dataquality-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_dataquality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_telemetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:02:14.914943 dataquality-0.9.8/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/hf_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/hf_integration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/hf_integration_constants_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/ner_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/pt_datasets_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-20 19:00:44.000000 dataquality-0.9.8/tests/test_utils/tc_constants.py
```

### Comparing `dataquality-0.9.7/LICENSE` & `dataquality-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/PKG-INFO` & `dataquality-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.7
+Version: 0.9.8
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.7/README.md` & `dataquality-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/__init__.py` & `dataquality-0.9.8/dataquality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import dataquality
     with dataquality(labels = ["neg", "pos"],
                      train_data = train_data):
         dataquality.get_insights()
 """
 
 
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 import sys
 from typing import Any, List, Optional
 
 import dataquality.core._config
 import dataquality.integrations
```

### Comparing `dataquality-0.9.7/dataquality/analytics.py` & `dataquality-0.9.8/dataquality/analytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/clients/api.py` & `dataquality-0.9.8/dataquality/clients/api.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/clients/objectstore.py` & `dataquality-0.9.8/dataquality/clients/objectstore.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/__init__.py` & `dataquality-0.9.8/dataquality/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/_config.py` & `dataquality-0.9.8/dataquality/core/_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/auth.py` & `dataquality-0.9.8/dataquality/core/auth.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/finish.py` & `dataquality-0.9.8/dataquality/core/finish.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/init.py` & `dataquality-0.9.8/dataquality/core/init.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/core/log.py` & `dataquality-0.9.8/dataquality/core/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,7 +629,9 @@
     assert isinstance(
         tokenizer, PreTrainedTokenizerFast
     ), "Tokenizer must be an instance of PreTrainedTokenizerFast"
     assert getattr(tokenizer, "is_fast", False), "Tokenizer must be a fast tokenizer"
     for attr in ["encode", "decode", "encode_plus", "padding_side"]:
         assert hasattr(tokenizer, attr), f"Tokenizer must support `{attr}`"
     seq2seq_logger_config.tokenizer = tokenizer
+    # Seq2Seq doesn't have labels but we need to set this to avoid validation errors
+    seq2seq_logger_config.labels = []
```

### Comparing `dataquality-0.9.7/dataquality/core/report.py` & `dataquality-0.9.8/dataquality/core/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/auto.py` & `dataquality-0.9.8/dataquality/dq_auto/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/base_data_manager.py` & `dataquality-0.9.8/dataquality/dq_auto/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/ner.py` & `dataquality-0.9.8/dataquality/dq_auto/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/ner_trainer.py` & `dataquality-0.9.8/dataquality/dq_auto/ner_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/notebook.py` & `dataquality-0.9.8/dataquality/dq_auto/notebook.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/tc_trainer.py` & `dataquality-0.9.8/dataquality/dq_auto/tc_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_auto/text_classification.py` & `dataquality-0.9.8/dataquality/dq_auto/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dq_start/__init__.py` & `dataquality-0.9.8/dataquality/dq_start/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/dqyolo.py` & `dataquality-0.9.8/dataquality/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/integrations/fastai.py` & `dataquality-0.9.8/dataquality/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/integrations/hf.py` & `dataquality-0.9.8/dataquality/integrations/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/integrations/keras.py` & `dataquality-0.9.8/dataquality/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/integrations/setfit.py` & `dataquality-0.9.8/dataquality/integrations/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/integrations/torch.py` & `dataquality-0.9.8/dataquality/integrations/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,41 +146,42 @@
         """Log the embeddings, ids and logits.
 
         We save the embeddings and logits in a dict called model_output_store
         in the helper data. This is because the embeddings and logits are
         extracted in the hooks and we need to log them in the on_step_end
         method.
         """
+
         model_outputs_store = self.torch_helper_data.model_outputs_store
         # Workaround for multiprocessing
-        if model_outputs_store.get("ids") is None and len(
+        if model_outputs_store.ids is None and len(
             self.torch_helper_data.dl_next_idx_ids
         ):
-            model_outputs_store["ids"] = self.torch_helper_data.dl_next_idx_ids.pop(0)
+            model_outputs_store.ids = self.torch_helper_data.dl_next_idx_ids.pop(0)
 
         # Log only if embedding exists
-        assert model_outputs_store.get("embs") is not None, GalileoException(
+        assert model_outputs_store.embs is not None, GalileoException(
             "Embedding passed to the logger can not be logged"
         )
-        assert model_outputs_store.get("logits") is not None, GalileoException(
+        assert model_outputs_store.logits is not None, GalileoException(
             "Logits passed to the logger can not be logged"
         )
-        assert model_outputs_store.get("ids") is not None, GalileoException(
+        assert model_outputs_store.ids is not None, GalileoException(
             "id column missing in dataset (needed to map rows to the indices/ids)"
         )
         # Convert the indices to ids
         cur_split = self.logger_config.cur_split
         assert cur_split is not None, GalileoException(
             "Current split must be set before logging"
         )
         cur_split = cur_split.lower()  # type: ignore
-        model_outputs_store["ids"] = map_indices_to_ids(
-            self.logger_config.idx_to_id_map[cur_split], model_outputs_store["ids"]
+        model_outputs_store.ids = map_indices_to_ids(
+            self.logger_config.idx_to_id_map[cur_split], model_outputs_store.ids
         )
-        dq.log_model_outputs(**model_outputs_store)
+        dq.log_model_outputs(**model_outputs_store.to_dict())
         model_outputs_store.clear()
 
 
 def watch(
     model: Module,
     dataloaders: Optional[List[DataLoader]] = [],
     classifier_layer: Optional[Union[str, Module]] = None,
```

### Comparing `dataquality-0.9.7/dataquality/integrations/torch_semantic_segmentation.py` & `dataquality-0.9.8/dataquality/integrations/torch_semantic_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,20 @@
         :param model_input: Model input of the current layer
         :param model_output: Model output of the current layer
         """
         if isinstance(model_output, dict) and "out" in model_output:
             logits = model_output["out"]
         else:
             logits = model_output
+        if not isinstance(logits, Tensor):
+            raise ValueError(
+                "Logits are not a tensor. Please ensure the logits are a tensor."
+            )
         model_outputs_store = self.torch_helper_data.model_outputs_store
-        model_outputs_store["logits"] = logits
+        model_outputs_store.logits = logits
 
     def _dq_classifier_hook_with_step_end(
         self,
         model: Module,
         model_input: torch.Tensor,
         model_output: Union[Any, torch.Tensor],
     ) -> None:
@@ -201,15 +205,15 @@
 
         :param model: torch.nn.Module segmentation model
         :param model_input: torch.Tensor input to the model - an image (bs, 3, h, w)
         :param model_output: torch.Tensor output of the model
 
         """
         # model input comes as a tuple of length 1
-        self.torch_helper_data.model_input = model_input[0].detach().cpu().numpy()
+        self.torch_helper_data.model_input = model_input[0].detach().cpu()
 
     def get_image_ids_and_image_paths(
         self, split: str, logging_data: Dict[str, Any]
     ) -> Tuple[List[int], List[str]]:
         img_ids = self.torch_helper_data.batch["ids"]  # np.ndarray (bs,)
         # convert the img_ids to absolute ids from file map
         img_ids = [
@@ -355,19 +359,29 @@
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Helper function to get the argmax and probs from the model outputs
 
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: argmax and logits tensors
         """
         # resize the logits to the input size based on hooks
-        preds = self.torch_helper_data.model_outputs_store["logits"]
+        preds = self.torch_helper_data.model_outputs_store.logits
+        if preds is None:
+            raise ValueError(
+                "Logits are missing in dataquality,"
+                " have connected to the right model layer?"
+            )
+        elif not isinstance(preds, Tensor):
+            raise ValueError(
+                f"Logits are not a tensor. Please ensure the logits are a tensor. \
+                Got {type(preds)}"
+            )
         if preds.dtype == torch.float16:
             preds = preds.to(torch.float32)
         input_shape = self.torch_helper_data.model_input.shape[-2:]
-        preds = F.interpolate(preds, size=input_shape, mode="bilinear")
+        preds = Tensor(F.interpolate(preds, size=input_shape, mode="bilinear"))
 
         # checks whether the model is (n, classes, w, h), or (n, w, h, classes)
         # takes the max in case of binary classification
         if max(preds.shape[1], 2) == self.number_classes:
             preds = preds.permute(0, 2, 3, 1)
         assert (
             max(preds.shape[3], 2) == self.number_classes
@@ -390,17 +404,26 @@
         """Function to be called at the end of step to log the inputs and outputs"""
         if not self.mask_col_name:
             self.find_mask_category(self.torch_helper_data.batch["data"])
 
         # if we have not inferred the number of classes from the model architecture
 
         # takes the max of the logits shape and 2 in case of binary classification
-        self.number_classes = max(
-            self.torch_helper_data.model_outputs_store["logits"].shape[1], 2
-        )
+        logits = self.torch_helper_data.model_outputs_store.logits
+        if logits is None:
+            raise ValueError(
+                "Logits are missing in dataquality,"
+                " have connected to the right model layer?"
+            )
+        elif not isinstance(logits, Tensor):
+            raise ValueError(
+                f"Logits are not a tensor. Please ensure the logits are a tensor. \
+                Got {type(logits)}"
+            )
+        self.number_classes = max(logits.shape[1], 2)
         if not self.init_lm_labels_flag:
             self._init_lm_labels()
             self.init_lm_labels_flag = True
         split = self.logger_config.cur_split.lower()  # type: ignore
         with torch.no_grad():
             logging_data = self.torch_helper_data.batch["data"]
             img_ids, image_paths = self.get_image_ids_and_image_paths(
```

### Comparing `dataquality-0.9.7/dataquality/integrations/transformers_trainer.py` & `dataquality-0.9.8/dataquality/integrations/transformers_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,29 @@
         self.logits_fn = logits_fn
         self._init_dimension(embedding_dim, logits_dim)
         self.trainer = trainer
 
     def _do_log(self) -> None:
         """Log the model outputs (called by the hook)"""
         # Log only if embedding exists
-        assert self.model_outputs_store.get("embs") is not None, GalileoException(
+        self.model_outputs_store.ids = self.model_outputs_store.ids_queue.pop(0)
+        assert self.model_outputs_store.embs is not None, GalileoException(
             "Embedding passed to the logger can not be logged"
         )
-        assert self.model_outputs_store.get("logits") is not None, GalileoException(
+        assert self.model_outputs_store.logits is not None, GalileoException(
             "Logits passed to the logger can not be logged"
         )
-        assert self.model_outputs_store.get("ids") is not None, GalileoException(
+        assert self.model_outputs_store.ids is not None, GalileoException(
             "Did you map IDs to your dataset before watching the model? You can run:\n"
             "`ds= dataset.map(lambda x, idx: {'id': idx}, with_indices=True)`\n"
             "id (index) column is needed in the dataset for logging"
         )
 
         # 🔭🌕 Galileo logging
-        dq.log_model_outputs(**self.model_outputs_store)
+        dq.log_model_outputs(**self.model_outputs_store.to_dict())
         self.model_outputs_store.clear()
 
     def validate(
         self,
         args: TrainingArguments,
         state: TrainerState,
         control: TrainerControl,
```

### Comparing `dataquality-0.9.7/dataquality/integrations/ultralytics.py` & `dataquality-0.9.8/dataquality/integrations/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/internal.py` & `dataquality-0.9.8/dataquality/internal.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/base_logger.py` & `dataquality-0.9.8/dataquality/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/__init__.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/base_data_logger.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/base_data_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/image_classification.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/object_detection.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/semantic_segmentation.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/seq2seq.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/seq2seq.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from dataquality.loggers.data_logger.base_data_logger import (
     ITER_CHUNK_SIZE,
     BaseGalileoDataLogger,
     DataSet,
     MetasType,
 )
 from dataquality.loggers.logger_config.seq2seq import seq2seq_logger_config
-from dataquality.schemas.seq2seq import Seq2SeqCols as C
+from dataquality.schemas.dataframe import BaseLoggerDataFrames
+from dataquality.schemas.seq2seq import Seq2SeqInputCols as C
 from dataquality.schemas.split import Split
 from dataquality.utils.seq2seq import (
     align_tokens_to_character_spans,
 )
 from dataquality.utils.vaex import rename_df
 
 if TYPE_CHECKING:
@@ -63,14 +64,15 @@
     training. This must be true in order to align inputs and outputs correctly. Ensure
     all necessary properties (like `add_eos_token`) are set before setting your
     tokenizer so as to match the tokenization process to your training process.
     """
 
     __logger_name__ = "seq2seq"
     logger_config = seq2seq_logger_config
+    DATA_FOLDER_EXTENSION = {"emb": "hdf5", "prob": "hdf5", "data": "arrow"}
 
     def __init__(self, meta: Optional[MetasType] = None) -> None:
         super().__init__(meta)
         # Tokens IDs in a given input string
         self.tokenized_labels: List[List[int]] = []
         # Character offsets for each token (from tokenized_inputs) in the dataset
         self.token_label_offsets: List[List[Tuple[int, int]]] = []
@@ -182,7 +184,39 @@
     @staticmethod
     def get_valid_attributes() -> List[str]:
         """
         Returns a list of valid attributes that for this Logger class
         :return: List[str]
         """
         return list(map(lambda x: x.value, C))
+
+    @classmethod
+    def _get_prob_cols(cls) -> List[str]:
+        return ["id"]
+
+    @classmethod
+    def separate_dataframe(
+        cls, df: DataFrame, prob_only: bool = True, split: Optional[str] = None
+    ) -> BaseLoggerDataFrames:
+        """Separates the singular dataframe into its 3 components
+
+        Gets the probability df, the embedding df, and the "data" df containing
+        all other columns
+        """
+        df_copy = df.copy()
+        # Separate out embeddings and probabilities into their own files
+        prob_cols = cls._get_prob_cols()
+        prob = df_copy[prob_cols]
+
+        if prob_only:  # In this case, we don't care about the other columns
+            emb_cols = ["id"]
+            other_cols = ["id"]
+        else:
+            emb_cols = ["id", "emb", "x", "y", "emb_pca"]
+            emb_cols = [c for c in emb_cols if c in df_copy.get_column_names()]
+            ignore_cols = ["split_id"] + prob_cols + emb_cols
+            other_cols = [i for i in df_copy.get_column_names() if i not in ignore_cols]
+            other_cols += ["id"]
+
+        emb = df_copy[emb_cols]
+        data_df = df_copy[other_cols]
+        return BaseLoggerDataFrames(prob=prob, emb=emb, data=data_df)
```

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/tabular_classification.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/text_classification.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/text_multi_label.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/data_logger/text_ner.py` & `dataquality-0.9.8/dataquality/loggers/data_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/base_logger_config.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/base_logger_config.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/object_detection.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/seq2seq.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/text_classification.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/text_multi_label.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/logger_config/text_ner.py` & `dataquality-0.9.8/dataquality/loggers/logger_config/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/base_model_logger.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/base_model_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/image_classification.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/image_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/object_detection.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/object_detection.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/semantic_segmentation.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/seq2seq.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/seq2seq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pyarrow as pa
 
 from dataquality.loggers.logger_config.seq2seq import seq2seq_logger_config
 from dataquality.loggers.model_logger.base_model_logger import BaseGalileoModelLogger
-from dataquality.schemas.seq2seq import Seq2SeqCols as C
+from dataquality.schemas.seq2seq import Seq2SeqOutputCols as C
 from dataquality.schemas.split import Split
 from dataquality.utils.arrow import save_arrow_file
 
 
 class Seq2SeqModelLogger(BaseGalileoModelLogger):
     __logger_name__ = "seq2seq"
     logger_config = seq2seq_logger_config
@@ -66,29 +66,42 @@
         self.token_dep, self.token_gold_probs = self.get_token_dep_probs(
             self.ids, probs
         )
 
     def get_dep_for_sample(
         self, sample_id: int, sample_probs: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
+        """Extracts DEP per token prediction for a single sample
+
+        Args:
+            sample_id: The sample id
+            sample_probs: The probabilities for each token in the sample
+                sample_probs.shape is [max_token_len, vocab_size]
+
+        Returns:
+            dep: The DEP per token prediction for the sample
+                dep.shape is [num_tokens_in_label]
+            gold_probs: The probabilities of the GT token label for the sample
+                gold_probs.shape is [num_tokens_in_label]
+        """
         assert (
             self.logger_config.tokenizer is not None
         ), "Must set your tokenizer. Use `dq.set_tokenizer`"
         labels = self.logger_config.id_to_tokens[self.token_map_key][sample_id]
         if self.logger_config.tokenizer.padding_side == "left":
             probs = sample_probs[-len(labels) :]
         else:
             probs = sample_probs[: len(labels)]
         gold_probs = probs[np.arange(len(labels)), labels]
         probs_copy = probs.copy()
         probs_copy[np.arange(len(labels)), labels] = 0
         # Max non-gold probability
         max_probs = np.max(probs_copy, axis=-1)
-        aum = gold_probs - max_probs
-        dep = (1 - aum) / 2
+        margin = gold_probs - max_probs
+        dep = (1 - margin) / 2
         return dep, gold_probs
 
     def get_token_dep_probs(
         self, batch_ids: np.ndarray, batch_probs: np.ndarray
     ) -> Tuple[pa.array, pa.array]:
         """Extracts DEP per token prediction
 
@@ -110,14 +123,20 @@
         for that sample that are ignored/padded are indexed out by this function.
         So we use that to get only the ones we care about.
 
         We return a pyarrow array because each batch will have a different shape, which
         can't be represented in numpy
 
         Returns: (token_dep, gold_probs)
+            token_dep: The DEP per token prediction for the batch
+                len(token_dep) == batch_size
+                token_dep[i].shape is [num_tokens_in_label]
+            gold_probs: The probabilities of the GT token label for the batch
+                len(gold_probs) == batch_size
+                gold_probs[i].shape is [num_tokens_in_label]
         """
         batch_deps = []
         batch_gold_probs = []
         for sample_id, sample_probs in zip(batch_ids, batch_probs):
             dep, gold_probs = self.get_dep_for_sample(sample_id, sample_probs)
             batch_deps.append(dep)
             batch_gold_probs.append(gold_probs)
@@ -131,12 +150,12 @@
             C.id.value: self.ids,
             C.token_deps.value: self.token_dep,
             C.token_gold_probs.value: self.token_gold_probs,
             C.split_.value: [Split[self.split].value] * batch_size,
             C.epoch.value: [self.epoch] * batch_size,
         }
         if self.split == Split.inference:
-            data["inference_name"] = [self.inference_name] * batch_size
+            data[C.inference_name.value] = [self.inference_name] * batch_size
         return data
 
     def _write_dict_to_disk(self, path: str, object_name: str, data: Dict) -> None:
         save_arrow_file(path, object_name, data)
```

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/tabular_classification.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/text_classification.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/text_classification.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/text_multi_label.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/text_multi_label.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/loggers/model_logger/text_ner.py` & `dataquality-0.9.8/dataquality/loggers/model_logger/text_ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/metrics.py` & `dataquality-0.9.8/dataquality/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/condition.py` & `dataquality-0.9.8/dataquality/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/dataframe.py` & `dataquality-0.9.8/dataquality/schemas/dataframe.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/edit.py` & `dataquality-0.9.8/dataquality/schemas/edit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/hf.py` & `dataquality-0.9.8/dataquality/schemas/hf.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/metrics.py` & `dataquality-0.9.8/dataquality/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/ner.py` & `dataquality-0.9.8/dataquality/schemas/ner.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/report.py` & `dataquality-0.9.8/dataquality/schemas/report.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/route.py` & `dataquality-0.9.8/dataquality/schemas/route.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/semantic_segmentation.py` & `dataquality-0.9.8/dataquality/schemas/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/split.py` & `dataquality-0.9.8/dataquality/schemas/split.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/task_type.py` & `dataquality-0.9.8/dataquality/schemas/task_type.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/schemas/torch.py` & `dataquality-0.9.8/dataquality/schemas/torch.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/ampli.py` & `dataquality-0.9.8/dataquality/utils/ampli.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/auto.py` & `dataquality-0.9.8/dataquality/utils/auto.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/auto_trainer.py` & `dataquality-0.9.8/dataquality/utils/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/cuda.py` & `dataquality-0.9.8/dataquality/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/cv.py` & `dataquality-0.9.8/dataquality/utils/cv.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/dq_logger.py` & `dataquality-0.9.8/dataquality/utils/dq_logger.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/dqyolo.py` & `dataquality-0.9.8/dataquality/utils/dqyolo.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/emb.py` & `dataquality-0.9.8/dataquality/utils/emb.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/file.py` & `dataquality-0.9.8/dataquality/utils/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 import os
 import shutil
 import time
 import warnings
 from typing import Dict, Optional
 
-from dataquality.exceptions import GalileoWarning
+from dataquality.exceptions import GalileoException, GalileoWarning
 from dataquality.schemas.split import Split
 
 
+def get_extension_for_dir(dir_: str) -> str:
+    """Returns the file extension of all files in the directory
+
+    Raises exception if there are no files in the directory
+    or if there are multiple file extensions
+    """
+    files = os.listdir(dir_)
+    if len(files) == 0:
+        raise GalileoException(f"No files found in {dir_}")
+
+    extensions = set([get_file_extension(f) for f in files])
+    if len(extensions) > 1:
+        raise GalileoException(
+            f"Multiple file extensions found in {dir_}: {extensions}"
+        )
+
+    return list(extensions)[0]
+
+
 def get_file_extension(path: str) -> str:
     """Returns the file extension"""
     return os.path.splitext(path)[-1]
 
 
 def _get_dir_size(dir_: str) -> int:
     """Returns dir size in bytes"""
```

### Comparing `dataquality-0.9.7/dataquality/utils/hdf5_store.py` & `dataquality-0.9.8/dataquality/utils/hdf5_store.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/helpers.py` & `dataquality-0.9.8/dataquality/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/hf_images.py` & `dataquality-0.9.8/dataquality/utils/hf_images.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/hf_tokenizer.py` & `dataquality-0.9.8/dataquality/utils/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/keras.py` & `dataquality-0.9.8/dataquality/utils/keras.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/ml.py` & `dataquality-0.9.8/dataquality/utils/ml.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/name.py` & `dataquality-0.9.8/dataquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/od.py` & `dataquality-0.9.8/dataquality/utils/od.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/patcher.py` & `dataquality-0.9.8/dataquality/utils/patcher.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/profiler.py` & `dataquality-0.9.8/dataquality/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/semantic_segmentation/errors.py` & `dataquality-0.9.8/dataquality/utils/semantic_segmentation/errors.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/semantic_segmentation/lm.py` & `dataquality-0.9.8/dataquality/utils/semantic_segmentation/lm.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/semantic_segmentation/metrics.py` & `dataquality-0.9.8/dataquality/utils/semantic_segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/semantic_segmentation/polygons.py` & `dataquality-0.9.8/dataquality/utils/semantic_segmentation/polygons.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/semantic_segmentation/utils.py` & `dataquality-0.9.8/dataquality/utils/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/seq2seq.py` & `dataquality-0.9.8/dataquality/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/setfit.py` & `dataquality-0.9.8/dataquality/utils/setfit.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/thread_pool.py` & `dataquality-0.9.8/dataquality/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/torch.py` & `dataquality-0.9.8/dataquality/utils/torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass, field
 from functools import wraps
 from queue import Queue
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 from warnings import warn
 
 import numpy as np  # noqa: F401
+import torch
 from torch import Tensor
 from torch.nn import Module
 from torch.utils.data import DataLoader
 from torch.utils.data.dataloader import (
     _BaseDataLoaderIter,
     _MultiProcessingDataLoaderIter,
     _SingleProcessDataLoaderIter,
@@ -22,31 +23,155 @@
 from dataquality.exceptions import GalileoException
 from dataquality.schemas.task_type import TaskType
 from dataquality.schemas.torch import DimensionSlice, HelperData, Layer
 from dataquality.utils.helpers import wrap_fn
 from dataquality.utils.patcher import Borg, Patch, PatchManager
 
 
+class ModelHookManager(Borg):
+    """
+    Manages hooks for models. Has the ability to find the layer automatically.
+    Otherwise the layer or the layer name needs to be provided.
+    """
+
+    # Stores all hooks to remove them from the model later.
+    def __init__(self) -> None:
+        """Class to manage patches"""
+        super().__init__()
+        if not hasattr(self, "initialized"):
+            self.hooks: List[RemovableHandle] = []
+
+    def get_embedding_layer_auto(self, model: Module) -> Module:
+        """
+        Use a scoring algorithm to find the embedding layer automatically
+        given a model. The higher the score the more likely it is the embedding layer.
+        """
+        name, layer = next(model.named_children())
+        print(f'Selected layer for the last hidden state embedding "{name}"')
+        return layer
+
+    def get_layer_by_name(self, model: Module, name: str) -> Module:
+        """
+        Iterate over each layer and stop once the the layer name matches
+        :param model: Model
+        :parm name: string
+        """
+        queue: Queue = Queue()
+        start = model.named_children()
+        queue.put(start)
+        layer_names = []
+        layer_names_str: str = ""
+        while not queue.empty():
+            named_children = queue.get()
+            for layer_name, layer_model in named_children:
+                layer_names.append(layer_name)
+                layer_names_str = ", ".join(layer_names)
+                if layer_name == name:
+                    print(
+                        f'Found layer "{layer_name}" in '
+                        f'model layers: "{layer_names_str}"'
+                    )
+                    return layer_model
+                layer_model._get_name()
+                queue.put(layer_model.named_children())
+        raise GalileoException(
+            f"Layer could not be found in layers: {layer_names_str}. "
+            "make sure to check capitalization or pass layer directly."
+        )
+
+    def attach_hooks_to_model(
+        self,
+        model: Module,
+        hook_fn: Callable,
+        model_layer: Optional[Layer] = None,
+    ) -> RemovableHandle:
+        """Attach hook and save it in our hook list"""
+        if model_layer is None:
+            selected_layer = self.get_embedding_layer_auto(model)
+        elif isinstance(model_layer, str):
+            selected_layer = self.get_layer_by_name(model, model_layer)
+        else:
+            selected_layer = model_layer
+        return self.attach_hook(selected_layer, hook_fn)
+
+    def attach_classifier_hook(
+        self,
+        model: Module,
+        classifier_hook: Callable,
+        model_layer: Optional[Layer] = None,
+    ) -> RemovableHandle:
+        """Attach hook and save it in our hook list"""
+        if model_layer is None:
+            try:
+                selected_layer = self.get_layer_by_name(model, "classifier")
+            except GalileoException:
+                selected_layer = self.get_layer_by_name(model, "fc")
+        elif isinstance(model_layer, str):
+            selected_layer = self.get_layer_by_name(model, model_layer)
+        else:
+            selected_layer = model_layer
+
+        return self.attach_hook(selected_layer, classifier_hook)
+
+    def attach_hook(self, selected_layer: Module, hook: Callable) -> RemovableHandle:
+        """Register a hook and save it in our hook list"""
+        self.initialized = True
+        h = selected_layer.register_forward_hook(hook)
+        self.hooks.append(h)
+        return h
+
+    def detach_hooks(self) -> None:
+        """Remove all hooks from the model"""
+        for h in self.hooks:
+            h.remove()
+        self.hooks = []
+
+
+@dataclass
+class ModelOutputsStore:
+    embs: Optional[Tensor] = None
+    logits: Optional[Union[Tensor, Tuple[Tuple]]] = None
+    ids_queue: List[List[int]] = field(default_factory=list)
+    ids: Optional[List[int]] = None
+
+    def clear(self) -> None:
+        """Resets the arrays of the class."""
+        self.embs = None
+        self.logits = None
+        self.ids = None
+
+    def clear_all(self) -> None:
+        """Resets the arrays of the class."""
+        self.embs = None
+        self.logits = None
+        self.ids = None
+        self.ids_queue.clear()
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Returns the class as a dictionary."""
+        return {"embs": self.embs, "logits": self.logits, "ids": self.ids}
+
+
 @dataclass
 class TorchHelper:
     model: Optional[Any] = None
-    hook_manager: Optional[Any] = None
-    model_outputs_store: Dict[str, Any] = field(default_factory=dict)
+    hook_manager: Optional[ModelHookManager] = None
+    model_outputs_store: ModelOutputsStore = field(default_factory=ModelOutputsStore)
     dl_next_idx_ids: List[Any] = field(default_factory=list)
-    model_input: Any = np.empty(0)
+    model_input: Tensor = torch.empty(0)
     batch: Dict[str, Any] = field(default_factory=dict)
     ids: List[Any] = field(default_factory=list)
     patches: List[Dict] = field(default_factory=list)
 
     def clear(self) -> None:
         """Resets the arrays of the class."""
         self.dl_next_idx_ids.clear()
         self.model_outputs_store.clear()
         self.ids.clear()
-        self.model_input = np.empty(0)
+        self.model_input = torch.empty(0)
         self.batch.clear()
 
 
 class TorchBaseInstance:
     embedding_dim: Optional[DimensionSlice]
     logits_dim: Optional[DimensionSlice]
     embedding_fn: Optional[Any] = None
@@ -136,15 +261,15 @@
             # for text classification tasks and multi label tasks
             output_detached = output_detached[:, 0]
         elif len(output_detached.shape) == 3 and self.task == TaskType.text_ner:
             # It is assumed that the CLS token is removed through this dimension
             # for NER tasks
             output_detached = output_detached[:, 1:, :]
 
-        self.torch_helper_data.model_outputs_store["embs"] = output_detached
+        self.torch_helper_data.model_outputs_store.embs = output_detached
 
     def _dq_logit_hook(
         self,
         model: Module,
         model_input: Optional[Tensor],
         model_output: Union[Tuple[Tensor], TokenClassifierOutput, Tensor],
     ) -> None:
@@ -178,15 +303,15 @@
         if self.logits_dim is not None:
             logits = logits[self.logits_dim]
         elif len(logits.shape) == 3 and self.task == TaskType.text_ner:
             # It is assumed that the CLS token is removed
             # through this dimension for NER tasks
             logits = logits[:, 1:, :]
 
-        self.torch_helper_data.model_outputs_store["logits"] = logits
+        self.torch_helper_data.model_outputs_store.logits = logits
 
     def _classifier_hook(
         self,
         model: Module,
         model_input: Union[BaseModelOutput, Tensor],
         model_output: Union[Tuple[Tensor], TokenClassifierOutput, Tensor],
     ) -> None:
@@ -263,113 +388,14 @@
     # Validate the string before we eval the fancy index
     assert validate_fancy_index_str(
         clean_str
     ), 'Fancy index string is not valid. Valid format: "[:, 1:, :]"'
     return eval("np.s_[{}]".format(clean_str))
 
 
-class ModelHookManager(Borg):
-    """
-    Manages hooks for models. Has the ability to find the layer automatically.
-    Otherwise the layer or the layer name needs to be provided.
-    """
-
-    # Stores all hooks to remove them from the model later.
-    def __init__(self) -> None:
-        """Class to manage patches"""
-        super().__init__()
-        if not hasattr(self, "initialized"):
-            self.hooks: List[RemovableHandle] = []
-
-    def get_embedding_layer_auto(self, model: Module) -> Module:
-        """
-        Use a scoring algorithm to find the embedding layer automatically
-        given a model. The higher the score the more likely it is the embedding layer.
-        """
-        name, layer = next(model.named_children())
-        print(f'Selected layer for the last hidden state embedding "{name}"')
-        return layer
-
-    def get_layer_by_name(self, model: Module, name: str) -> Module:
-        """
-        Iterate over each layer and stop once the the layer name matches
-        :param model: Model
-        :parm name: string
-        """
-        queue: Queue = Queue()
-        start = model.named_children()
-        queue.put(start)
-        layer_names = []
-        layer_names_str: str = ""
-        while not queue.empty():
-            named_children = queue.get()
-            for layer_name, layer_model in named_children:
-                layer_names.append(layer_name)
-                layer_names_str = ", ".join(layer_names)
-                if layer_name == name:
-                    print(
-                        f'Found layer "{layer_name}" in '
-                        f'model layers: "{layer_names_str}"'
-                    )
-                    return layer_model
-                layer_model._get_name()
-                queue.put(layer_model.named_children())
-        raise GalileoException(
-            f"Layer could not be found in layers: {layer_names_str}. "
-            "make sure to check capitalization or pass layer directly."
-        )
-
-    def attach_hooks_to_model(
-        self,
-        model: Module,
-        hook_fn: Callable,
-        model_layer: Optional[Layer] = None,
-    ) -> RemovableHandle:
-        """Attach hook and save it in our hook list"""
-        if model_layer is None:
-            selected_layer = self.get_embedding_layer_auto(model)
-        elif isinstance(model_layer, str):
-            selected_layer = self.get_layer_by_name(model, model_layer)
-        else:
-            selected_layer = model_layer
-        return self.attach_hook(selected_layer, hook_fn)
-
-    def attach_classifier_hook(
-        self,
-        model: Module,
-        classifier_hook: Callable,
-        model_layer: Optional[Layer] = None,
-    ) -> RemovableHandle:
-        """Attach hook and save it in our hook list"""
-        if model_layer is None:
-            try:
-                selected_layer = self.get_layer_by_name(model, "classifier")
-            except GalileoException:
-                selected_layer = self.get_layer_by_name(model, "fc")
-        elif isinstance(model_layer, str):
-            selected_layer = self.get_layer_by_name(model, model_layer)
-        else:
-            selected_layer = model_layer
-
-        return self.attach_hook(selected_layer, classifier_hook)
-
-    def attach_hook(self, selected_layer: Module, hook: Callable) -> RemovableHandle:
-        """Register a hook and save it in our hook list"""
-        self.initialized = True
-        h = selected_layer.register_forward_hook(hook)
-        self.hooks.append(h)
-        return h
-
-    def detach_hooks(self) -> None:
-        """Remove all hooks from the model"""
-        for h in self.hooks:
-            h.remove()
-        self.hooks = []
-
-
 def unpatch(patches: List[Dict[str, Any]] = []) -> None:
     """
     Unpatch all patched classes and instances
     :param patches: list of patches
     """
     manager = PatchManager()
     manager.unpatch()
@@ -493,15 +519,15 @@
 
 class PatchSingleDataloaderIterator(Patch):
     name = "patch_single_dataloader_iterator"
 
     def __init__(
         self,
         dataloader_cls: DataLoader,
-        store: Dict[str, List[int]],
+        store: ModelOutputsStore,
         fn_name: str = "_get_iterator",
     ):
         """Initializes the class with a collate function,
         columns to keep, and a store to save ids.
 
         :param collate_fn: The collate function to wrap
         :param keep_cols: The columns to keep
@@ -533,15 +559,15 @@
 
 class PatchSingleDataloaderNextIndex(Patch):
     name = "patch_next_index"
 
     def __init__(
         self,
         dataloader_cls: DataLoader,
-        store: Dict[str, List[int]],
+        store: ModelOutputsStore,
         fn_name: str = "_get_iterator",
     ):
         """Initializes the class with a collate function,
         columns to keep, and a store to save ids.
 
         :param collate_fn: The collate function to wrap
         :param keep_cols: The columns to keep
@@ -562,15 +588,15 @@
         """Restores the original collate function,
         removing the id removal functionality."""
         setattr(self.orig_cls, self._fn_name, self._original_fn)
 
     def __call__(self, *args: Any, **kwargs: Any) -> List[dict]:
         indices = self._original_fn(*args, **kwargs)
         if indices:
-            self.store["ids"] = indices
+            self.store.ids = indices
         return indices
 
 
 class PatchDataloadersGlobally(Patch):
     name = "patch_dataloaders_globally"
 
     def __init__(self, torch_helper: TorchHelper):
```

### Comparing `dataquality-0.9.7/dataquality/utils/transformers.py` & `dataquality-0.9.8/dataquality/utils/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import inspect
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, List, Union
 
 from torch.nn import Module
 from transformers import Trainer
 
 from dataquality.utils.patcher import Patch
+from dataquality.utils.torch import ModelOutputsStore
 
 
 class RemoveIdCollatePatch(Patch):
     _original_collate_fn: Union[Callable, Any]
     name = "remove_id_collate_patch"
 
     def __init__(
         self,
         trainer_cls: Trainer,
         keep_cols: List[str],
-        store: Dict[str, List[int]],
+        store: ModelOutputsStore,
         fn_name: str = "data_collator",
     ):
         """Initializes the class with a collate function,
         columns to keep, and a store to save ids.
 
         :param collate_fn: The collate function to wrap
         :param keep_cols: The columns to keep
@@ -55,15 +56,15 @@
                 if key == "id":
                     ids.append(value)
                 elif key in self.keep_cols:
                     clean_row[key] = value
                 elif len(self.keep_cols) == 0:
                     clean_row[key] = value
             clean_rows.append(clean_row)
-        self.store["ids"] = ids
+        self.store.ids_queue.append(ids)
         return self._original_collate_fn(clean_rows)
 
 
 class SignatureColumnsPatch(Patch):
     name = "signature_columns_patch"
 
     def __init__(self, trainer: Trainer):
```

### Comparing `dataquality-0.9.7/dataquality/utils/ultralytics.py` & `dataquality-0.9.8/dataquality/utils/ultralytics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/upload.py` & `dataquality-0.9.8/dataquality/utils/upload.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality/utils/vaex.py` & `dataquality-0.9.8/dataquality/utils/vaex.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from dataquality.utils.cuda import (
     PCA_CHUNK_SIZE,
     PCA_N_COMPONENTS,
     cuml_available,
     get_pca_embeddings,
     get_umap_embeddings,
 )
+from dataquality.utils.file import get_extension_for_dir
 from dataquality.utils.hdf5_store import HDF5_STORE, concat_hdf5_files
 from dataquality.utils.helpers import galileo_verbose_logging
 
 object_store = ObjectStore()
 
 # To decide between "all-MiniLM-L6-v2" or "all-mpnet-base-v2"
 # https://www.sbert.net/docs/pretrained_models.html#model-overview
@@ -225,38 +226,50 @@
     epoch_or_inf: Union[str, int],
 ) -> DataFrame:
     """Creates the single hdf5 file for the output data of a split/epoch
 
     Applies the necessary conversions post-concatenation of files
     (see `concat_hdf5_files`)
     """
-    out_frame_path = f"{dir_name}/{HDF5_STORE}"
-    # It's possible the files were already concatenated and handled. In that case
-    # just open the processed file
-    if os.path.isfile(out_frame_path):
-        return vaex.open(out_frame_path)
-    str_cols = concat_hdf5_files(dir_name, prob_only)
-    out_frame = vaex.open(out_frame_path)
+    out_frame_ext = get_extension_for_dir(dir_name)
+
+    if out_frame_ext == ".arrow":
+        out_frame = vaex.open(f"{dir_name}/*.arrow")
+    elif out_frame_ext == ".hdf5":
+        out_frame_path = f"{dir_name}/{HDF5_STORE}"
+        # It's possible the files were already concatenated and handled. In that case
+        # just open the processed file
+        if os.path.isfile(out_frame_path):
+            return vaex.open(out_frame_path)
+
+        str_cols = concat_hdf5_files(dir_name, prob_only)
+        out_frame = vaex.open(out_frame_path)
+        # Post concat, string columns come back as bytes and need conversion
+        for col in str_cols:
+            out_frame[col] = out_frame[col].as_arrow().astype("str")
+            out_frame[col] = out_frame[f'astype({col}, "large_string")']
+
+    else:
+        raise GalileoException(
+            f"Unsupported file extension {out_frame_ext} for output data"
+        )
 
     if split == Split.inference:
         dtype: Union[str, None] = "str"
         epoch_or_inf_name = "inference_name"
     else:
         dtype = None
         epoch_or_inf_name = "epoch"
 
-    # Post concat, string columns come back as bytes and need conversion
-    for col in str_cols:
-        out_frame[col] = out_frame[col].as_arrow().astype("str")
-        out_frame[col] = out_frame[f'astype({col}, "large_string")']
     if prob_only:
         out_frame["split"] = vaex.vconstant(split, length=len(out_frame), dtype="str")
         out_frame[epoch_or_inf_name] = vaex.vconstant(
             epoch_or_inf, length=len(out_frame), dtype=dtype
         )
+
     return out_frame
 
 
 def add_pca_to_df(df: DataFrame, chunk_size: int = PCA_CHUNK_SIZE) -> DataFrame:
     """Adds the 'emb_pca' to the dataframe"""
     df_copy = df.copy()
     # n_components must be <= num samples and <= emb dimension
```

### Comparing `dataquality-0.9.7/dataquality/utils/version.py` & `dataquality-0.9.8/dataquality/utils/version.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality.egg-info/PKG-INFO` & `dataquality-0.9.8/dataquality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataquality
-Version: 0.9.7
+Version: 0.9.8
 Author-email: "Galileo Technologies, Inc." <devs+dq@rungalileo.io>
 License: See LICENSE
 Project-URL: Homepage, https://github.com/rungalileo/dataquality
 Project-URL: Documentation, https://rungalileo.gitbook.io/galileo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
```

### Comparing `dataquality-0.9.7/dataquality.egg-info/SOURCES.txt` & `dataquality-0.9.8/dataquality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/dataquality.egg-info/requires.txt` & `dataquality-0.9.8/dataquality.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/pyproject.toml` & `dataquality-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_dataquality.py` & `dataquality-0.9.8/tests/test_dataquality.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_telemetrics.py` & `dataquality-0.9.8/tests/test_telemetrics.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/data_utils.py` & `dataquality-0.9.8/tests/test_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/hf_datasets_mock.py` & `dataquality-0.9.8/tests/test_utils/hf_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/hf_integration_constants.py` & `dataquality-0.9.8/tests/test_utils/hf_integration_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/hf_integration_constants_inference.py` & `dataquality-0.9.8/tests/test_utils/hf_integration_constants_inference.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/lightning_model.py` & `dataquality-0.9.8/tests/test_utils/lightning_model.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/mock_data.py` & `dataquality-0.9.8/tests/test_utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/mock_request.py` & `dataquality-0.9.8/tests/test_utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/ner_constants.py` & `dataquality-0.9.8/tests/test_utils/ner_constants.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/pt_datasets_mock.py` & `dataquality-0.9.8/tests/test_utils/pt_datasets_mock.py`

 * *Files identical despite different names*

### Comparing `dataquality-0.9.7/tests/test_utils/tc_constants.py` & `dataquality-0.9.8/tests/test_utils/tc_constants.py`

 * *Files identical despite different names*

