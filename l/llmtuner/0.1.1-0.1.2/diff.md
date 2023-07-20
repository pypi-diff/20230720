# Comparing `tmp/llmtuner-0.1.1.tar.gz` & `tmp/llmtuner-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.1.1.tar", last modified: Tue Jul 18 12:51:58 2023, max compression
+gzip compressed data, was "llmtuner-0.1.2.tar", last modified: Thu Jul 20 14:33:27 2023, max compression
```

## Comparing `llmtuner-0.1.1.tar` & `llmtuner-0.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.806001 llmtuner-0.1.1/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-18 12:51:17.000000 llmtuner-0.1.1/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14220 2023-07-18 12:51:58.806001 llmtuner-0.1.1/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13593 2023-07-18 12:51:23.000000 llmtuner-0.1.1/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-18 12:51:23.000000 llmtuner-0.1.1/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-18 12:51:58.806001 llmtuner-0.1.1/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-18 12:51:24.000000 llmtuner-0.1.1/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.501988 llmtuner-0.1.1/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.513988 llmtuner-0.1.1/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      258 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.521989 llmtuner-0.1.1/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4554 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.525989 llmtuner-0.1.1/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3737 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.533989 llmtuner-0.1.1/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      105 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2565 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/dsets/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8194 2023-07-18 12:51:18.000000 llmtuner-0.1.1/src/llmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.565991 llmtuner-0.1.1/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3138 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1410 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5775 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.581991 llmtuner-0.1.1/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3739 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-18 12:51:19.000000 llmtuner-0.1.1/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.581991 llmtuner-0.1.1/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.645994 llmtuner-0.1.1/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7094 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-18 12:51:20.000000 llmtuner-0.1.1/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.653994 llmtuner-0.1.1/src/llmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8094 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.657994 llmtuner-0.1.1/src/llmtuner/tuner/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2884 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.717997 llmtuner-0.1.1/src/llmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1482 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2854 2023-07-18 12:51:21.000000 llmtuner-0.1.1/src/llmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.741998 llmtuner-0.1.1/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2183 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4162 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4264 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.786000 llmtuner-0.1.1/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2739 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.802000 llmtuner-0.1.1/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1859 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2543 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1390 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4132 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1952 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-18 12:51:22.000000 llmtuner-0.1.1/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1461 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10687 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7723 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2896 2023-07-18 12:51:23.000000 llmtuner-0.1.1/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-18 12:51:58.517989 llmtuner-0.1.1/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14220 2023-07-18 12:51:57.000000 llmtuner-0.1.1/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2238 2023-07-18 12:51:58.000000 llmtuner-0.1.1/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-18 12:51:57.000000 llmtuner-0.1.1/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      198 2023-07-18 12:51:57.000000 llmtuner-0.1.1/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-18 12:51:57.000000 llmtuner-0.1.1/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.086244 llmtuner-0.1.2/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-20 14:33:04.000000 llmtuner-0.1.2/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-20 14:33:27.086244 llmtuner-0.1.2/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-20 14:33:09.000000 llmtuner-0.1.2/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-20 14:33:09.000000 llmtuner-0.1.2/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-20 14:33:27.086244 llmtuner-0.1.2/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-20 14:33:09.000000 llmtuner-0.1.2/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.838234 llmtuner-0.1.2/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.886236 llmtuner-0.1.2/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.906237 llmtuner-0.1.2/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.926237 llmtuner-0.1.2/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3670 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.934238 llmtuner-0.1.2/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8202 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      515 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.950239 llmtuner-0.1.2/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3138 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6500 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.966239 llmtuner-0.1.2/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.966239 llmtuner-0.1.2/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.986240 llmtuner-0.1.2/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7187 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.994240 llmtuner-0.1.2/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8221 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.018241 llmtuner-0.1.2/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2516 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.030242 llmtuner-0.1.2/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1527 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2486 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.038242 llmtuner-0.1.2/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2183 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4553 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3896 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.066243 llmtuner-0.1.2/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2769 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.082244 llmtuner-0.1.2/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1837 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1424 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5132 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2081 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1456 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12736 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8072 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2896 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.902237 llmtuner-0.1.2/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2234 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.1.1/LICENSE` & `llmtuner-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/PKG-INFO` & `llmtuner-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -30,37 +30,40 @@
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
-[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [HuggingFace Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
+[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model. If you want to train with RTX3090, use `git checkout baichuan-7b-rtx3090` to switch to the `baichuan-7b-rtx3090` branch and try the `--baichuan_rtx_gpu true` argument. (Other RTX series GPUs can also be tried)
+[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
 [23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
+- [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
 - [BLOOM](https://huggingface.co/bigscience/bloom) & [BLOOMZ](https://huggingface.co/bigscience/bloomz) (560M/1.1B/1.7B/3B/7.1B/176B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B/40B)
 - [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Supported Training Approaches
 
@@ -77,44 +80,44 @@
 - [RLHF](https://arxiv.org/abs/2203.02155)
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
-  - [Wiki Demo](data/wiki_demo.txt)
+  - [Wiki Demo (en)](data/wiki_demo.txt)
 - For supervised fine-tuning:
-  - [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-  - [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-  - [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-  - [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-  - [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-  - [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-  - [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-  - [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-  - [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-  - [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-  - [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-  - [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-  - [UltraChat](https://github.com/thunlp/UltraChat)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
-- For reward model training:
-  - [HH-RLHF](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [GPT-4 Generated Data (Chinese)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
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
 
 ## Requirement
@@ -280,69 +283,93 @@
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage pt \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
+### Predict
+
+```bash
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
+    --model_name_or_path path_to_your_model \
+    --do_predict \
+    --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
+    --checkpoint_dir path_to_checkpoint \
+    --output_dir path_to_predict_result \
+    --per_device_eval_batch_size 8 \
+    --max_samples 100 \
+    --predict_with_generate
+```
+
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
+- [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
 - [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
```

### Comparing `llmtuner-0.1.1/README.md` & `llmtuner-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,37 +6,40 @@
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
-[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [HuggingFace Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
+[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model. If you want to train with RTX3090, use `git checkout baichuan-7b-rtx3090` to switch to the `baichuan-7b-rtx3090` branch and try the `--baichuan_rtx_gpu true` argument. (Other RTX series GPUs can also be tried)
+[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
 [23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
+- [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
 - [BLOOM](https://huggingface.co/bigscience/bloom) & [BLOOMZ](https://huggingface.co/bigscience/bloomz) (560M/1.1B/1.7B/3B/7.1B/176B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B/40B)
 - [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Supported Training Approaches
 
@@ -53,44 +56,44 @@
 - [RLHF](https://arxiv.org/abs/2203.02155)
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
-  - [Wiki Demo](data/wiki_demo.txt)
+  - [Wiki Demo (en)](data/wiki_demo.txt)
 - For supervised fine-tuning:
-  - [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-  - [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-  - [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-  - [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-  - [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-  - [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-  - [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-  - [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-  - [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-  - [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-  - [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-  - [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-  - [UltraChat](https://github.com/thunlp/UltraChat)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
-- For reward model training:
-  - [HH-RLHF](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [GPT-4 Generated Data (Chinese)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
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
 
 ## Requirement
@@ -256,69 +259,93 @@
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage pt \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
+### Predict
+
+```bash
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
+    --model_name_or_path path_to_your_model \
+    --do_predict \
+    --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
+    --checkpoint_dir path_to_checkpoint \
+    --output_dir path_to_predict_result \
+    --per_device_eval_batch_size 8 \
+    --max_samples 100 \
+    --predict_with_generate
+```
+
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
+- [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
 - [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
```

### Comparing `llmtuner-0.1.1/setup.py` & `llmtuner-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/api/app.py` & `llmtuner-0.1.2/src/llmtuner/api/app.py`

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

### Comparing `llmtuner-0.1.1/src/llmtuner/api/protocol.py` & `llmtuner-0.1.2/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/chat/stream_chat.py` & `llmtuner-0.1.2/src/llmtuner/chat/stream_chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import torch
 from typing import Any, Dict, Generator, List, Optional, Tuple
 from threading import Thread
 from transformers import TextIteratorStreamer
 
 from llmtuner.extras.misc import get_logits_processor
-from llmtuner.extras.template import Template
+from llmtuner.extras.template import get_template
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments
 from llmtuner.tuner import load_model_and_tokenizer
 
 
 class ChatModel:
 
     def __init__(
         self,
         model_args: ModelArguments,
         data_args: DataArguments,
         finetuning_args: FinetuningArguments,
         generating_args: GeneratingArguments
     ) -> None:
         self.model, self.tokenizer = load_model_and_tokenizer(model_args, finetuning_args)
-        self.template = Template(data_args.prompt_template)
-        self.source_prefix = data_args.source_prefix if data_args.source_prefix else ""
+        self.template = get_template(data_args.prompt_template)
+        self.source_prefix = data_args.source_prefix or ""
         self.generating_args = generating_args
 
     def process_args(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = None, **input_kwargs
     ) -> Tuple[Dict[str, Any], int]:
-        prefix = prefix if prefix else self.source_prefix
+        prefix = prefix or self.source_prefix
 
         inputs = self.tokenizer([self.template.get_prompt(query, history, prefix)], return_tensors="pt")
         inputs = inputs.to(self.model.device)
         prompt_length = len(inputs["input_ids"][0])
 
         temperature = input_kwargs.pop("temperature", None)
         top_p = input_kwargs.pop("top_p", None)
@@ -77,9 +77,8 @@
         gen_kwargs, _ = self.process_args(query, history, prefix, **input_kwargs)
         streamer = TextIteratorStreamer(self.tokenizer, timeout=60.0, skip_prompt=True, skip_special_tokens=True)
         gen_kwargs["streamer"] = streamer
 
         thread = Thread(target=self.model.generate, kwargs=gen_kwargs)
         thread.start()
 
-        for new_text in streamer:
-            yield new_text
+        yield from streamer
```

### Comparing `llmtuner-0.1.1/src/llmtuner/dsets/callbacks.py` & `llmtuner-0.1.2/src/llmtuner/extras/callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,74 @@
-import os
-import json
-import time
-from datetime import timedelta
-
-from transformers import (
-    TrainerCallback,
-    TrainerControl,
-    TrainerState,
-    TrainingArguments
-)
-
-
-class LogCallback(TrainerCallback):
-
-    def __init__(self, runner=None):
-        self.runner = runner
-        self.start_time = time.time()
-        self.tracker = {}
-
-    def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
-        r"""
-        Event called at the beginning of a training step. If using gradient accumulation, one training step
-        might take several inputs.
-        """
-        if self.runner is not None and self.runner.aborted:
-            control.should_epoch_stop = True
-            control.should_training_stop = True
-
-    def on_substep_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
-        r"""
-        Event called at the end of an substep during gradient accumulation.
-        """
-        if self.runner is not None and self.runner.aborted:
-            control.should_epoch_stop = True
-            control.should_training_stop = True
-
-    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
-        r"""
-        Event called after logging the last logs.
-        """
-        if "loss" not in state.log_history[-1]:
-            return
-        cur_time = time.time()
-        cur_steps = state.log_history[-1].get("step")
-        elapsed_time = cur_time - self.start_time
-        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
-        remaining_steps = state.max_steps - cur_steps
-        remaining_time = remaining_steps * avg_time_per_step
-        self.tracker = {
-            "current_steps": cur_steps,
-            "total_steps": state.max_steps,
-            "loss": state.log_history[-1].get("loss", None),
-            "reward": state.log_history[-1].get("reward", None),
-            "learning_rate": state.log_history[-1].get("learning_rate", None),
-            "epoch": state.log_history[-1].get("epoch", None),
-            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
-            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
-            "remaining_time": str(timedelta(seconds=int(remaining_time)))
-        }
-        os.makedirs(args.output_dir, exist_ok=True)
-        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a", encoding="utf-8") as f:
-            f.write(json.dumps(self.tracker) + "\n")
+import os
+import json
+import time
+from datetime import timedelta
+
+from transformers import (
+    TrainerCallback,
+    TrainerControl,
+    TrainerState,
+    TrainingArguments
+)
+from transformers.trainer_callback import TrainerControl, TrainerState
+from transformers.training_args import TrainingArguments
+
+
+class LogCallback(TrainerCallback):
+
+    def __init__(self, runner=None):
+        self.runner = runner
+        self.start_time = time.time()
+        self.tracker = {}
+
+    def on_train_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the beginning of training.
+        """
+        self.start_time = time.time()
+
+    def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the beginning of a training step. If using gradient accumulation, one training step
+        might take several inputs.
+        """
+        if self.runner is not None and self.runner.aborted:
+            control.should_epoch_stop = True
+            control.should_training_stop = True
+
+    def on_substep_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the end of an substep during gradient accumulation.
+        """
+        if self.runner is not None and self.runner.aborted:
+            control.should_epoch_stop = True
+            control.should_training_stop = True
+
+    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
+        r"""
+        Event called after logging the last logs.
+        """
+        if not state.is_world_process_zero:
+            return
+
+        cur_time = time.time()
+        cur_steps = state.log_history[-1].get("step")
+        elapsed_time = cur_time - self.start_time
+        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
+        remaining_steps = state.max_steps - cur_steps
+        remaining_time = remaining_steps * avg_time_per_step
+        self.tracker = {
+            "current_steps": cur_steps,
+            "total_steps": state.max_steps,
+            "loss": state.log_history[-1].get("loss", None),
+            "eval_loss": state.log_history[-1].get("eval_loss", None),
+            "predict_loss": state.log_history[-1].get("predict_loss", None),
+            "reward": state.log_history[-1].get("reward", None),
+            "learning_rate": state.log_history[-1].get("learning_rate", None),
+            "epoch": state.log_history[-1].get("epoch", None),
+            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
+            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
+            "remaining_time": str(timedelta(seconds=int(remaining_time)))
+        }
+        os.makedirs(args.output_dir, exist_ok=True)
+        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a", encoding="utf-8") as f:
+            f.write(json.dumps(self.tracker) + "\n")
```

### Comparing `llmtuner-0.1.1/src/llmtuner/dsets/loader.py` & `llmtuner-0.1.2/src/llmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/dsets/preprocess.py` & `llmtuner-0.1.2/src/llmtuner/dsets/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from itertools import chain
 from transformers import Seq2SeqTrainingArguments
 from transformers.tokenization_utils import PreTrainedTokenizer
 
 from datasets import Dataset
 
 from llmtuner.extras.constants import IGNORE_INDEX
-from llmtuner.extras.template import Template
+from llmtuner.extras.template import get_template
 from llmtuner.hparams import DataArguments
 
 
 def preprocess_dataset(
     dataset: Dataset,
     tokenizer: PreTrainedTokenizer,
     data_args: DataArguments,
     training_args: Seq2SeqTrainingArguments,
     stage: Literal["pt", "sft", "rm", "ppo"]
 ) -> Dataset:
 
     column_names = list(dataset.column_names)
-    prompt_template = Template(data_args.prompt_template)
+    prompt_template = get_template(data_args.prompt_template)
 
     # support question with a single answer or multiple answers
     def get_dialog(examples):
         for i in range(len(examples["prompt"])):
             if examples["prompt"][i] and examples["response"][i]:
                 query, answer = examples["prompt"][i], examples["response"][i]
                 query = query + "\n" + examples["query"][i] if examples["query"][i] else query
```

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/constants.py` & `llmtuner-0.1.2/src/llmtuner/extras/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 METHODS = ["full", "freeze", "lora"]
 
 SUPPORTED_MODELS = {
     "LLaMA-7B": "huggyllama/llama-7b",
     "LLaMA-13B": "huggyllama/llama-13b",
     "LLaMA-30B": "huggyllama/llama-30b",
     "LLaMA-65B": "huggyllama/llama-65b",
+    "LLaMA2-7B": "meta-llama/Llama-2-7b-hf",
+    "LLaMA2-13B": "meta-llama/Llama-2-13b-hf",
+    "LLaMA2-70B": "meta-llama/Llama-2-70b-hf",
+    "LLaMA2-7B-Chat": "meta-llama/Llama-2-7b-chat-hf",
+    "LLaMA2-13B-Chat": "meta-llama/Llama-2-13b-chat-hf",
+    "LLaMA2-70B-Chat": "meta-llama/Llama-2-70b-chat-hf",
     "BLOOM-560M": "bigscience/bloom-560m",
     "BLOOM-3B": "bigscience/bloom-3b",
     "BLOOM-7B1": "bigscience/bloom-7b1",
     "BLOOMZ-560M": "bigscience/bloomz-560m",
     "BLOOMZ-3B": "bigscience/bloomz-3b",
     "BLOOMZ-7B1-mt": "bigscience/bloomz-7b1-mt",
     "Falcon-7B-Base": "tiiuae/falcon-7b",
@@ -26,15 +32,16 @@
     "Baichuan-7B": "baichuan-inc/Baichuan-7B",
     "Baichuan-13B-Base": "baichuan-inc/Baichuan-13B-Base",
     "Baichuan-13B-Chat": "baichuan-inc/Baichuan-13B-Chat",
     "InternLM-7B-Base": "internlm/internlm-7b",
     "InternLM-7B-Chat": "internlm/internlm-chat-7b"
 }
 
-DEFAULT_MODULE = { # will be deprecated
+DEFAULT_MODULE = {
     "LLaMA": "q_proj,v_proj",
+    "LLaMA2": "q_proj,v_proj",
     "BLOOM": "query_key_value",
     "BLOOMZ": "query_key_value",
     "Falcon": "query_key_value",
     "Baichuan": "W_pack",
     "InternLM": "q_proj,v_proj"
 }
```

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/logging.py` & `llmtuner-0.1.2/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/misc.py` & `llmtuner-0.1.2/src/llmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/ploting.py` & `llmtuner-0.1.2/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.1.2/src/llmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/extras/template.py` & `llmtuner-0.1.2/src/llmtuner/extras/template.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,19 @@
 from typing import Dict, List, Optional, Tuple
 from dataclasses import dataclass
 
 
 @dataclass
-class Format:
+class Template:
+
     prefix: str
     prompt: str
     sep: str
     use_history: bool
 
-
-templates: Dict[str, Format] = {}
-
-
-@dataclass
-class Template:
-
-    name: str
-
-    def __post_init__(self):
-        if self.name in templates:
-            self.prefix = templates[self.name].prefix
-            self.prompt = templates[self.name].prompt
-            self.sep = templates[self.name].sep
-            self.use_history = templates[self.name].use_history
-        else:
-            raise ValueError("Template {} does not exist.".format(self.name))
-
     def get_prompt(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = ""
     ) -> str:
         r"""
         Returns a string containing prompt without response.
         """
         return "".join(self._format_example(query, history, prefix))
@@ -42,38 +25,47 @@
         Returns a list containing 2 * n elements where the 2k-th is a query and the (2k+1)-th is a response.
         """
         return self._format_example(query, history, prefix) + [resp]
 
     def _format_example(
         self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = ""
     ) -> List[str]:
-        prefix = prefix if prefix else self.prefix # use prefix if provided
+        prefix = prefix or self.prefix # use prefix if provided
         prefix = prefix + self.sep if prefix else "" # add separator for non-empty prefix
         history = history if (history and self.use_history) else []
         history = history + [(query, "<dummy>")]
         convs = []
         for turn_idx, (user_query, bot_resp) in enumerate(history):
             if turn_idx == 0:
                 convs.append(prefix + self.prompt.format(query=user_query))
                 convs.append(bot_resp)
             else:
                 convs.append(self.sep + self.prompt.format(query=user_query))
                 convs.append(bot_resp)
         return convs[:-1] # drop last
 
 
+templates: Dict[str, Template] = {}
+
+
 def register_template(name: str, prefix: str, prompt: str, sep: str, use_history: bool) -> None:
-    templates[name] = Format(
+    templates[name] = Template(
         prefix=prefix,
         prompt=prompt,
         sep=sep,
         use_history=use_history
     )
 
 
+def get_template(name: str) -> Template:
+    template = templates.get(name, None)
+    assert template is not None, "Template {} does not exist.".format(name)
+    return template
+
+
 r"""
 Supports language model inference without histories.
 """
 register_template(
     name="vanilla",
     prefix="",
     prompt="{query}",
@@ -92,14 +84,35 @@
     prompt="Human: {query}\nAssistant: ",
     sep="\n",
     use_history=True
 )
 
 
 r"""
+Supports: https://huggingface.co/meta-llama/Llama-2-7b-chat-hf
+          https://huggingface.co/meta-llama/Llama-2-13b-chat-hf
+          https://huggingface.co/meta-llama/Llama-2-70b-chat-hf
+"""
+register_template(
+    name="llama2",
+    prefix="<<SYS>>\nYou are a helpful, respectful and honest assistant. "
+           "Always answer as helpfully as possible, while being safe.  "
+           "Your answers should not include any harmful, unethical, "
+           "racist, sexist, toxic, dangerous, or illegal content. "
+           "Please ensure that your responses are socially unbiased and positive in nature.\n"
+           "If a question does not make any sense, or is not factually coherent, "
+           "explain why instead of answering something not correct. "
+           "If you don't know the answer to a question, please don't share false information.\n<</SYS>>\n\n",
+    prompt=" [INST] {query} [/INST] ",
+    sep="</s>",
+    use_history=True
+)
+
+
+r"""
 Supports: https://huggingface.co/tatsu-lab/alpaca-7b-wdiff
           https://github.com/ymcui/Chinese-LLaMA-Alpaca
 """
 register_template(
     name="alpaca",
     prefix="Below is an instruction that describes a task. "
            "Write a response that appropriately completes the request.",
@@ -198,15 +211,15 @@
 
 r"""
 Supports: https://huggingface.co/baichuan-inc/Baichuan-13B-Chat
 """
 register_template(
     name="baichuan",
     prefix="",
-    prompt=" <reserved_102> {query} <reserved_103> ",
+    prompt="<reserved_102>{query}<reserved_103>",
     sep="</s>",
     use_history=True
 )
 
 
 r"""
 Supports: https://huggingface.co/HuggingFaceH4/starchat-alpha
```

### Comparing `llmtuner-0.1.1/src/llmtuner/hparams/data_args.py` & `llmtuner-0.1.2/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.1.2/src/llmtuner/hparams/finetuning_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,26 +12,27 @@
         default="lora",
         metadata={"help": "Which fine-tuning method to use."}
     )
     num_hidden_layers: Optional[int] = field(
         default=32,
         metadata={"help": "Number of decoder blocks in the model. \
                   LLaMA choices: [\"32\", \"40\", \"60\", \"80\"], \
+                  LLaMA-2 choices: [\"32\", \"40\", \"80\"], \
                   BLOOM choices: [\"24\", \"30\", \"70\"], \
                   Falcon choices: [\"32\", \"60\"], \
-                  Baichuan choices: [\"32\"]"}
+                  Baichuan choices: [\"32\", \"40\"]"}
     )
     num_layer_trainable: Optional[int] = field(
         default=3,
         metadata={"help": "Number of trainable layers for Freeze fine-tuning."}
     )
     name_module_trainable: Optional[Literal["mlp", "self_attn", "self_attention"]] = field(
         default="mlp",
         metadata={"help": "Name of trainable modules for Freeze fine-tuning. \
-                  LLaMA choices: [\"mlp\", \"self_attn\"], \
+                  LLaMA & LLaMA-2 choices: [\"mlp\", \"self_attn\"], \
                   BLOOM & Falcon choices: [\"mlp\", \"self_attention\"], \
                   Baichuan choices: [\"mlp\", \"self_attn\"]"}
     )
     lora_rank: Optional[int] = field(
         default=8,
         metadata={"help": "The intrinsic dimension for LoRA fine-tuning."}
     )
@@ -42,15 +43,15 @@
     lora_dropout: Optional[float] = field(
         default=0.1,
         metadata={"help": "Dropout rate for the LoRA fine-tuning."}
     )
     lora_target: Optional[str] = field(
         default="q_proj,v_proj",
         metadata={"help": "Name(s) of target modules to apply LoRA. Use commas to separate multiple modules. \
-                  LLaMA choices: [\"q_proj\", \"k_proj\", \"v_proj\", \"o_proj\", \"gate_proj\", \"up_proj\", \"down_proj\"], \
+                  LLaMA & LLaMA-2 choices: [\"q_proj\", \"k_proj\", \"v_proj\", \"o_proj\", \"gate_proj\", \"up_proj\", \"down_proj\"], \
                   BLOOM & Falcon choices: [\"query_key_value\", \"self_attention.dense\", \"mlp.dense\"], \
                   Baichuan choices: [\"W_pack\", \"o_proj\", \"gate_proj\", \"up_proj\", \"down_proj\"]"}
     )
 
     def __post_init__(self):
         if isinstance(self.lora_target, str): # support custom target modules/layers of LoRA
             self.lora_target = [target.strip() for target in self.lora_target.split(",")]
```

### Comparing `llmtuner-0.1.1/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.1.2/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/hparams/model_args.py` & `llmtuner-0.1.2/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.1.2/src/llmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.1.2/src/llmtuner/tuner/core/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     AutoConfig,
     AutoModelForCausalLM,
     AutoTokenizer,
     BitsAndBytesConfig
 )
 from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
+from transformers.deepspeed import is_deepspeed_zero3_enabled
 from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizerBase
 from trl import AutoModelForCausalLMWithValueHead
 
 from llmtuner.extras.logging import get_logger
 from llmtuner.extras.misc import prepare_model_for_training, print_trainable_params
 from llmtuner.extras.save_and_load import load_valuehead_params
@@ -104,15 +105,15 @@
         model_to_load = model_args.model_name_or_path
 
     # Load and prepare pretrained models (without valuehead).
     model = AutoModelForCausalLM.from_pretrained(
         model_to_load,
         config=config,
         torch_dtype=torch.bfloat16 if model_args.compute_dtype == torch.bfloat16 else torch.float16,
-        low_cpu_mem_usage=True,
+        low_cpu_mem_usage=(not is_deepspeed_zero3_enabled()),
         **config_kwargs
     )
 
     # Register auto class to save the custom code files.
     if isinstance(config, PretrainedConfig) and "AutoConfig" in getattr(config, "auto_map", {}):
         config.__class__.register_for_auto_class()
     if isinstance(model, PreTrainedModel) and "AutoModelForCausalLM" in getattr(config, "auto_map", {}):
```

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.1.2/src/llmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.1.2/src/llmtuner/tuner/core/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/ppo/trainer.py` & `llmtuner-0.1.2/src/llmtuner/tuner/ppo/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,19 @@
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
             rewards = [reward for reward in values[:, -1].to(torch.float32)] # use float32 type
             replace_model(unwrapped_model, target="default")
 
             # Run PPO step
             unwrapped_model.gradient_checkpointing_enable()
             unwrapped_model.config.use_cache = False
             stats = self.step(queries, responses, rewards)
```

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/ppo/utils.py` & `llmtuner-0.1.2/src/llmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/ppo/workflow.py` & `llmtuner-0.1.2/src/llmtuner/tuner/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/pt/workflow.py` & `llmtuner-0.1.2/src/llmtuner/tuner/pt/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Inspired by: https://github.com/huggingface/transformers/blob/v4.29.2/examples/pytorch/language-modeling/run_clm.py
 
 import math
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, DataCollatorForSeq2Seq, TrainerCallback
 
-from llmtuner.dsets import get_dataset, preprocess_dataset
+from llmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.constants import IGNORE_INDEX
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.core.trainer import PeftTrainer
 
@@ -24,33 +24,23 @@
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="pt")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="pt")
     data_collator = DataCollatorForSeq2Seq(
         tokenizer=tokenizer,
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id
     )
 
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
     trainer = PeftTrainer(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
-        **trainer_kwargs
+        **split_dataset(dataset, data_args.dev_ratio, training_args.do_train)
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train()
         trainer.log_metrics("train", train_result.metrics)
         trainer.save_metrics("train", train_result.metrics)
```

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/rm/collator.py` & `llmtuner-0.1.2/src/llmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/rm/trainer.py` & `llmtuner-0.1.2/src/llmtuner/tuner/rm/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,11 +28,11 @@
         Subclass and override to inject custom behavior. It should not be directly used by external scripts.
 
         Note that the first element will be removed from the output tuple.
 
         See: https://github.com/huggingface/transformers/blob/v4.30.2/src/transformers/trainer.py#L3509
         """
         batch_size = inputs["input_ids"].size(0) // 2
-        _, _, values = model(**inputs)
+        _, _, values = model(**inputs, output_hidden_states=True, return_dict=True)
         r_accept, r_reject = values[:, -1].split(batch_size, dim=0)
         loss = -torch.log(torch.sigmoid(r_accept - r_reject)).mean()
         return (loss, [loss, r_accept, r_reject]) if return_outputs else loss
```

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/rm/workflow.py` & `llmtuner-0.1.2/src/llmtuner/tuner/rm/workflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/summarization/scripts/reward_summarization.py
 # https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
-from llmtuner.dsets import get_dataset, preprocess_dataset
+from llmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.rm.metric import compute_accuracy
 from llmtuner.tuner.rm.collator import PairwiseDataCollatorWithPadding
 from llmtuner.tuner.rm.trainer import PairwisePeftTrainer
@@ -25,34 +25,24 @@
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="rm")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="rm")
     data_collator = PairwiseDataCollatorWithPadding(tokenizer)
 
     training_args.remove_unused_columns = False # important for pairwise dataset
 
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
     trainer = PairwisePeftTrainer(
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

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.1.2/src/llmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.1.2/src/llmtuner/tuner/sft/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,39 +32,52 @@
         Subclass and override to inject custom behavior.
         """
         prompt_len, label_len = inputs["input_ids"].size(-1), inputs["labels"].size(-1)
         if prompt_len > label_len:
             inputs["labels"] = self._pad_tensors_to_target_len(inputs["labels"], inputs["input_ids"])
         if label_len > prompt_len:
             inputs["input_ids"] = self._pad_tensors_to_target_len(inputs["input_ids"], inputs["labels"])
+            if "attention_mask" in inputs:
+                inputs["attention_mask"] = self._pad_tensors_to_target_len(
+                    inputs["attention_mask"], inputs["labels"], pad_token_id=0
+                )
+            if "position_ids" in inputs:
+                inputs["position_ids"] = self._pad_tensors_to_target_len(
+                    inputs["position_ids"], inputs["labels"], pad_token_id=0
+                )
 
         loss, generated_tokens, labels = super().prediction_step(
             model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
         )
-        generated_tokens = generated_tokens[:, max(prompt_len, label_len):] if generated_tokens is not None else None
+        generated_tokens = (
+            generated_tokens[:, max(prompt_len, label_len):] if generated_tokens is not None else None
+        )
 
         return (loss, generated_tokens, labels)
 
-    def _pad_tensors_to_target_len(self, src_tensor: torch.Tensor, tgt_tensor: torch.Tensor) -> torch.Tensor:
+    def _pad_tensors_to_target_len(
+        self,
+        src_tensor: torch.Tensor,
+        tgt_tensor: torch.Tensor,
+        pad_token_id: Optional[int] = None
+    ) -> torch.Tensor:
         r"""
         Pads the tensor to the same length as the target tensor.
 
         Should only be called when predict_with_generate=True.
         """
-        if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
-            assert self.tokenizer.padding_side == "left", "This method only accepts left-padded tensor."
-            # If PAD token is not defined at least EOS token has to be defined
-            pad_token_id = (
-                self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
-            )
-        else:
-            if self.model.config.pad_token_id is not None:
-                pad_token_id = self.model.config.pad_token_id
+        if pad_token_id is None:
+            if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
+                assert self.tokenizer.padding_side == "left", "This method only accepts left-padded tensor."
+                pad_token_id = self.tokenizer.pad_token_id
             else:
-                raise ValueError("Pad_token_id must be set in the configuration of the model, in order to pad tensors")
+                if self.model.config.pad_token_id is not None:
+                    pad_token_id = self.model.config.pad_token_id
+                else:
+                    raise ValueError("Pad_token_id must be set in the configuration of the model.")
 
         padded_tensor = pad_token_id * torch.ones_like(tgt_tensor)
         padded_tensor[:, -src_tensor.shape[-1]:] = src_tensor # adopt left-padding
         return padded_tensor
 
     def save_predictions(
         self,
```

### Comparing `llmtuner-0.1.1/src/llmtuner/tuner/sft/workflow.py` & `llmtuner-0.1.2/src/llmtuner/tuner/sft/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Inspired by: https://github.com/huggingface/transformers/blob/v4.29.2/examples/pytorch/summarization/run_summarization.py
 
 from typing import Optional, List
 from transformers import Seq2SeqTrainingArguments, DataCollatorForSeq2Seq, TrainerCallback
 
-from llmtuner.dsets import get_dataset, preprocess_dataset
+from llmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.constants import IGNORE_INDEX
 from llmtuner.extras.misc import get_logits_processor
 from llmtuner.extras.ploting import plot_loss
 from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.sft.metric import ComputeMetrics
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
     trainer = Seq2SeqPeftTrainer(
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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/chat.py` & `llmtuner-0.1.2/src/llmtuner/webui/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,20 +69,21 @@
         yield ALERTS["info_unloaded"][lang]
 
     def predict(
         self,
         chatbot: List[Tuple[str, str]],
         query: str,
         history: List[Tuple[str, str]],
+        prefix: str,
         max_new_tokens: int,
         top_p: float,
         temperature: float
     ):
         chatbot.append([query, ""])
         response = ""
         for new_text in self.stream_chat(
-            query, history, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
+            query, history, prefix, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
         ):
             response += new_text
             new_history = history + [(query, response)]
             chatbot[-1] = [query, response]
             yield chatbot, new_history
```

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/common.py` & `llmtuner-0.1.2/src/llmtuner/webui/common.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/chatbot.py`

 * *Files 10% similar despite different names*

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
+                prefix = gr.Textbox(show_label=False)
+                query = gr.Textbox(show_label=False, lines=8)
+                submit_btn = gr.Button(variant="primary")
 
             with gr.Column(scale=1):
                 clear_btn = gr.Button()
                 max_new_tokens = gr.Slider(
                     10, 2048, value=chat_model.generating_args.max_new_tokens, step=1, interactive=True
                 )
                 top_p = gr.Slider(0.01, 1, value=chat_model.generating_args.top_p, step=0.01, interactive=True)
@@ -32,24 +30,25 @@
                     0.01, 1.5, value=chat_model.generating_args.temperature, step=0.01, interactive=True
                 )
 
     history = gr.State([])
 
     submit_btn.click(
         chat_model.predict,
-        [chatbot, query, history, max_new_tokens, top_p, temperature],
+        [chatbot, query, history, prefix, max_new_tokens, top_p, temperature],
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
         max_new_tokens=max_new_tokens,
         top_p=top_p,
         temperature=temperature
     )
```

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/data.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/eval.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/eval.py`

 * *Files 1% similar despite different names*

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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/infer.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/infer.py`

 * *Files 4% similar despite different names*

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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/sft.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/sft.py`

 * *Files 19% similar despite different names*

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
@@ -70,18 +81,23 @@
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
@@ -99,17 +115,24 @@
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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/components/top.py` & `llmtuner-0.1.2/src/llmtuner/webui/components/top.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,19 @@
         model_path = gr.Textbox(scale=3)
 
     with gr.Row():
         finetuning_type = gr.Dropdown(value="lora", choices=METHODS, scale=1)
         checkpoints = gr.Dropdown(multiselect=True, scale=5)
         refresh_btn = gr.Button(scale=1)
 
-    with gr.Row():
-        quantization_bit = gr.Dropdown([8, 4], scale=1)
-        template = gr.Dropdown(value="default", choices=list(templates.keys()), scale=2)
-        source_prefix = gr.Textbox(scale=4)
+    with gr.Accordion(label="Advanced config", open=False) as advanced_tab:
+        with gr.Row():
+            quantization_bit = gr.Dropdown([8, 4], scale=1)
+            template = gr.Dropdown(value="default", choices=list(templates.keys()), scale=1)
+            source_prefix = gr.Textbox(scale=2)
 
     model_name.change(
         list_checkpoint, [model_name, finetuning_type], [checkpoints]
     ).then(
         get_model_path, [model_name], [model_path]
     ) # do not save config since the below line will save
     model_path.change(save_config, [model_name, model_path])
@@ -43,13 +44,14 @@
     refresh_btn.click(list_checkpoint, [model_name, finetuning_type], [checkpoints])
 
     return dict(
         lang=lang,
         model_name=model_name,
         model_path=model_path,
         finetuning_type=finetuning_type,
-        template=template,
         checkpoints=checkpoints,
         refresh_btn=refresh_btn,
+        advanced_tab=advanced_tab,
         quantization_bit=quantization_bit,
+        template=template,
         source_prefix=source_prefix
     )
```

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/interface.py` & `llmtuner-0.1.2/src/llmtuner/webui/interface.py`

 * *Files 14% similar despite different names*

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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/locales.py` & `llmtuner-0.1.2/src/llmtuner/webui/locales.py`

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

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/manager.py` & `llmtuner-0.1.2/src/llmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/runner.py` & `llmtuner-0.1.2/src/llmtuner/webui/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import threading
 import time
 import transformers
 from typing import List, Optional, Tuple
 
 from llmtuner.extras.callbacks import LogCallback
-from llmtuner.extras.constants import DEFAULT_MODULE # will be deprecated
+from llmtuner.extras.constants import DEFAULT_MODULE
 from llmtuner.extras.logging import LoggerHandler
 from llmtuner.extras.misc import torch_gc
 from llmtuner.tuner import get_train_args, run_sft
 from llmtuner.webui.common import get_model_path, get_save_dir
 from llmtuner.webui.locales import ALERTS
 from llmtuner.webui.utils import format_info, get_eval_results
 
@@ -73,18 +73,23 @@
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
 
@@ -95,15 +100,14 @@
         else:
             checkpoint_dir = None
 
         args = dict(
             model_name_or_path=model_name_or_path,
             do_train=True,
             overwrite_cache=True,
-            lora_target=DEFAULT_MODULE.get(model_name.split("-")[0], None) or "q_proj,v_proj",
             checkpoint_dir=checkpoint_dir,
             finetuning_type=finetuning_type,
             quantization_bit=int(quantization_bit) if quantization_bit else None,
             prompt_template=template,
             source_prefix=source_prefix,
             dataset_dir=dataset_dir,
             dataset=",".join(dataset),
@@ -111,17 +115,23 @@
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
+            lora_target=lora_target or DEFAULT_MODULE.get(model_name.split("-")[0], "q_proj,v_proj"),
             output_dir=os.path.join(get_save_dir(model_name), finetuning_type, output_dir)
         )
 
         if dev_ratio > 1e-6:
             args["dev_ratio"] = dev_ratio
             args["evaluation_strategy"] = "steps"
             args["eval_steps"] = save_steps
```

### Comparing `llmtuner-0.1.1/src/llmtuner/webui/utils.py` & `llmtuner-0.1.2/src/llmtuner/webui/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.1/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.1.2/src/llmtuner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -30,37 +30,40 @@
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 ## Changelog
 
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
 [23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
-[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [HuggingFace Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
+[23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
-[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model. If you want to train with RTX3090, use `git checkout baichuan-7b-rtx3090` to switch to the `baichuan-7b-rtx3090` branch and try the `--baichuan_rtx_gpu true` argument. (Other RTX series GPUs can also be tried)
+[23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
 [23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
+- [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
 - [BLOOM](https://huggingface.co/bigscience/bloom) & [BLOOMZ](https://huggingface.co/bigscience/bloomz) (560M/1.1B/1.7B/3B/7.1B/176B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B/40B)
 - [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Supported Training Approaches
 
@@ -77,44 +80,44 @@
 - [RLHF](https://arxiv.org/abs/2203.02155)
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
-  - [Wiki Demo](data/wiki_demo.txt)
+  - [Wiki Demo (en)](data/wiki_demo.txt)
 - For supervised fine-tuning:
-  - [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
-  - [Stanford Alpaca (Chinese)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [BELLE 2M](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
-  - [BELLE 1M](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
-  - [BELLE 0.5M](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
-  - [BELLE Dialogue 0.4M](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
-  - [BELLE School Math 0.25M](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
-  - [BELLE Multiturn Chat 0.8M](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
-  - [Guanaco Dataset](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
-  - [Firefly 1.1M](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
-  - [CodeAlpaca 20k](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
-  - [Alpaca CoT](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
-  - [Web QA (Chinese)](https://huggingface.co/datasets/suolyer/webqa)
-  - [UltraChat](https://github.com/thunlp/UltraChat)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [WebNovel (Chinese)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
-- For reward model training:
-  - [HH-RLHF](https://huggingface.co/datasets/Anthropic/hh-rlhf)
-  - [Open Assistant](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [Open Assistant (Chinese)](https://huggingface.co/datasets/OpenAssistant/oasst1)
-  - [GPT-4 Generated Data](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
-  - [GPT-4 Generated Data (Chinese)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
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
 
 ## Requirement
@@ -280,69 +283,93 @@
 
 </details>
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage pt \
+    --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
-    --max_samples 50 \
+    --max_samples 100 \
     --predict_with_generate
 ```
 
 We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit evaluation.
 
+### Predict
+
+```bash
+CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
+    --stage sft \
+    --model_name_or_path path_to_your_model \
+    --do_predict \
+    --dataset alpaca_gpt4_en \
+    --finetuning_type lora \
+    --checkpoint_dir path_to_checkpoint \
+    --output_dir path_to_predict_result \
+    --per_device_eval_batch_size 8 \
+    --max_samples 100 \
+    --predict_with_generate
+```
+
+If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
+
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
-See `http://localhost:8000/docs` for API documentation.
+Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
+- [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
 - [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
```

### Comparing `llmtuner-0.1.1/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.1.2/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 src/llmtuner.egg-info/top_level.txt
 src/llmtuner/api/__init__.py
 src/llmtuner/api/app.py
 src/llmtuner/api/protocol.py
 src/llmtuner/chat/__init__.py
 src/llmtuner/chat/stream_chat.py
 src/llmtuner/dsets/__init__.py
-src/llmtuner/dsets/callbacks.py
 src/llmtuner/dsets/loader.py
 src/llmtuner/dsets/preprocess.py
+src/llmtuner/dsets/utils.py
 src/llmtuner/extras/__init__.py
 src/llmtuner/extras/callbacks.py
 src/llmtuner/extras/constants.py
 src/llmtuner/extras/logging.py
 src/llmtuner/extras/misc.py
 src/llmtuner/extras/ploting.py
 src/llmtuner/extras/save_and_load.py
```

