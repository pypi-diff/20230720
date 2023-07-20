# Comparing `tmp/mindpet-1.0.0.tar.gz` & `tmp/mindpet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindpet-1.0.0.tar", last modified: Tue Jun 13 07:55:22 2023, max compression
+gzip compressed data, was "mindpet-1.0.1.tar", last modified: Thu Jul 20 06:12:57 2023, max compression
```

## Comparing `mindpet-1.0.0.tar` & `mindpet-1.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-13 07:45:19.000000 mindpet-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3258 2023-06-13 07:55:22.000000 mindpet-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3015 2023-06-13 07:45:19.000000 mindpet-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3258 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2023-06-13 07:55:22.000000 mindpet-1.0.0/mindpet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1526 2023-06-13 07:45:19.000000 mindpet-1.0.0/set_up.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 07:55:22.000000 mindpet-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/delta/
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/adapter.py
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/delta_constants.py
--rw-r--r--   0 root         (0) root         (0)     9893 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/lora.py
--rw-r--r--   0 root         (0) root         (0)    26658 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/low_rank_adapter.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/prefix_layer.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/delta/r_drop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/graph/
--rw-r--r--   0 root         (0) root         (0)      362 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/graph/ckpt_util.py
--rw-r--r--   0 root         (0) root         (0)     8770 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/graph/freeze_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/log/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18071 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/log/log.py
--rw-r--r--   0 root         (0) root         (0)     8586 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/log/log_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/security/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/security/param_check/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/security/param_check/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/security/param_check/base_check.py
--rw-r--r--   0 root         (0) root         (0)     3336 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/security/param_check/model_config_params_check_util.py
--rw-r--r--   0 root         (0) root         (0)    24719 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/security/param_check/option_check_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/task/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/task/evaluate_infer/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/evaluate_infer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11024 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/evaluate_infer/evaluate_infer_task.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/evaluate_infer/result_file_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/task/finetune/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/finetune/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/finetune/finetune_options_check.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/finetune/finetune_task.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/option_decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/task/options/
--rw-r--r--   0 root         (0) root         (0)      646 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/boot_file_path_option.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/ckpt_path_option.py
--rw-r--r--   0 root         (0) root         (0)     1630 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/data_path_option.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/model_config_path_option.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/output_path_option.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/path_check_param.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/pretrained_model_path_option.py
--rw-r--r--   0 root         (0) root         (0)      795 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/quiet_option.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/task/options/timeout_option.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/tk_main.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/tk_sdk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:55:22.000000 mindpet-1.0.0/tk/utils/
--rw-r--r--   0 root         (0) root         (0)      123 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3356 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/constants.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/entrance_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/io_utils.py
--rw-r--r--   0 root         (0) root         (0)     7738 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/task_utils.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-06-13 07:45:19.000000 mindpet-1.0.0/tk/utils/version_utils.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.093659 mindpet-1.0.1/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    11357 2023-07-20 06:12:24.000000 mindpet-1.0.1/LICENSE
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3202 2023-07-20 06:12:57.093659 mindpet-1.0.1/PKG-INFO
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3015 2023-07-20 06:12:24.000000 mindpet-1.0.1/README.md
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/mindpet.egg-info/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3202 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/PKG-INFO
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1557 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/SOURCES.txt
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)        1 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/dependency_links.txt
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)       46 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/entry_points.txt
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)       13 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/requires.txt
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)        3 2023-07-20 06:12:57.000000 mindpet-1.0.1/mindpet.egg-info/top_level.txt
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1526 2023-07-20 06:12:44.000000 mindpet-1.0.1/set_up.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)       38 2023-07-20 06:12:57.093659 mindpet-1.0.1/setup.cfg
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      174 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/__init__.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/delta/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      552 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    14178 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/adapter.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      251 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/delta_constants.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     9895 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/lora.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    26659 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/low_rank_adapter.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3965 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/prefix_layer.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2213 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/delta/r_drop.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/graph/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      362 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/graph/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     5623 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/graph/ckpt_util.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     8770 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/graph/freeze_utils.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/log/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      345 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/log/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    18071 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/log/log.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     8586 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/log/log_utils.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/security/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/security/__init__.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/security/param_check/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/security/param_check/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1968 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/security/param_check/base_check.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3336 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/security/param_check/model_config_params_check_util.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    24719 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/security/param_check/option_check_utils.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.089659 mindpet-1.0.1/tk/task/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/__init__.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.093659 mindpet-1.0.1/tk/task/evaluate_infer/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/evaluate_infer/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)    11024 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/evaluate_infer/evaluate_infer_task.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2051 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/evaluate_infer/result_file_check.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.093659 mindpet-1.0.1/tk/task/finetune/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/finetune/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     4182 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/finetune/finetune_options_check.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     6041 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/finetune/finetune_task.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1826 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/option_decorators.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.093659 mindpet-1.0.1/tk/task/options/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      646 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2224 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/boot_file_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1636 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/ckpt_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1630 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/data_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2160 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/model_config_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1673 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/output_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1559 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/path_check_param.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1713 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/pretrained_model_path_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      795 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/quiet_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1930 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/task/options/timeout_option.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1854 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/tk_main.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2985 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/tk_sdk.py
+drwxr-xr-x   0 huanglei  (1009) huanglei  (1010)        0 2023-07-20 06:12:57.093659 mindpet-1.0.1/tk/utils/
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      123 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/__init__.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3356 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/constants.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)      654 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/entrance_monitor.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     3737 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/exceptions.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     1817 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/io_utils.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     7738 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/task_utils.py
+-rw-r--r--   0 huanglei  (1009) huanglei  (1010)     2008 2023-07-20 06:12:24.000000 mindpet-1.0.1/tk/utils/version_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mindpet-1.0.0/LICENSE` & `mindpet-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/PKG-INFO` & `mindpet-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: mindpet
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parameter-Efficient Tuning
-Home-page: UNKNOWN
-License: UNKNOWN
 Keywords: Parameter-Efficient Tuning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MindPet微调算法用户文档
 
 
 
@@ -76,9 +73,7 @@
 
 
 ### 4.2 保存可训练参数功能API
 
 MindPet支持用户单独保存训练中可更新的参数为ckpt文件，从而节省存储所用的物理资源。
 
 使用说明参考[TK_GraphOperation_README](doc/TK_GraphOperation_README.md) 第二章。
-
-
```

### Comparing `mindpet-1.0.0/README.md` & `mindpet-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/mindpet.egg-info/PKG-INFO` & `mindpet-1.0.1/mindpet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: mindpet
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parameter-Efficient Tuning
-Home-page: UNKNOWN
-License: UNKNOWN
 Keywords: Parameter-Efficient Tuning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MindPet微调算法用户文档
 
 
 
@@ -76,9 +73,7 @@
 
 
 ### 4.2 保存可训练参数功能API
 
 MindPet支持用户单独保存训练中可更新的参数为ckpt文件，从而节省存储所用的物理资源。
 
 使用说明参考[TK_GraphOperation_README](doc/TK_GraphOperation_README.md) 第二章。
-
-
```

### Comparing `mindpet-1.0.0/mindpet.egg-info/SOURCES.txt` & `mindpet-1.0.1/mindpet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/set_up.py` & `mindpet-1.0.1/set_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 cmd_class = {}
 
 
 def get_version():
-    version = '1.0.0'
+    version = '1.0.1'
     return version
 
 
 def do_setup(packages_data):
     setup(
         name='mindpet',
```

### Comparing `mindpet-1.0.0/tk/delta/__init__.py` & `mindpet-1.0.1/tk/delta/__init__.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/delta/adapter.py` & `mindpet-1.0.1/tk/delta/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import mindspore.nn as nn
 import mindspore.common.dtype as mstype
 from mindspore.nn.layer.activation import get_activation, _activation
 from mindspore.ops import operations as P
 from mindspore.ops import functional as F
 from tk.delta.delta_constants import VALID_TENSOR_DATATYPE
 
-if is_version_ge(ms.__version__, '2.0.0'):
+if is_version_ge(ms.__version__, '1.11.0'):
     from mindformers.modules.layers import Linear, _args_type_validator_check, _valid_value_checks
     import mindspore._checkparam as Validator
     _Linear = Linear
 else:
     from mindspore.nn.transformer.layers import _Linear, _args_type_validator_check, _valid_value_checks
     from mindspore._checkparam import Validator
```

### Comparing `mindpet-1.0.0/tk/delta/lora.py` & `mindpet-1.0.1/tk/delta/lora.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from mindspore.common.tensor import Tensor
 from mindspore import dtype as mstype
 from mindspore.ops import operations as P
 from mindspore.ops import functional as F
 from mindspore.common.initializer import initializer, HeUniform
 from tk.delta.delta_constants import VALID_TENSOR_DATATYPE
 
-if is_version_ge(ms.__version__, '2.0.0'):
+if is_version_ge(ms.__version__, '1.11.0'):
     import mindspore._checkparam as Validator
     INC_LEFT = Validator.INC_LEFT
 else:
     from mindspore._checkparam import Validator, Rel
     INC_LEFT = Rel.INC_LEFT
 
 class LoRADense(nn.Dense):
@@ -56,15 +56,15 @@
         self._check_num(lora_rank, lora_alpha, lora_dropout)
         self._check_init(lora_a_init, lora_b_init, lora_rank)
         self._check_type_of_data(param_init_type, compute_dtype)
 
         # Define and initialize params
         self.lora_rank = lora_rank
         self.lora_alpha = lora_alpha
-        if is_version_ge(ms.__version__, '2.0.0'):
+        if is_version_ge(ms.__version__, '1.11.0'):
             self.lora_dropout = nn.Dropout(p=lora_dropout)
         else:
             self.lora_dropout = nn.Dropout(keep_prob=1 - lora_dropout)
         self.tk_delta_lora_a = Parameter(
             initializer(lora_a_init, [lora_rank, in_channels], param_init_type),
             name='tk_delta_lora_A')
         self.tk_delta_lora_b = Parameter(initializer(lora_b_init, [out_channels, lora_rank], param_init_type),
```

### Comparing `mindpet-1.0.0/tk/delta/low_rank_adapter.py` & `mindpet-1.0.1/tk/delta/low_rank_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from mindspore import Tensor
 
 from mindspore.nn.layer.activation import get_activation, _activation
 from mindspore.ops import operations as P
 from mindspore.ops import functional as F
 from tk.delta.delta_constants import VALID_TENSOR_DATATYPE
 
-if is_version_ge(ms.__version__, '2.0.0'):
+if is_version_ge(ms.__version__, '1.11.0'):
     from mindformers.modules.layers import _args_type_validator_check, _valid_type_checks, _valid_value_checks
     import mindspore._checkparam as Validator
 else:
     from mindspore.nn.transformer.layers import _args_type_validator_check, _valid_type_checks, _valid_value_checks
     from mindspore._checkparam import Validator
```

### Comparing `mindpet-1.0.0/tk/delta/prefix_layer.py` & `mindpet-1.0.1/tk/delta/prefix_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © Huawei Technologies Co., Ltd. 2010-2022. All rights reserved.
 
 import mindspore as ms
 import mindspore.nn as nn
 
 from tk.utils.version_utils import is_version_ge
 
-if is_version_ge(ms.__version__, '2.0.0'):
+if is_version_ge(ms.__version__, '1.11.0'):
     import mindspore._checkparam as Validator
     INC_LEFT = Validator.INC_LEFT
 else:
     from mindspore._checkparam import Validator, Rel
     INC_LEFT = Rel.INC_LEFT
 
 
@@ -51,15 +51,15 @@
         self.mid_dim = Validator.check_positive_int(mid_dim, int, "mid_dim")
         self.dropout_rate = Validator.check_float_range(dropout_rate, 0.0, 1.0, INC_LEFT)
         try:
             check_multiple("prefix_token_num", prefix_token_num, "batch_size", batch_size)
         except ValueError as ex:
             raise ValueError(f"Invalid param [prefix_token_num] when initializing"
                              f"PrefixLayer, error message:{str(ex)}") from ex
-        if is_version_ge(ms.__version__, '2.0.0'):
+        if is_version_ge(ms.__version__, '1.11.0'):
             self.dropout = nn.Dropout(p=dropout_rate)
         else:
             self.dropout = nn.Dropout(keep_prob=1 - dropout_rate)
         self.past_value_reparam = None
         self.past_key_reparam = None
         self.__define_network()
         self.__allocate_parameter()
```

### Comparing `mindpet-1.0.0/tk/delta/r_drop.py` & `mindpet-1.0.1/tk/delta/r_drop.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/graph/ckpt_util.py` & `mindpet-1.0.1/tk/graph/ckpt_util.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/graph/freeze_utils.py` & `mindpet-1.0.1/tk/graph/freeze_utils.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/log/log.py` & `mindpet-1.0.1/tk/log/log.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/log/log_utils.py` & `mindpet-1.0.1/tk/log/log_utils.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/security/param_check/base_check.py` & `mindpet-1.0.1/tk/security/param_check/base_check.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/security/param_check/model_config_params_check_util.py` & `mindpet-1.0.1/tk/security/param_check/model_config_params_check_util.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/security/param_check/option_check_utils.py` & `mindpet-1.0.1/tk/security/param_check/option_check_utils.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/evaluate_infer/evaluate_infer_task.py` & `mindpet-1.0.1/tk/task/evaluate_infer/evaluate_infer_task.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/evaluate_infer/result_file_check.py` & `mindpet-1.0.1/tk/task/evaluate_infer/result_file_check.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/finetune/finetune_options_check.py` & `mindpet-1.0.1/tk/task/finetune/finetune_options_check.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/finetune/finetune_task.py` & `mindpet-1.0.1/tk/task/finetune/finetune_task.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/option_decorators.py` & `mindpet-1.0.1/tk/task/option_decorators.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/__init__.py` & `mindpet-1.0.1/tk/task/options/__init__.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/boot_file_path_option.py` & `mindpet-1.0.1/tk/task/options/boot_file_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/ckpt_path_option.py` & `mindpet-1.0.1/tk/task/options/ckpt_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/data_path_option.py` & `mindpet-1.0.1/tk/task/options/data_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/model_config_path_option.py` & `mindpet-1.0.1/tk/task/options/model_config_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/output_path_option.py` & `mindpet-1.0.1/tk/task/options/output_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/path_check_param.py` & `mindpet-1.0.1/tk/task/options/path_check_param.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/pretrained_model_path_option.py` & `mindpet-1.0.1/tk/task/options/pretrained_model_path_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/quiet_option.py` & `mindpet-1.0.1/tk/task/options/quiet_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/task/options/timeout_option.py` & `mindpet-1.0.1/tk/task/options/timeout_option.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/tk_main.py` & `mindpet-1.0.1/tk/tk_main.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/tk_sdk.py` & `mindpet-1.0.1/tk/tk_sdk.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/constants.py` & `mindpet-1.0.1/tk/utils/constants.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/entrance_monitor.py` & `mindpet-1.0.1/tk/utils/entrance_monitor.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/exceptions.py` & `mindpet-1.0.1/tk/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/io_utils.py` & `mindpet-1.0.1/tk/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/task_utils.py` & `mindpet-1.0.1/tk/utils/task_utils.py`

 * *Files identical despite different names*

### Comparing `mindpet-1.0.0/tk/utils/version_utils.py` & `mindpet-1.0.1/tk/utils/version_utils.py`

 * *Files identical despite different names*

