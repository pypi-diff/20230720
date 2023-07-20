# Comparing `tmp/alphawave-0.3.92.tar.gz` & `tmp/alphawave-0.3.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.92.tar", last modified: Tue Jul 18 17:40:56 2023, max compression
+gzip compressed data, was "alphawave-0.3.93.tar", last modified: Thu Jul 20 19:06:00 2023, max compression
```

## Comparing `alphawave-0.3.92.tar` & `alphawave-0.3.93.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.085750 alphawave-0.3.92/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.92/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-18 17:40:56.085750 alphawave-0.3.92/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.92/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1022 2023-07-18 17:37:47.000000 alphawave-0.3.92/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-18 17:40:56.085750 alphawave-0.3.92/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.077750 alphawave-0.3.92/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.081750 alphawave-0.3.92/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9961 2023-07-18 17:07:38.000000 alphawave-0.3.92/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.92/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.92/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.92/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.92/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.92/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.92/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.92/src/alphawave/PythonResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.92/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.92/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6969 2023-07-18 17:07:21.000000 alphawave-0.3.92/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.92/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.92/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.92/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.92/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.92/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.92/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.081750 alphawave-0.3.92/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-18 17:40:56.000000 alphawave-0.3.92/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-18 17:40:56.000000 alphawave-0.3.92/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-18 17:40:56.000000 alphawave-0.3.92/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-18 17:40:56.000000 alphawave-0.3.92/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-18 17:40:56.000000 alphawave-0.3.92/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.081750 alphawave-0.3.92/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17679 2023-07-12 20:04:10.000000 alphawave-0.3.92/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.92/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7018 2023-07-16 16:56:57.000000 alphawave-0.3.92/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-07-12 19:12:18.000000 alphawave-0.3.92/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.92/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.92/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1423 2023-07-12 19:12:30.000000 alphawave-0.3.92/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1518 2023-07-12 19:12:07.000000 alphawave-0.3.92/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.92/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7938 2023-07-12 19:12:49.000000 alphawave-0.3.92/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.92/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.92/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.92/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.92/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.085750 alphawave-0.3.92/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.92/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.92/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2858 2023-07-12 19:14:52.000000 alphawave-0.3.92/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.92/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.92/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.92/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.92/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.085750 alphawave-0.3.92/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.92/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-12 19:15:47.000000 alphawave-0.3.92/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.92/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.92/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8718 2023-07-18 17:08:04.000000 alphawave-0.3.92/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-18 17:40:56.085750 alphawave-0.3.92/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.92/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.92/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.686530 alphawave-0.3.93/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.93/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-20 19:06:00.686530 alphawave-0.3.93/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.93/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1022 2023-07-20 19:05:50.000000 alphawave-0.3.93/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-20 19:06:00.686530 alphawave-0.3.93/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.678530 alphawave-0.3.93/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.682530 alphawave-0.3.93/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9961 2023-07-18 17:07:38.000000 alphawave-0.3.93/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.93/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.93/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.93/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.93/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.93/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.93/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.93/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.93/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.93/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6969 2023-07-18 17:07:21.000000 alphawave-0.3.93/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.93/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.93/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.93/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.93/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.93/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.93/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.682530 alphawave-0.3.93/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-20 19:06:00.000000 alphawave-0.3.93/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-20 19:06:00.000000 alphawave-0.3.93/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-20 19:06:00.000000 alphawave-0.3.93/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-20 19:06:00.000000 alphawave-0.3.93/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-20 19:06:00.000000 alphawave-0.3.93/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.682530 alphawave-0.3.93/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17679 2023-07-12 20:04:10.000000 alphawave-0.3.93/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.93/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7018 2023-07-16 16:56:57.000000 alphawave-0.3.93/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-07-12 19:12:18.000000 alphawave-0.3.93/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.93/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.93/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1423 2023-07-12 19:12:30.000000 alphawave-0.3.93/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1518 2023-07-12 19:12:07.000000 alphawave-0.3.93/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.93/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7938 2023-07-12 19:12:49.000000 alphawave-0.3.93/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.93/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.93/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.93/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.93/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.682530 alphawave-0.3.93/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.93/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6409 2023-07-19 16:46:22.000000 alphawave-0.3.93/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2858 2023-07-12 19:14:52.000000 alphawave-0.3.93/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.93/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.93/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    25504 2023-07-20 19:04:26.000000 alphawave-0.3.93/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.93/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.686530 alphawave-0.3.93/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.93/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-12 19:15:47.000000 alphawave-0.3.93/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.93/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.93/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8718 2023-07-18 17:08:04.000000 alphawave-0.3.93/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-20 19:06:00.686530 alphawave-0.3.93/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.93/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.93/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.92/LICENSE` & `alphawave-0.3.93/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/PKG-INFO` & `alphawave-0.3.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.92
+Version: 0.3.93
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.92/README.md` & `alphawave-0.3.93/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/pyproject.toml` & `alphawave-0.3.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.92"
+version = "0.3.93"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.92/src/alphawave/AlphaWave.py` & `alphawave-0.3.93/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/Colorize.py` & `alphawave-0.3.93/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.93/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.93/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/MemoryFork.py` & `alphawave-0.3.93/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/OSClient.py` & `alphawave-0.3.93/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/OpenAIClient.py` & `alphawave-0.3.93/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/PythonResponseValidator.py` & `alphawave-0.3.93/src/alphawave/PythonResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/RepairTestClient.py` & `alphawave-0.3.93/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/Response.py` & `alphawave-0.3.93/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.93/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/TestClient.py` & `alphawave-0.3.93/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/TestClientTest.py` & `alphawave-0.3.93/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.93/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/internalTypes.py` & `alphawave-0.3.93/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave/jsonParser.py` & `alphawave-0.3.93/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.93/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.92
+Version: 0.3.93
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.92/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.93/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/Agent.py` & `alphawave-0.3.93/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.93/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.93/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.93/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.93/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.93/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.93/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.93/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.93/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.93/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.93/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.93/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.93/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.93/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.93/src/alphawave_pyexts/LLMClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,19 @@
             elif role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
                 role_index = 0
                 conv.append_message(conv.roles[role_index], msg['content'])
             else:
                 role_index = 1
                 conv.append_message(conv.roles[role_index], msg['content'])
                 #print(conv.messages[-1])
-        #priming prompt - removed, user will add?
-        #conv.append_message(conv.roles[1], '')
+
+        # priming prompt
+        if conv.response_prime:
+            conv.append_message(conv.roles[1], '')
+
         prompt = conv.get_prompt()
         if len(prime) > 0:
             prompt = prime+conv.sep+prompt
     else:
         prompt = messages
     prompt = re.sub('\n{3,}', '\n\n', prompt)
     #print(f'***** llm output prompt string {prompt}')
```

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.93/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/chat.py` & `alphawave-0.3.93/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.93/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.93/src/alphawave_pyexts/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,53 @@
     sep2: str = None
     # Stop criteria (the default one is EOS token)
     stop_str: str = None
     # Stops generation if meeting any token in this list
     stop_token_ids: List[int] = None
     # prepends first msg text to front of prompt
     first_msg_no_role:bool = False
+    # response_prime - should we end with 'Assistant'?
+    response_prime:bool = False
 
+
+    
+
+    def get_llama_2_prompt(self):
+        B_INST, E_INST = "[INST]", "[/INST]"
+        B_SYS, E_SYS = "<<SYS>>\n", "\n<</SYS>>\n\n"
+        DEFAULT_SYSTEM_PROMPT = """You are a helpful, respectful and honest assistant. 
+If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, say so."""
+        
+        messages = self.messages
+        #print(f'Input: {messages}')
+        if messages[0][0] != "system":
+            messages = [("system", '')] + messages
+        messages = [[messages[1][0],B_SYS + messages[0][1] + E_SYS + messages[1][1]]] + messages[2:]
+        #print(f'\nInitial rewrite: {messages}')
+        ret: str = \
+            ''.join([
+                f"{B_INST} {(prompt[1]).strip()} {E_INST} {(answer[1]).strip()} "
+                for prompt, answer in zip(
+                        messages[::2],
+                        messages[1::2],
+                )
+            ])
+        #print(f'ret: {ret}')
+        assert (messages[-1][0] == "user"), f"Last message must be from user, got {ret[-1][0]}"
+        ret_suffix =  f"{B_INST} {(messages[-1][1]).strip()} {E_INST}"
+        #print(f'ret_suffix: {ret_suffix}')
+        ret=ret+ret_suffix
+        #print(f'Final ret: {ret}')
+        return ret
+
+        
     def get_prompt(self, include_system=False) -> str:
         """Get the prompt for generation."""
+        if self.name == 'llama-2':
+            return self.get_llama_2_prompt()
         if self.sep_style == SeparatorStyle.SINGLE:
             ret = ''
             if len(self.system) > 0 and include_system:
                 ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + "<s>" + message + "</s>\n"
@@ -205,14 +241,15 @@
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
             stop_str=self.stop_str,
             stop_token_ids=self.stop_token_ids,
             first_msg_no_role=self.first_msg_no_role,
+            response_prime = self.response_prime,
         )
 
     def dict(self):
         return {
             "template_name": self.name,
             "system": self.system,
             "roles": self.roles,
@@ -292,14 +329,15 @@
         system="",
         roles=("USER", "ASSISTANT"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep=" ",
         sep2="</s>",
+        response_prime=True,
     )
 )
 
 # Koala default template
 register_conv_template(
     Conversation(
         name="koala_v1",
@@ -319,18 +357,19 @@
         name="alpaca",
         system="",
         roles=("### Instruction", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n\n",
+        response_prime=True,
     )
 )
 
-# OpenLLama default template (copy of alpaca_
+# OpenLLama default template (copy of alpaca)
 register_conv_template(
     Conversation(
         name="openllama",
         system="",
         roles=("### Instruction", "### Response"),
         messages=(),
         offset=0,
@@ -373,14 +412,15 @@
         name="oasst_pythia",
         system="",
         roles=("<|prompter|>", "<|assistant|>"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.NO_COLON_SINGLE,
         sep="<|endoftext|>",
+        response_prime=True,
     )
 )
 
 # StableLM Alpha default template
 register_conv_template(
     Conversation(
         name="stablelm",
@@ -466,14 +506,27 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.NO_COLON_SINGLE,
         sep=None,
     )
 )
 
+# Llama-2 default template
+register_conv_template(
+    Conversation(
+        name="llama-2",
+        system="",
+        roles=("user", "assistant", "system"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.NO_COLON_SINGLE,
+        sep=None,
+    )
+)
+
 # Claude default template
 register_conv_template(
     Conversation(
         name="claude",
         system="",
         roles=("Human", "Assistant"),
         messages=(),
@@ -491,28 +544,30 @@
         roles=("<|im_start|>user", "<|im_start|>assistant", "<|im_start|>system"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
         sep="<|im_end|>",
         sep2='',
         stop_token_ids=[50278, 0],
+        response_prime=True,
     )
 )
 # MPT instruct template as per HG MPT 30b instruct model page
 register_conv_template(
     Conversation(
         name="mpt_instruct",
         system="",
         roles=("### Instruction", "### Response",""),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
         sep="\n",
         sep2='',
         stop_token_ids=[50278, 0],
+        response_prime=True,
     )
 )
 
 # Bard default template
 # Reference: https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L150
 #            https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L40
 register_conv_template(
@@ -634,14 +689,15 @@
             6,
             7,
             8,
             9,
             10,
             11,
         ],  # it better only put special tokens here, because tokenizer only remove special tokens
+        response_prime=True,
     )
 )
 
 register_conv_template(
     Conversation(
         name="falcon_instruct",
         system="",
@@ -650,14 +706,15 @@
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         stop_str=["User:", "Assistant:"],
         stop_token_ids=[11],
         sep="\n",
         sep2="<|endoftext|>",
         first_msg_no_role=False,
+        response_prime=True,
     )
 )
 register_conv_template(
     Conversation(
         name="falcon_GPTQ",
         system="",
         roles=("### Human", "### Assistant"),
@@ -676,58 +733,63 @@
         system="",
         roles=("Question", "Answer", ""), # third entry is system prefix. if absent defaults to user prefix.
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="",
+        response_prime=True,
     )
 )
 register_conv_template(Conversation(
         name="guanaco",
         system="",
         roles=("### Human", "### Assistant"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="",
+        response_prime=True,
     )
 )
 register_conv_template(Conversation(
         name="wizardLM2",
         system="",
         roles=("### Input", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="\n",
+        response_prime=True,
     )
 )
 register_conv_template(Conversation(
         name="wizardCoder",
         system="Below is an instruction that describes a task. Write a response that appropriately completes the request",
         roles=("### Instruction", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="<|end|>",
+        response_prime=True,
     )
 )
 register_conv_template(Conversation(
         name="wizardLM",
         system="",
         roles=("USER", "ASSISTANT"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="\n",
+        response_prime=True,
     )
 )
 
 # ChagGPT default template
 register_conv_template(
     Conversation(
         name="polyglot_changgpt",
@@ -746,14 +808,15 @@
         name="pygmalion",
         system="",
         roles=("You", "Samanath"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n",
+        response_prime=True,
     )
 )
 
 # tigerbot template
 register_conv_template(
     Conversation(
         name="tigerbot",
@@ -778,13 +841,13 @@
         sep="\n\n",
         stop_str="###",
     )
 )
 
 
 if __name__ == "__main__":
-    conv = get_conv_template("vicuna_v1.1")
-    conv.append_message(conv.roles[0], "Hello!")
-    conv.append_message(conv.roles[1], "Hi!")
-    conv.append_message(conv.roles[0], "How are you?")
-    conv.append_message(conv.roles[1], None)
+    conv = get_conv_template("llama-2")
+    conv.append_message('system', "You are a friendly AI")
+    conv.append_message(conv.roles[0], "Hi!")
+    conv.append_message(conv.roles[1], "How are you?")
+    conv.append_message(conv.roles[0], "What is your name")
     print(conv.get_prompt())
```

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/handler.py` & `alphawave-0.3.93/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.93/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.93/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.93/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.93/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.93/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/tests/testOSClient.py` & `alphawave-0.3.93/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.92/tests/testOpenAiClient.py` & `alphawave-0.3.93/tests/testOpenAiClient.py`

 * *Files identical despite different names*

