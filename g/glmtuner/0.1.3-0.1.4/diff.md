# Comparing `tmp/glmtuner-0.1.3.tar.gz` & `tmp/glmtuner-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glmtuner-0.1.3.tar", last modified: Tue Jul 18 12:51:54 2023, max compression
+gzip compressed data, was "glmtuner-0.1.4.tar", last modified: Thu Jul 20 14:31:53 2023, max compression
```

## Comparing `glmtuner-0.1.3.tar` & `glmtuner-0.1.4.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.674250 glmtuner-0.1.3/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-18 12:50:56.000000 glmtuner-0.1.3/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18770 2023-07-18 12:51:54.670250 glmtuner-0.1.3/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18203 2023-07-18 12:51:01.000000 glmtuner-0.1.3/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-18 12:51:01.000000 glmtuner-0.1.3/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-18 12:51:54.674250 glmtuner-0.1.3/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-18 12:51:01.000000 glmtuner-0.1.3/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.362251 glmtuner-0.1.3/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.382251 glmtuner-0.1.3/src/glmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      250 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.414250 glmtuner-0.1.3/src/glmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4554 2023-07-18 12:50:56.000000 glmtuner-0.1.3/src/glmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-18 12:50:56.000000 glmtuner-0.1.3/src/glmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.418251 glmtuner-0.1.3/src/glmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4618 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.434250 glmtuner-0.1.3/src/glmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      165 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6589 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/dsets/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.474250 glmtuner-0.1.3/src/glmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3064 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      306 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5062 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-18 12:50:57.000000 glmtuner-0.1.3/src/glmtuner/extras/save_and_load.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.510250 glmtuner-0.1.3/src/glmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4283 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3309 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3310 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.510250 glmtuner-0.1.3/src/glmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.534250 glmtuner-0.1.3/src/glmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8545 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5754 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4125 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.554250 glmtuner-0.1.3/src/glmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10451 2023-07-18 12:50:58.000000 glmtuner-0.1.3/src/glmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3066 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.582250 glmtuner-0.1.3/src/glmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1523 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2888 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.602250 glmtuner-0.1.3/src/glmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2189 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2587 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4208 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.634250 glmtuner-0.1.3/src/glmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-18 12:51:01.000000 glmtuner-0.1.3/src/glmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2662 2023-07-18 12:50:59.000000 glmtuner-0.1.3/src/glmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.670250 glmtuner-0.1.3/src/glmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1839 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2507 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1354 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4096 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1786 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1461 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10687 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-18 12:51:00.000000 glmtuner-0.1.3/src/glmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7432 2023-07-18 12:51:01.000000 glmtuner-0.1.3/src/glmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2914 2023-07-18 12:51:01.000000 glmtuner-0.1.3/src/glmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:54.386251 glmtuner-0.1.3/src/glmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18770 2023-07-18 12:51:53.000000 glmtuner-0.1.3/src/glmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2137 2023-07-18 12:51:53.000000 glmtuner-0.1.3/src/glmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-18 12:51:53.000000 glmtuner-0.1.3/src/glmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      219 2023-07-18 12:51:53.000000 glmtuner-0.1.3/src/glmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-18 12:51:53.000000 glmtuner-0.1.3/src/glmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.674405 glmtuner-0.1.4/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-20 14:30:29.000000 glmtuner-0.1.4/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    19827 2023-07-20 14:31:53.674405 glmtuner-0.1.4/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    19276 2023-07-20 14:30:34.000000 glmtuner-0.1.4/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-20 14:30:34.000000 glmtuner-0.1.4/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-20 14:31:53.690405 glmtuner-0.1.4/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-20 14:30:35.000000 glmtuner-0.1.4/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.794369 glmtuner-0.1.4/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.826370 glmtuner-0.1.4/src/glmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.850371 glmtuner-0.1.4/src/glmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.874372 glmtuner-0.1.4/src/glmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4530 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.926374 glmtuner-0.1.4/src/glmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      213 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6578 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/dsets/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/dsets/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      531 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/dsets/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.174384 glmtuner-0.1.4/src/glmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3064 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      306 2023-07-20 14:30:30.000000 glmtuner-0.1.4/src/glmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5108 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/extras/save_and_load.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.298390 glmtuner-0.1.4/src/glmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4283 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3309 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3310 2023-07-20 14:30:31.000000 glmtuner-0.1.4/src/glmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.310390 glmtuner-0.1.4/src/glmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.350391 glmtuner-0.1.4/src/glmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8545 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5754 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4125 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.378393 glmtuner-0.1.4/src/glmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    10623 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3066 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.446395 glmtuner-0.1.4/src/glmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-20 14:30:32.000000 glmtuner-0.1.4/src/glmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1568 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2520 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.462396 glmtuner-0.1.4/src/glmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2189 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2587 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3840 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.550400 glmtuner-0.1.4/src/glmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2692 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:53.582401 glmtuner-0.1.4/src/glmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1818 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2531 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1388 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5096 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1911 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-20 14:30:33.000000 glmtuner-0.1.4/src/glmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1456 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12736 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7853 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2914 2023-07-20 14:30:34.000000 glmtuner-0.1.4/src/glmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:31:52.830370 glmtuner-0.1.4/src/glmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    19827 2023-07-20 14:31:51.000000 glmtuner-0.1.4/src/glmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2165 2023-07-20 14:31:52.000000 glmtuner-0.1.4/src/glmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-20 14:31:51.000000 glmtuner-0.1.4/src/glmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      236 2023-07-20 14:31:51.000000 glmtuner-0.1.4/src/glmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-20 14:31:51.000000 glmtuner-0.1.4/src/glmtuner.egg-info/top_level.txt
```

### Comparing `glmtuner-0.1.3/LICENSE` & `glmtuner-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/PKG-INFO` & `glmtuner-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -62,36 +62,43 @@
 
 [23/04/12] Now we support **training from checkpoints**! Use `--checkpoint_dir` argument to specify the checkpoint model to fine-tune from.
 
 [23/04/11] Now we support training with **combined datasets**! Try `--dataset dataset1,dataset2` argument for training with multiple datasets.
 
 ## Datasets
 
-Our script now supports the following datasets:
-
-- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-- [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-- [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-- [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-- [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-- [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-- [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-- [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-- [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-- [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-- [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-- [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-- [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-- [UltraChat](https://github.com/thunlp/UltraChat)
-- [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For supervised fine-tuning:
+  - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
+  - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [Self-cognition (zh)](data/self_cognition.json)
+  - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
+  - [RefGPT (zh)](https://github.com/sufengniu/RefGPT)
+  - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
+  - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
+  - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+  - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+  - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
+  - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
+  - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+  - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
+  - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
+  - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
+  - [UltraChat (en)](https://github.com/thunlp/UltraChat)
+  - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For reward modelling:
+  - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 
 Please refer to [data/README.md](data/README.md) for details.
 
-Some datasets require confirmation before using them, so we recommend logging in with your HuggingFace account using these commands.
+Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
 pip install --upgrade huggingface_hub
 huggingface-cli login
 ```
 
 ## Fine-Tuning Methods
@@ -224,66 +231,75 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
+
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
@@ -338,18 +354,18 @@
   - Official implementation of fine-tuning ChatGLM with [P-Tuning v2](https://github.com/THUDM/P-tuning-v2) on the [ADGEN](https://aclanthology.org/D19-1321.pdf) dataset.
   - Our fine-tuning script is largely depend on it. We further implement the [LoRA](https://arxiv.org/abs/2106.09685) tuning method. Additionally, we **dynamically** pad the inputs to the longest sequence in the batch instead of the maximum length, to accelerate the fine-tuning.
 - [mymusise/ChatGLM-Tuning](https://github.com/mymusise/ChatGLM-Tuning)
   - An unoffical implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
   - We borrowed some ideas from it. Our fine-tuning script **integrates** the data pre-processing part into the training procedure, so we need not generate a pre-processed dataset before training.
 - [ssbuild/chatglm_finetuning](https://github.com/ssbuild/chatglm_finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several PEFT methods on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - Our fine-tuning script is implemented **purely** with [Huggingface transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
+  - Our fine-tuning script is implemented **purely** with [Hugging Face transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
 - [lich99/ChatGLM-finetune-LoRA](https://github.com/lich99/ChatGLM-finetune-LoRA)
   - An unofficial implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - We use the [Huggingface PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
+  - We use the [Hugging Face PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
 - [liucongg/ChatGLM-Finetuning](https://github.com/liucongg/ChatGLM-Finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several methods including Freeze, LoRA and P-Tuning on the industrial dataset.
   - We are aim to incorporate more instruction-following datasets for fine-tuning the ChatGLM model.
 - [yanqiangmiffy/InstructGLM](https://github.com/yanqiangmiffy/InstructGLM)
   - An unofficial implementation of fine-tuning ChatGLM that explores the ChatGLM's ability on the instruction-following datasets.
   - Our fine-tuning script integrates the data pre-processing part in to the training procedure.
```

### Comparing `glmtuner-0.1.3/README.md` & `glmtuner-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,36 +38,43 @@
 
 [23/04/12] Now we support **training from checkpoints**! Use `--checkpoint_dir` argument to specify the checkpoint model to fine-tune from.
 
 [23/04/11] Now we support training with **combined datasets**! Try `--dataset dataset1,dataset2` argument for training with multiple datasets.
 
 ## Datasets
 
-Our script now supports the following datasets:
-
-- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-- [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-- [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-- [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-- [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-- [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-- [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-- [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-- [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-- [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-- [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-- [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-- [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-- [UltraChat](https://github.com/thunlp/UltraChat)
-- [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For supervised fine-tuning:
+  - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
+  - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [Self-cognition (zh)](data/self_cognition.json)
+  - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
+  - [RefGPT (zh)](https://github.com/sufengniu/RefGPT)
+  - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
+  - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
+  - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+  - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+  - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
+  - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
+  - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+  - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
+  - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
+  - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
+  - [UltraChat (en)](https://github.com/thunlp/UltraChat)
+  - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For reward modelling:
+  - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 
 Please refer to [data/README.md](data/README.md) for details.
 
-Some datasets require confirmation before using them, so we recommend logging in with your HuggingFace account using these commands.
+Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
 pip install --upgrade huggingface_hub
 huggingface-cli login
 ```
 
 ## Fine-Tuning Methods
@@ -200,66 +207,75 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
+
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
@@ -314,18 +330,18 @@
   - Official implementation of fine-tuning ChatGLM with [P-Tuning v2](https://github.com/THUDM/P-tuning-v2) on the [ADGEN](https://aclanthology.org/D19-1321.pdf) dataset.
   - Our fine-tuning script is largely depend on it. We further implement the [LoRA](https://arxiv.org/abs/2106.09685) tuning method. Additionally, we **dynamically** pad the inputs to the longest sequence in the batch instead of the maximum length, to accelerate the fine-tuning.
 - [mymusise/ChatGLM-Tuning](https://github.com/mymusise/ChatGLM-Tuning)
   - An unoffical implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
   - We borrowed some ideas from it. Our fine-tuning script **integrates** the data pre-processing part into the training procedure, so we need not generate a pre-processed dataset before training.
 - [ssbuild/chatglm_finetuning](https://github.com/ssbuild/chatglm_finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several PEFT methods on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - Our fine-tuning script is implemented **purely** with [Huggingface transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
+  - Our fine-tuning script is implemented **purely** with [Hugging Face transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
 - [lich99/ChatGLM-finetune-LoRA](https://github.com/lich99/ChatGLM-finetune-LoRA)
   - An unofficial implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - We use the [Huggingface PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
+  - We use the [Hugging Face PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
 - [liucongg/ChatGLM-Finetuning](https://github.com/liucongg/ChatGLM-Finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several methods including Freeze, LoRA and P-Tuning on the industrial dataset.
   - We are aim to incorporate more instruction-following datasets for fine-tuning the ChatGLM model.
 - [yanqiangmiffy/InstructGLM](https://github.com/yanqiangmiffy/InstructGLM)
   - An unofficial implementation of fine-tuning ChatGLM that explores the ChatGLM's ability on the instruction-following datasets.
   - Our fine-tuning script integrates the data pre-processing part in to the training procedure.
```

### Comparing `glmtuner-0.1.3/setup.py` & `glmtuner-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/api/app.py` & `glmtuner-0.1.4/src/glmtuner/api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from contextlib import asynccontextmanager
 from sse_starlette import EventSourceResponse
 from typing import List, Tuple
 
@@ -27,17 +26,15 @@
 
 @asynccontextmanager
 async def lifespan(app: FastAPI): # collects GPU memory
     yield
     torch_gc()
 
 
-def create_app():
-    chat_model = ChatModel(*get_infer_args())
-
+def create_app(chat_model: ChatModel) -> FastAPI:
     app = FastAPI(lifespan=lifespan)
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_credentials=True,
         allow_methods=["*"],
@@ -92,38 +89,39 @@
     async def predict(query: str, history: List[Tuple[str, str]], prefix: str, request: ChatCompletionRequest):
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(role=Role.ASSISTANT),
             finish_reason=None
         )
         chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-        yield json.dumps(chunk, ensure_ascii=False)
+        yield chunk.json(exclude_unset=True, ensure_ascii=False)
 
         for new_text in chat_model.stream_chat(
             query, history, prefix, temperature=request.temperature, top_p=request.top_p, max_new_tokens=request.max_tokens
         ):
             if len(new_text) == 0:
                 continue
 
             choice_data = ChatCompletionResponseStreamChoice(
                 index=0,
                 delta=DeltaMessage(content=new_text),
                 finish_reason=None
             )
             chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-            yield json.dumps(chunk, ensure_ascii=False)
+            yield chunk.json(exclude_unset=True, ensure_ascii=False)
 
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(),
             finish_reason=Finish.STOP
         )
         chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data])
-        yield json.dumps(chunk, ensure_ascii=False)
+        yield chunk.json(exclude_unset=True, ensure_ascii=False)
         yield "[DONE]"
 
     return app
 
 
 if __name__ == "__main__":
-    app = create_app()
+    chat_model = ChatModel(*get_infer_args())
+    app = create_app(chat_model)
     uvicorn.run(app, host="0.0.0.0", port=8000, workers=1)
```

### Comparing `glmtuner-0.1.3/src/glmtuner/api/protocol.py` & `glmtuner-0.1.4/src/glmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/chat/stream_chat.py` & `glmtuner-0.1.4/src/glmtuner/chat/stream_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,33 +23,33 @@
         if torch.cuda.device_count() > 1:
             from accelerate import dispatch_model
             device_map = auto_configure_device_map(torch.cuda.device_count(), use_v2=(self.tokenizer.eos_token_id==2))
             self.model = dispatch_model(self.model, device_map)
         else:
             self.model = self.model.cuda()
 
-        self.source_prefix = data_args.source_prefix if data_args.source_prefix else ""
+        self.source_prefix = data_args.source_prefix or ""
         self.generating_args = generating_args
 
     def get_prompt(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = None
     ) -> str:
         prefix = prefix + "\n" if prefix else "" # add separator for non-empty prefix
-        history = history if history else []
+        history = history or []
         prompt = ""
         for i, (old_query, response) in enumerate(history):
             prompt += "[Round {}]\n\n问：{}\n\n答：{}\n\n".format(i+1, old_query, response)
         prompt += "[Round {}]\n\n问：{}\n\n答：".format(len(history)+1, query)
         prompt = prefix + prompt
         return prompt
 
     def process_args(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = None, **input_kwargs
     ) -> Tuple[Dict[str, Any], int]:
-        prefix = prefix if prefix else self.source_prefix
+        prefix = prefix or self.source_prefix
 
         inputs = self.tokenizer([self.get_prompt(query, history, prefix)], return_tensors="pt")
         inputs = inputs.to(self.model.device)
         prompt_length = len(inputs["input_ids"][0])
 
         temperature = input_kwargs.pop("temperature", None)
         top_p = input_kwargs.pop("top_p", None)
@@ -96,9 +96,8 @@
         gen_kwargs, _ = self.process_args(query, history, prefix, **input_kwargs)
         streamer = TextIteratorStreamer(self.tokenizer, timeout=60.0, skip_prompt=True, skip_special_tokens=True)
         gen_kwargs["streamer"] = streamer
 
         thread = Thread(target=self.model.generate, kwargs=gen_kwargs)
         thread.start()
 
-        for new_text in streamer:
-            yield new_text
+        yield from streamer
```

### Comparing `glmtuner-0.1.3/src/glmtuner/dsets/collator.py` & `glmtuner-0.1.4/src/glmtuner/dsets/collator.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             input_ids = [torch.tensor(feature["input_ids"]).flip(0) for feature in features]
 
         if "labels" in features[0]:
             if isinstance(features[0]["labels"], torch.Tensor):
                 labels = [feature["labels"].clone().detach().flip(0) for feature in features]
             else:
                 labels = [torch.tensor(feature["labels"]).flip(0) for feature in features]
-            input_ids = input_ids + labels # pad them to the same length
+            input_ids += labels # pad them to the same length
 
         input_ids = torch.nn.utils.rnn.pad_sequence(
             input_ids,
             batch_first=True,
             padding_value=self.tokenizer.pad_token_id
         ).flip(-1)
```

### Comparing `glmtuner-0.1.3/src/glmtuner/dsets/loader.py` & `glmtuner-0.1.4/src/glmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/dsets/preprocess.py` & `glmtuner-0.1.4/src/glmtuner/dsets/preprocess.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/extras/callbacks.py` & `glmtuner-0.1.4/src/glmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/extras/logging.py` & `glmtuner-0.1.4/src/glmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/extras/misc.py` & `glmtuner-0.1.4/src/glmtuner/extras/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     layers_per_gpu = 30 / num_gpus
     if use_v2:
         device_map = {
             "transformer.embedding.word_embeddings": 0,
             "transformer.encoder.final_layernorm": 0,
             "transformer.output_layer": 0,
             "transformer.rotary_pos_emb": 0,
+            "transformer.prefix_encoder": 0,
             "lm_head": 0
         }
     else:
         device_map = {
             "transformer.word_embeddings": 0,
             "transformer.final_layernorm": 0,
             "transformer.prefix_encoder": 0,
```

### Comparing `glmtuner-0.1.3/src/glmtuner/extras/ploting.py` & `glmtuner-0.1.4/src/glmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/extras/save_and_load.py` & `glmtuner-0.1.4/src/glmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/hparams/data_args.py` & `glmtuner-0.1.4/src/glmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/hparams/finetuning_args.py` & `glmtuner-0.1.4/src/glmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/hparams/generating_args.py` & `glmtuner-0.1.4/src/glmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/hparams/model_args.py` & `glmtuner-0.1.4/src/glmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/core/adapter.py` & `glmtuner-0.1.4/src/glmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/core/loader.py` & `glmtuner-0.1.4/src/glmtuner/tuner/core/loader.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/core/parser.py` & `glmtuner-0.1.4/src/glmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/core/trainer.py` & `glmtuner-0.1.4/src/glmtuner/tuner/core/trainer.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/ppo/trainer.py` & `glmtuner-0.1.4/src/glmtuner/tuner/ppo/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,19 @@
                 response_length = (response_tensors[i] != self.tokenizer.pad_token_id).nonzero()[-1] + 1
                 queries.append(query_tensors[i, query_length:]) # remove padding from left
                 responses.append(response_tensors[i, :response_length]) # remove padding from right
 
             # Compute rewards
             replace_model(unwrapped_model, target="reward")
             with torch.no_grad():
-                _, _, values = self.model(**self.prepare_model_inputs(queries, responses))
+                _, _, values = self.model(
+                    **self.prepare_model_inputs(queries, responses),
+                    output_hidden_states=True,
+                    return_dict=True
+                )
             rewards = [reward for reward in values[-1].to(torch.float32)] # use float32 type
             replace_model(unwrapped_model, target="default")
 
             # Run PPO step
             unwrapped_model.gradient_checkpointing_enable()
             unwrapped_model.config.use_cache = False
             stats = self.step(queries, responses, rewards)
@@ -204,15 +208,15 @@
             response_batch = responses[i * fbs : (i + 1) * fbs]
             input_ids = input_kwargs["input_ids"] # left-padded sequences
 
             if self.is_distributed: # re-generate them to adapt padded inputs
                 input_kwargs["attention_mask"] = self.data_collator.get_attention_masks(input_ids, device=self.current_device)
                 input_kwargs["position_ids"] = self.data_collator.get_position_ids(input_ids, device=self.current_device)
 
-            logits, _, values = model(**input_kwargs)
+            logits, _, values = model(**input_kwargs, output_hidden_states=True, return_dict=True)
             logprobs = logprobs_from_logits(logits[:, :-1, :], input_ids[:, 1:])
             values = values.transpose(0, 1)
             masks = torch.zeros_like(input_ids)
 
             for j in range(fbs):
                 start = len(query_batch[j]) - 1
                 start += (input_ids[j] != self.tokenizer.pad_token_id).nonzero()[0].item()
```

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/ppo/utils.py` & `glmtuner-0.1.4/src/glmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/ppo/workflow.py` & `glmtuner-0.1.4/src/glmtuner/tuner/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/rm/collator.py` & `glmtuner-0.1.4/src/glmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/rm/trainer.py` & `glmtuner-0.1.4/src/glmtuner/tuner/rm/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,11 +28,11 @@
         Subclass and override to inject custom behavior. It should not be directly used by external scripts.
 
         Note that the first element will be removed from the output tuple.
 
         See: https://github.com/huggingface/transformers/blob/v4.30.2/src/transformers/trainer.py#L3509
         """
         batch_size = inputs["input_ids"].size(0) // 2
-        _, _, values = model(**inputs)
+        _, _, values = model(**inputs, output_hidden_states=True, return_dict=True)
         r_accept, r_reject = values[-1].split(batch_size, dim=0)
         loss = -torch.log(torch.sigmoid(r_accept - r_reject)).mean()
         return (loss, [loss, r_accept, r_reject]) if return_outputs else loss
```

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/rm/workflow.py` & `glmtuner-0.1.4/src/glmtuner/tuner/rm/workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/summarization/scripts/reward_summarization.py
 # https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
-from glmtuner.dsets import get_dataset, preprocess_dataset
+from glmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from glmtuner.extras.callbacks import LogCallback
 from glmtuner.extras.ploting import plot_loss
 from glmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from glmtuner.tuner.core import load_model_and_tokenizer
 from glmtuner.tuner.rm.metric import compute_accuracy
 from glmtuner.tuner.rm.collator import PairwiseDataCollatorForChatGLM
 from glmtuner.tuner.rm.trainer import PairwiseTrainerForChatGLM
@@ -25,34 +25,24 @@
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="rm")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="rm")
     data_collator = PairwiseDataCollatorForChatGLM(tokenizer, model.pretrained_model)
 
     training_args.remove_unused_columns = False # Important for pairwise dataset
 
-    # Split the dataset
-    if training_args.do_train:
-        if data_args.dev_ratio > 1e-6:
-            dataset = dataset.train_test_split(test_size=data_args.dev_ratio)
-            trainer_kwargs = {"train_dataset": dataset["train"], "eval_dataset": dataset["test"]}
-        else:
-            trainer_kwargs = {"train_dataset": dataset}
-    else: # do_eval or do_predict
-        trainer_kwargs = {"eval_dataset": dataset}
-
     # Initialize our Trainer
     trainer = PairwiseTrainerForChatGLM(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
         compute_metrics=compute_accuracy,
-        **trainer_kwargs
+        **split_dataset(dataset, data_args.dev_ratio, training_args.do_train)
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train()
         trainer.log_metrics("train", train_result.metrics)
         trainer.save_metrics("train", train_result.metrics)
```

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/sft/metric.py` & `glmtuner-0.1.4/src/glmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/sft/trainer.py` & `glmtuner-0.1.4/src/glmtuner/tuner/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/tuner/sft/workflow.py` & `glmtuner-0.1.4/src/glmtuner/tuner/sft/workflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Inspired by: https://github.com/THUDM/ChatGLM-6B/blob/main/ptuning/main.py
 
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
-from glmtuner.dsets import DataCollatorForChatGLM, get_dataset, preprocess_dataset
+from glmtuner.dsets import DataCollatorForChatGLM, get_dataset, preprocess_dataset, split_dataset
 from glmtuner.extras.callbacks import LogCallback
 from glmtuner.extras.misc import get_logits_processor
 from glmtuner.extras.ploting import plot_loss
 from glmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from glmtuner.tuner.core import load_model_and_tokenizer
 from glmtuner.tuner.sft.metric import ComputeMetrics
 from glmtuner.tuner.sft.trainer import Seq2SeqTrainerForChatGLM
@@ -31,34 +31,24 @@
 
     # Override the decoding parameters of Seq2SeqTrainer
     training_args.generation_max_length = training_args.generation_max_length if \
                 training_args.generation_max_length is not None else data_args.max_target_length
     training_args.generation_num_beams = data_args.eval_num_beams if \
                 data_args.eval_num_beams is not None else training_args.generation_num_beams
 
-    # Split the dataset
-    if training_args.do_train:
-        if data_args.dev_ratio > 1e-6:
-            dataset = dataset.train_test_split(test_size=data_args.dev_ratio)
-            trainer_kwargs = {"train_dataset": dataset["train"], "eval_dataset": dataset["test"]}
-        else:
-            trainer_kwargs = {"train_dataset": dataset}
-    else: # do_eval or do_predict
-        trainer_kwargs = {"eval_dataset": dataset}
-
     # Initialize our Trainer
     trainer = Seq2SeqTrainerForChatGLM(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
         compute_metrics=ComputeMetrics(tokenizer) if training_args.predict_with_generate else None,
-        **trainer_kwargs
+        **split_dataset(dataset, data_args.dev_ratio, training_args.do_train)
     )
 
     # Keyword arguments for `model.generate`
     gen_kwargs = {
         "do_sample": True,
         "top_p": 0.7,
         "max_new_tokens": data_args.max_target_length + 1,
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/chat.py` & `glmtuner-0.1.4/src/glmtuner/webui/chat.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,20 +66,21 @@
         yield ALERTS["info_unloaded"][lang]
 
     def predict(
         self,
         chatbot: List[Tuple[str, str]],
         query: str,
         history: List[Tuple[str, str]],
+        prefix: str,
         max_length: int,
         top_p: float,
         temperature: float
     ):
         chatbot.append([query, ""])
         response = ""
         for new_text in self.stream_chat(
-            query, history, max_length=max_length, top_p=top_p, temperature=temperature
+            query, history, prefix, max_length=max_length, top_p=top_p, temperature=temperature
         ):
             response += new_text
             new_history = history + [(query, response)]
             chatbot[-1] = [query, response]
             yield chatbot, new_history
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/common.py` & `glmtuner-0.1.4/src/glmtuner/webui/common.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/chatbot.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/chatbot.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,17 @@
     visible: Optional[bool] = False
 ) -> Tuple[Block, Component, Component, Dict[str, Component]]:
     with gr.Box(visible=visible) as chat_box:
         chatbot = gr.Chatbot()
 
         with gr.Row():
             with gr.Column(scale=4):
-                with gr.Column(scale=12):
-                    query = gr.Textbox(show_label=False, lines=8)
-
-                with gr.Column(min_width=32, scale=1):
-                    submit_btn = gr.Button(variant="primary")
+                prefix = gr.Dropdown(show_label=False)
+                query = gr.Textbox(show_label=False, lines=8)
+                submit_btn = gr.Button(variant="primary")
 
             with gr.Column(scale=1):
                 clear_btn = gr.Button()
                 max_length = gr.Slider(
                     10, 2048, value=chat_model.generating_args.max_length, step=1, interactive=True
                 )
                 top_p = gr.Slider(0.01, 1, value=chat_model.generating_args.top_p, step=0.01, interactive=True)
@@ -32,24 +30,25 @@
                     0.01, 1.5, value=chat_model.generating_args.temperature, step=0.01, interactive=True
                 )
 
     history = gr.State([])
 
     submit_btn.click(
         chat_model.predict,
-        [chatbot, query, history, max_length, top_p, temperature],
+        [chatbot, query, history, prefix, max_length, top_p, temperature],
         [chatbot, history],
         show_progress=True
     ).then(
         lambda: gr.update(value=""), outputs=[query]
     )
 
     clear_btn.click(lambda: ([], []), outputs=[chatbot, history], show_progress=True)
 
     return chat_box, chatbot, history, dict(
+        prefix=prefix,
         query=query,
         submit_btn=submit_btn,
         clear_btn=clear_btn,
         max_length=max_length,
         top_p=top_p,
         temperature=temperature
     )
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/data.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/eval.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         batch_size = gr.Slider(value=8, minimum=1, maximum=512, step=1)
         predict = gr.Checkbox(value=True)
 
     with gr.Row():
         start_btn = gr.Button()
         stop_btn = gr.Button()
 
-    output_box = gr.Markdown()
+    with gr.Box():
+        output_box = gr.Markdown()
 
     start_btn.click(
         runner.run_eval,
         [
             top_elems["lang"],
             top_elems["model_name"],
             top_elems["checkpoints"],
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/infer.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/infer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def create_infer_tab(top_elems: Dict[str, Component]) -> Dict[str, Component]:
     with gr.Row():
         load_btn = gr.Button()
         unload_btn = gr.Button()
 
-    info_box = gr.Markdown()
+    info_box = gr.Textbox(show_label=False, interactive=False)
 
     chat_model = WebChatModel()
     chat_box, chatbot, history, chat_elems = create_chat_box(chat_model)
 
     load_btn.click(
         chat_model.load_model,
         [
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/sft.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/sft.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,29 +31,40 @@
 
     with gr.Row():
         batch_size = gr.Slider(value=4, minimum=1, maximum=512, step=1)
         gradient_accumulation_steps = gr.Slider(value=4, minimum=1, maximum=512, step=1)
         lr_scheduler_type = gr.Dropdown(
             value="cosine", choices=[scheduler.value for scheduler in SchedulerType]
         )
+        max_grad_norm = gr.Textbox(value="1.0")
         dev_ratio = gr.Slider(value=0, minimum=0, maximum=1, step=0.001)
-        fp16 = gr.Checkbox(value=True)
 
-    with gr.Row():
-        logging_steps = gr.Slider(value=5, minimum=5, maximum=1000, step=5)
-        save_steps = gr.Slider(value=100, minimum=10, maximum=5000, step=10)
+    with gr.Accordion(label="Advanced config", open=False) as advanced_tab:
+        with gr.Row():
+            logging_steps = gr.Slider(value=5, minimum=5, maximum=1000, step=5)
+            save_steps = gr.Slider(value=100, minimum=10, maximum=5000, step=10)
+            warmup_steps = gr.Slider(value=0, minimum=0, maximum=5000, step=1)
+            compute_type = gr.Radio(choices=["fp16", "bf16"], value="fp16")
+
+    with gr.Accordion(label="LoRA config", open=False) as lora_tab:
+        with gr.Row():
+            lora_rank = gr.Slider(value=8, minimum=1, maximum=1024, step=1, scale=1)
+            lora_dropout = gr.Slider(value=0, minimum=0, maximum=1, step=0.01, scale=1)
+            lora_target = gr.Textbox(scale=2)
 
     with gr.Row():
         start_btn = gr.Button()
         stop_btn = gr.Button()
 
     with gr.Row():
         with gr.Column(scale=4):
             output_dir = gr.Textbox(interactive=True)
-            output_box = gr.Markdown()
+
+            with gr.Box():
+                output_box = gr.Markdown()
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot()
 
     start_btn.click(
         runner.run_train,
         [
@@ -69,18 +80,23 @@
             max_target_length,
             learning_rate,
             num_train_epochs,
             max_samples,
             batch_size,
             gradient_accumulation_steps,
             lr_scheduler_type,
+            max_grad_norm,
             dev_ratio,
-            fp16,
             logging_steps,
             save_steps,
+            warmup_steps,
+            compute_type,
+            lora_rank,
+            lora_dropout,
+            lora_target,
             output_dir
         ],
         [output_box]
     )
     stop_btn.click(runner.set_abort, queue=False)
 
     output_box.change(
@@ -98,17 +114,24 @@
         max_target_length=max_target_length,
         learning_rate=learning_rate,
         num_train_epochs=num_train_epochs,
         max_samples=max_samples,
         batch_size=batch_size,
         gradient_accumulation_steps=gradient_accumulation_steps,
         lr_scheduler_type=lr_scheduler_type,
+        max_grad_norm=max_grad_norm,
         dev_ratio=dev_ratio,
-        fp16=fp16,
+        advanced_tab=advanced_tab,
         logging_steps=logging_steps,
         save_steps=save_steps,
+        warmup_steps=warmup_steps,
+        compute_type=compute_type,
+        lora_tab=lora_tab,
+        lora_rank=lora_rank,
+        lora_dropout=lora_dropout,
+        lora_target=lora_target,
         start_btn=start_btn,
         stop_btn=stop_btn,
         output_dir=output_dir,
         output_box=output_box,
         loss_viewer=loss_viewer
     )
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/components/top.py` & `glmtuner-0.1.4/src/glmtuner/webui/components/top.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,18 @@
         model_path = gr.Textbox(scale=3)
 
     with gr.Row():
         finetuning_type = gr.Dropdown(value="lora", choices=METHODS, scale=1)
         checkpoints = gr.Dropdown(multiselect=True, scale=5)
         refresh_btn = gr.Button(scale=1)
 
-    with gr.Row():
-        quantization_bit = gr.Dropdown([8, 4], scale=1)
-        source_prefix = gr.Textbox(scale=6)
+    with gr.Accordion(label="Advanced config", open=False) as advanced_tab:
+        with gr.Row():
+            quantization_bit = gr.Dropdown([8, 4], scale=1)
+            source_prefix = gr.Textbox(scale=4)
 
     model_name.change(
         get_model_path, [model_name], [model_path]
     ).then(
         list_checkpoint, [model_name, finetuning_type], [checkpoints]
     ) # do not save config since the below line will save
     model_path.change(save_config, [model_name, model_path])
@@ -43,10 +44,11 @@
     return dict(
         lang=lang,
         model_name=model_name,
         model_path=model_path,
         finetuning_type=finetuning_type,
         checkpoints=checkpoints,
         refresh_btn=refresh_btn,
+        advanced_tab=advanced_tab,
         quantization_bit=quantization_bit,
         source_prefix=source_prefix
     )
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/interface.py` & `glmtuner-0.1.4/src/glmtuner/webui/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         with gr.Tab("SFT"):
             sft_elems = create_sft_tab(top_elems, runner)
 
         with gr.Tab("Evaluate"):
             eval_elems = create_eval_tab(top_elems, runner)
 
-        with gr.Tab("Inference"):
+        with gr.Tab("Chat"):
             infer_elems = create_infer_tab(top_elems)
 
         elem_list = [top_elems, sft_elems, eval_elems, infer_elems]
         manager = Manager(elem_list)
 
         demo.load(
             manager.gen_label,
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/locales.py` & `glmtuner-0.1.4/src/glmtuner/webui/locales.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,22 @@
         "en": {
             "value": "Refresh checkpoints"
         },
         "zh": {
             "value": "刷新断点"
         }
     },
+    "advanced_tab": {
+        "en": {
+            "label": "Advanced configurations"
+        },
+        "zh": {
+            "label": "高级设置"
+        }
+    },
     "quantization_bit": {
         "en": {
             "label": "Quantization bit (optional)",
             "info": "Enable 4/8-bit model quantization."
         },
         "zh": {
             "label": "量化等级（非必填）",
@@ -67,20 +75,20 @@
         "zh": {
             "label": "提示模板",
             "info": "构建提示词时使用的模板"
         }
     },
     "source_prefix": {
         "en": {
-            "label": "Source prefix (optional)",
-            "info": "A sequence used as the prefix of each samples."
+            "label": "System prompt (optional)",
+            "info": "A sequence used as the default system prompt."
         },
         "zh": {
-            "label": "前缀序列（非必填）",
-            "info": "作为每个输入样本前缀的序列"
+            "label": "系统提示词（非必填）",
+            "info": "默认使用的系统提示词"
         }
     },
     "dataset_dir": {
         "en": {
             "label": "Data dir",
             "info": "Path of the data directory."
         },
@@ -205,54 +213,112 @@
             "info": "Name of learning rate scheduler.",
         },
         "zh": {
             "label": "学习率调节器",
             "info": "采用的学习率调节器名称。"
         }
     },
-    "dev_ratio": {
+    "max_grad_norm": {
         "en": {
-            "label": "Dev ratio",
-            "info": "Proportion of data in the dev set."
+            "label": "Maximum gradient norm",
+            "info": "Norm for gradient clipping.."
         },
         "zh": {
-            "label": "验证集比例",
-            "info": "验证集占全部样本的百分比。"
+            "label": "最大梯度范数",
+            "info": "用于梯度裁剪的范数。"
         }
     },
-    "fp16": {
+    "dev_ratio": {
         "en": {
-            "label": "fp16",
-            "info": "Whether to use fp16 mixed precision training."
+            "label": "Dev ratio",
+            "info": "Proportion of data in the dev set."
         },
         "zh": {
-            "label": "fp16",
-            "info": "是否启用 FP16 混合精度训练。"
+            "label": "验证集比例",
+            "info": "验证集占全部样本的百分比。"
         }
     },
     "logging_steps": {
         "en": {
             "label": "Logging steps",
-            "info": "Number of update steps between two logs."
+            "info": "Number of steps between two logs."
         },
         "zh": {
             "label": "日志间隔",
             "info": "每两次日志输出间的更新步数。"
         }
     },
     "save_steps": {
         "en": {
             "label": "Save steps",
-            "info": "Number of updates steps between two checkpoints."
+            "info": "Number of steps between two checkpoints."
         },
         "zh": {
             "label": "保存间隔",
             "info": "每两次断点保存间的更新步数。"
         }
     },
+    "warmup_steps": {
+        "en": {
+            "label": "Warmup steps",
+            "info": "Number of steps used for warmup."
+        },
+        "zh": {
+            "label": "预热步数",
+            "info": "学习率预热采用的步数。"
+        }
+    },
+    "compute_type": {
+        "en": {
+            "label": "Compute type",
+            "info": "Whether to use fp16 or bf16 mixed precision training."
+        },
+        "zh": {
+            "label": "计算类型",
+            "info": "是否启用 FP16 或 BF16 混合精度训练。"
+        }
+    },
+    "lora_tab": {
+        "en": {
+            "label": "LoRA configurations"
+        },
+        "zh": {
+            "label": "LoRA 参数设置"
+        }
+    },
+    "lora_rank": {
+        "en": {
+            "label": "LoRA rank",
+            "info": "The rank of LoRA matrices."
+        },
+        "zh": {
+            "label": "LoRA 秩",
+            "info": "LoRA 矩阵的秩。"
+        }
+    },
+    "lora_dropout": {
+        "en": {
+            "label": "LoRA Dropout",
+            "info": "Dropout ratio of LoRA weights."
+        },
+        "zh": {
+            "label": "LoRA 随机丢弃",
+            "info": "LoRA 权重随机丢弃的概率。"
+        }
+    },
+    "lora_target": {
+        "en": {
+            "label": "LoRA modules (optional)",
+            "info": "The name(s) of target modules to apply LoRA. Use commas to separate multiple modules."
+        },
+        "zh": {
+            "label": "LoRA 作用层（非必填）",
+            "info": "应用 LoRA 的线性层名称。使用英文逗号分隔多个名称。"
+        }
+    },
     "start_btn": {
         "en": {
             "value": "Start"
         },
         "zh": {
             "value": "开始"
         }
@@ -319,14 +385,22 @@
         "en": {
             "value": "Model unloaded, please load a model first."
         },
         "zh": {
             "value": "模型未加载，请先加载模型。"
         }
     },
+    "prefix": {
+        "en": {
+            "placeholder": "System prompt (optional)"
+        },
+        "zh": {
+            "placeholder": "系统提示词（非必填）"
+        }
+    },
     "query": {
         "en": {
             "placeholder": "Input..."
         },
         "zh": {
             "placeholder": "输入..."
         }
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/manager.py` & `glmtuner-0.1.4/src/glmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/runner.py` & `glmtuner-0.1.4/src/glmtuner/webui/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,23 @@
         max_target_length: int,
         learning_rate: str,
         num_train_epochs: str,
         max_samples: str,
         batch_size: int,
         gradient_accumulation_steps: int,
         lr_scheduler_type: str,
+        max_grad_norm: str,
         dev_ratio: float,
-        fp16: bool,
         logging_steps: int,
         save_steps: int,
+        warmup_steps: int,
+        compute_type: str,
+        lora_rank: int,
+        lora_dropout: float,
+        lora_target: str,
         output_dir: str
     ):
         model_name_or_path, error, logger_handler, trainer_callback = self.initialize(lang, model_name, dataset)
         if error:
             yield error
             return
 
@@ -107,17 +112,23 @@
             max_target_length=max_target_length,
             learning_rate=float(learning_rate),
             num_train_epochs=float(num_train_epochs),
             max_samples=int(max_samples),
             per_device_train_batch_size=batch_size,
             gradient_accumulation_steps=gradient_accumulation_steps,
             lr_scheduler_type=lr_scheduler_type,
-            fp16=fp16,
+            max_grad_norm=float(max_grad_norm),
             logging_steps=logging_steps,
             save_steps=save_steps,
+            warmup_steps=warmup_steps,
+            fp16=(compute_type == "fp16"),
+            bf16=(compute_type == "bf16"),
+            lora_rank=lora_rank,
+            lora_dropout=lora_dropout,
+            lora_target=lora_target or "query_key_value",
             output_dir=os.path.join(get_save_dir(model_name), finetuning_type, output_dir)
         )
 
         if dev_ratio > 1e-6:
             args["dev_ratio"] = dev_ratio
             args["evaluation_strategy"] = "steps"
             args["eval_steps"] = save_steps
```

### Comparing `glmtuner-0.1.3/src/glmtuner/webui/utils.py` & `glmtuner-0.1.4/src/glmtuner/webui/utils.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.3/src/glmtuner.egg-info/PKG-INFO` & `glmtuner-0.1.4/src/glmtuner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -62,36 +62,43 @@
 
 [23/04/12] Now we support **training from checkpoints**! Use `--checkpoint_dir` argument to specify the checkpoint model to fine-tune from.
 
 [23/04/11] Now we support training with **combined datasets**! Try `--dataset dataset1,dataset2` argument for training with multiple datasets.
 
 ## Datasets
 
-Our script now supports the following datasets:
-
-- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-- [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-- [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-- [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-- [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-- [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-- [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-- [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-- [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-- [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-- [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-- [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-- [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-- [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-- [UltraChat](https://github.com/thunlp/UltraChat)
-- [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For supervised fine-tuning:
+  - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
+  - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [Self-cognition (zh)](data/self_cognition.json)
+  - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
+  - [RefGPT (zh)](https://github.com/sufengniu/RefGPT)
+  - [Guanaco Dataset (multilingual)](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
+  - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
+  - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
+  - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
+  - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
+  - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
+  - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
+  - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
+  - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
+  - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
+  - [UltraChat (en)](https://github.com/thunlp/UltraChat)
+  - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
+- For reward modelling:
+  - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
+  - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
+  - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 
 Please refer to [data/README.md](data/README.md) for details.
 
-Some datasets require confirmation before using them, so we recommend logging in with your HuggingFace account using these commands.
+Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
 pip install --upgrade huggingface_hub
 huggingface-cli login
 ```
 
 ## Fine-Tuning Methods
@@ -224,66 +231,75 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
+
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_chatglm_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
@@ -338,18 +354,18 @@
   - Official implementation of fine-tuning ChatGLM with [P-Tuning v2](https://github.com/THUDM/P-tuning-v2) on the [ADGEN](https://aclanthology.org/D19-1321.pdf) dataset.
   - Our fine-tuning script is largely depend on it. We further implement the [LoRA](https://arxiv.org/abs/2106.09685) tuning method. Additionally, we **dynamically** pad the inputs to the longest sequence in the batch instead of the maximum length, to accelerate the fine-tuning.
 - [mymusise/ChatGLM-Tuning](https://github.com/mymusise/ChatGLM-Tuning)
   - An unoffical implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
   - We borrowed some ideas from it. Our fine-tuning script **integrates** the data pre-processing part into the training procedure, so we need not generate a pre-processed dataset before training.
 - [ssbuild/chatglm_finetuning](https://github.com/ssbuild/chatglm_finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several PEFT methods on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - Our fine-tuning script is implemented **purely** with [Huggingface transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
+  - Our fine-tuning script is implemented **purely** with [Hugging Face transformers](https://github.com/huggingface/transformers) and is independent of the [deep_training](https://github.com/ssbuild/deep_training) framework.
 - [lich99/ChatGLM-finetune-LoRA](https://github.com/lich99/ChatGLM-finetune-LoRA)
   - An unofficial implementation of fine-tuning ChatGLM with [LoRA](https://arxiv.org/abs/2106.09685) on the [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca) dataset.
-  - We use the [Huggingface PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
+  - We use the [Hugging Face PEFT](https://github.com/huggingface/peft) to provide the state-of-the-art PEFT methods.
 - [liucongg/ChatGLM-Finetuning](https://github.com/liucongg/ChatGLM-Finetuning)
   - An unofficial implementation of fine-tuning ChatGLM with several methods including Freeze, LoRA and P-Tuning on the industrial dataset.
   - We are aim to incorporate more instruction-following datasets for fine-tuning the ChatGLM model.
 - [yanqiangmiffy/InstructGLM](https://github.com/yanqiangmiffy/InstructGLM)
   - An unofficial implementation of fine-tuning ChatGLM that explores the ChatGLM's ability on the instruction-following datasets.
   - Our fine-tuning script integrates the data pre-processing part in to the training procedure.
```

### Comparing `glmtuner-0.1.3/src/glmtuner.egg-info/SOURCES.txt` & `glmtuner-0.1.4/src/glmtuner.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/glmtuner/api/protocol.py
 src/glmtuner/chat/__init__.py
 src/glmtuner/chat/stream_chat.py
 src/glmtuner/dsets/__init__.py
 src/glmtuner/dsets/collator.py
 src/glmtuner/dsets/loader.py
 src/glmtuner/dsets/preprocess.py
+src/glmtuner/dsets/utils.py
 src/glmtuner/extras/__init__.py
 src/glmtuner/extras/callbacks.py
 src/glmtuner/extras/constants.py
 src/glmtuner/extras/logging.py
 src/glmtuner/extras/misc.py
 src/glmtuner/extras/ploting.py
 src/glmtuner/extras/save_and_load.py
```

