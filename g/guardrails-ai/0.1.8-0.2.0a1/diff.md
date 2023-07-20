# Comparing `tmp/guardrails-ai-0.1.8.tar.gz` & `tmp/guardrails-ai-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-ai-0.1.8.tar", last modified: Wed Jun 14 10:50:01 2023, max compression
+gzip compressed data, was "guardrails-ai-0.2.0a1.tar", last modified: Thu Jul 20 19:29:11 2023, max compression
```

## Comparing `guardrails-ai-0.1.8.tar` & `guardrails-ai-0.2.0a1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.662508 guardrails-ai-0.1.8/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    11357 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/LICENSE
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      165 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/MANIFEST.in
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-06-14 10:50:01.662299 guardrails-ai-0.1.8/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7902 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/README.md
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.657662 guardrails-ai-0.1.8/guardrails/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      629 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/__init__.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.658060 guardrails-ai-0.1.8/guardrails/applications/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/applications/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6588 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/applications/text2sql.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      778 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/applications/text2sql.rail
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1613 2023-05-19 21:55:45.000000 guardrails-ai-0.1.8/guardrails/cli.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4966 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/constants.xml
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    16754 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/datatypes.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7352 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/document_store.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6331 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/embedding.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7502 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/guard.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     5592 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/llm_providers.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      295 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/logging_utils.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.658547 guardrails-ai-0.1.8/guardrails/prompt/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      115 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/prompt/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3260 2023-06-06 19:33:09.000000 guardrails-ai-0.1.8/guardrails/prompt/base_prompt.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1279 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/prompt/instructions.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      796 2023-05-09 03:35:20.000000 guardrails-ai-0.1.8/guardrails/prompt/prompt.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8741 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/rail.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    11536 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/run.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    28902 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/schema.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.660814 guardrails-ai-0.1.8/guardrails/utils/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/utils/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1555 2023-06-08 19:52:05.000000 guardrails-ai-0.1.8/guardrails/utils/constants.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2530 2023-04-27 15:53:00.000000 guardrails-ai-0.1.8/guardrails/utils/docs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6217 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/logs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2567 2023-06-14 07:06:12.000000 guardrails-ai-0.1.8/guardrails/utils/misc.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    16550 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/pydantic_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7050 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/reask_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4018 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/sql_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    48218 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/validators.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.661307 guardrails-ai-0.1.8/guardrails/vectordb/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       93 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/vectordb/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2956 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/vectordb/base.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3244 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/vectordb/faiss.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       22 2023-06-14 10:49:41.000000 guardrails-ai-0.1.8/guardrails/version.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.662033 guardrails-ai-0.1.8/guardrails_ai.egg-info/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1153 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/SOURCES.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        1 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/dependency_links.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       50 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/entry_points.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      557 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/requires.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       11 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/top_level.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       38 2023-06-14 10:50:01.662554 guardrails-ai-0.1.8/setup.cfg
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4722 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/setup.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.191104 guardrails-ai-0.2.0a1/
+-rw-r--r--   0 rafael     (501) staff       (20)    11357 2023-03-14 22:38:38.000000 guardrails-ai-0.2.0a1/LICENSE
+-rw-r--r--   0 rafael     (501) staff       (20)      165 2023-03-14 22:38:38.000000 guardrails-ai-0.2.0a1/MANIFEST.in
+-rw-r--r--   0 rafael     (501) staff       (20)     8609 2023-07-20 19:29:11.190660 guardrails-ai-0.2.0a1/PKG-INFO
+-rw-r--r--   0 rafael     (501) staff       (20)     7902 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/README.md
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.178790 guardrails-ai-0.2.0a1/guardrails/
+-rw-r--r--   0 rafael     (501) staff       (20)      629 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/__init__.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.180064 guardrails-ai-0.2.0a1/guardrails/applications/
+-rw-r--r--   0 rafael     (501) staff       (20)        0 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/applications/__init__.py
+-rw-r--r--   0 rafael     (501) staff       (20)     6588 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/applications/text2sql.py
+-rw-r--r--   0 rafael     (501) staff       (20)      778 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/applications/text2sql.rail
+-rw-r--r--   0 rafael     (501) staff       (20)     1613 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/cli.py
+-rw-r--r--   0 rafael     (501) staff       (20)     5217 2023-07-11 21:40:58.000000 guardrails-ai-0.2.0a1/guardrails/constants.xml
+-rw-r--r--   0 rafael     (501) staff       (20)    19083 2023-07-20 19:23:37.000000 guardrails-ai-0.2.0a1/guardrails/datatypes.py
+-rw-r--r--   0 rafael     (501) staff       (20)     7352 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/document_store.py
+-rw-r--r--   0 rafael     (501) staff       (20)     6331 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/embedding.py
+-rw-r--r--   0 rafael     (501) staff       (20)    12686 2023-07-19 21:39:49.000000 guardrails-ai-0.2.0a1/guardrails/guard.py
+-rw-r--r--   0 rafael     (501) staff       (20)     9219 2023-07-11 21:40:58.000000 guardrails-ai-0.2.0a1/guardrails/llm_providers.py
+-rw-r--r--   0 rafael     (501) staff       (20)      295 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/logging_utils.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.181632 guardrails-ai-0.2.0a1/guardrails/prompt/
+-rw-r--r--   0 rafael     (501) staff       (20)      115 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/prompt/__init__.py
+-rw-r--r--   0 rafael     (501) staff       (20)     3260 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/prompt/base_prompt.py
+-rw-r--r--   0 rafael     (501) staff       (20)     1279 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/prompt/instructions.py
+-rw-r--r--   0 rafael     (501) staff       (20)      796 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/prompt/prompt.py
+-rw-r--r--   0 rafael     (501) staff       (20)     8910 2023-07-11 21:40:58.000000 guardrails-ai-0.2.0a1/guardrails/rail.py
+-rw-r--r--   0 rafael     (501) staff       (20)    16426 2023-07-19 21:39:49.000000 guardrails-ai-0.2.0a1/guardrails/run.py
+-rw-r--r--   0 rafael     (501) staff       (20)    30231 2023-07-20 19:23:37.000000 guardrails-ai-0.2.0a1/guardrails/schema.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.186171 guardrails-ai-0.2.0a1/guardrails/utils/
+-rw-r--r--   0 rafael     (501) staff       (20)        0 2023-03-14 22:38:38.000000 guardrails-ai-0.2.0a1/guardrails/utils/__init__.py
+-rw-r--r--   0 rafael     (501) staff       (20)     1555 2023-06-20 13:22:53.000000 guardrails-ai-0.2.0a1/guardrails/utils/constants.py
+-rw-r--r--   0 rafael     (501) staff       (20)     2530 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/utils/docs_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)     8978 2023-07-18 22:50:54.000000 guardrails-ai-0.2.0a1/guardrails/utils/json_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)     6984 2023-07-20 19:23:37.000000 guardrails-ai-0.2.0a1/guardrails/utils/logs_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)     4865 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/utils/misc.py
+-rw-r--r--   0 rafael     (501) staff       (20)    16769 2023-07-18 18:03:31.000000 guardrails-ai-0.2.0a1/guardrails/utils/pydantic_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)     7173 2023-07-11 21:40:58.000000 guardrails-ai-0.2.0a1/guardrails/utils/reask_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)     4018 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/utils/sql_utils.py
+-rw-r--r--   0 rafael     (501) staff       (20)    49946 2023-07-20 19:23:37.000000 guardrails-ai-0.2.0a1/guardrails/validators.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.187912 guardrails-ai-0.2.0a1/guardrails/vectordb/
+-rw-r--r--   0 rafael     (501) staff       (20)       93 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/vectordb/__init__.py
+-rw-r--r--   0 rafael     (501) staff       (20)     2956 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/vectordb/base.py
+-rw-r--r--   0 rafael     (501) staff       (20)     3244 2023-06-27 15:46:15.000000 guardrails-ai-0.2.0a1/guardrails/vectordb/faiss.py
+-rw-r--r--   0 rafael     (501) staff       (20)       30 2023-07-20 19:25:21.000000 guardrails-ai-0.2.0a1/guardrails/version.py
+drwxr-xr-x   0 rafael     (501) staff       (20)        0 2023-07-20 19:29:11.190098 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/
+-rw-r--r--   0 rafael     (501) staff       (20)     8609 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/PKG-INFO
+-rw-r--r--   0 rafael     (501) staff       (20)     1184 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 rafael     (501) staff       (20)        1 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 rafael     (501) staff       (20)       50 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/entry_points.txt
+-rw-r--r--   0 rafael     (501) staff       (20)      580 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/requires.txt
+-rw-r--r--   0 rafael     (501) staff       (20)       11 2023-07-20 19:29:11.000000 guardrails-ai-0.2.0a1/guardrails_ai.egg-info/top_level.txt
+-rw-r--r--   0 rafael     (501) staff       (20)       38 2023-07-20 19:29:11.191181 guardrails-ai-0.2.0a1/setup.cfg
+-rw-r--r--   0 rafael     (501) staff       (20)     4756 2023-07-18 18:03:31.000000 guardrails-ai-0.2.0a1/setup.py
```

### Comparing `guardrails-ai-0.1.8/LICENSE` & `guardrails-ai-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/PKG-INFO` & `guardrails-ai-0.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.8
+Version: 0.2.0a1
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `guardrails-ai-0.1.8/README.md` & `guardrails-ai-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/__init__.py` & `guardrails-ai-0.2.0a1/guardrails/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/applications/text2sql.py` & `guardrails-ai-0.2.0a1/guardrails/applications/text2sql.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/applications/text2sql.rail` & `guardrails-ai-0.2.0a1/guardrails/applications/text2sql.rail`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/cli.py` & `guardrails-ai-0.2.0a1/guardrails/cli.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/constants.xml` & `guardrails-ai-0.2.0a1/guardrails/constants.xml`

 * *Files 12% similar despite different names*

#### Comparing `guardrails-ai-0.1.8/guardrails/constants.xml` & `guardrails-ai-0.2.0a1/guardrails/constants.xml`

```diff
@@ -5,14 +5,19 @@
   <json_suffix_prompt_v2>ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter &quot;None&quot;.</json_suffix_prompt_v2>
   <json_suffix_prompt_v2_wo_none>ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise.</json_suffix_prompt_v2_wo_none>
   <high_level_json_reask_prompt>I was given the following JSON response, which had problems due to incorrect values.
 
 {previous_response}
 
 Help me correct the incorrect values based on the given error messages.</high_level_json_reask_prompt>
+  <high_level_skeleton_reask_prompt>I was given the following JSON response, which had problems due to incorrect values.
+
+{previous_response}
+
+Help me correct the incorrect values based on the given error messages.</high_level_skeleton_reask_prompt>
   <complete_json_suffix>
     Given below is XML that describes the information to extract from this document and the tags to extract it into.
 
 {output_schema}
 
 ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `null`.
```

### Comparing `guardrails-ai-0.1.8/guardrails/datatypes.py` & `guardrails-ai-0.2.0a1/guardrails/datatypes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import datetime
+import logging
 from types import SimpleNamespace
 from typing import TYPE_CHECKING, Any, Dict, Generator
 from typing import List as TypedList
 from typing import Tuple, Type, Union
 
 from lxml import etree as ET
 from pydantic import BaseModel
 
+from guardrails.utils.logs_utils import FieldValidationLogs, ValidatorLogs
+
 if TYPE_CHECKING:
     from guardrails.schema import FormatAttr
 
+logger = logging.getLogger(__name__)
+
 
 class DataType:
     def __init__(
         self,
         children: Dict[str, Any],
         format_attr: "FormatAttr",
         element: ET._Element,
@@ -62,23 +67,53 @@
         """Create a DataType from a string.
 
         Note: ScalarTypes like int, float, bool, etc. will override this method.
         Other ScalarTypes like string, email, url, etc. will not override this
         """
         return s
 
-    def validate(self, key: str, value: Any, schema: Dict) -> Dict:
-        """Validate a value."""
-        value = self.from_str(value)
-
+    def _iterate_validators(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
         for validator in self.validators:
-            schema = validator.validate_with_correction(key, value, schema)
-
+            validator_class_name = validator.__class__.__name__
+            validator_logs = ValidatorLogs(
+                validator_name=validator_class_name,
+                value_before_validation=value,
+            )
+            validation_logs.validator_logs.append(validator_logs)
+            logger.debug(
+                f"Validating field {key} with validator {validator_class_name}..."
+            )
+            value = validator.validate_with_correction(value, metadata)
+            validator_logs.value_after_validation = value
+            logger.debug(
+                f"Validator {validator_class_name} finished, "
+                f"key {key} has value {value}."
+            )
+            schema[key] = value
         return schema
 
+    def validate(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
+        """Validate a value."""
+        value = self.from_str(value)
+        return self._iterate_validators(validation_logs, key, value, schema, metadata)
+
     def set_children(self, element: ET._Element):
         raise NotImplementedError("Abstract method.")
 
     @classmethod
     def from_xml(cls, element: ET._Element, strict: bool = False) -> "DataType":
         from guardrails.schema import FormatAttr
 
@@ -101,14 +136,15 @@
 registry: Dict[str, DataType] = {}
 
 
 # Create a decorator to register a type
 def register_type(name: str):
     def decorator(cls: type):
         registry[name] = cls
+        cls.rail_alias = name
         return cls
 
     return decorator
 
 
 class ScalarType(DataType):
     def set_children(self, element: ET._Element):
@@ -194,15 +230,15 @@
 
         return datetime.datetime.strptime(s, self.date_format).date()
 
     @classmethod
     def from_xml(cls, element: ET._Element, strict: bool = False) -> "DataType":
         datatype = super().from_xml(element, strict)
 
-        if "date-format" in element.attrib:
+        if "date-format" in element.attrib or "date_format" in element.attrib:
             datatype.date_format = element.attrib["date-format"]
 
         return datatype
 
 
 @register_type("time")
 class Time(ScalarType):
@@ -225,15 +261,15 @@
 
         return datetime.datetime.strptime(s, self.time_format).time()
 
     @classmethod
     def from_xml(cls, element: ET._Element, strict: bool = False) -> "DataType":
         datatype = super().from_xml(element, strict)
 
-        if "time-format" in element.attrib:
+        if "time-format" in element.attrib or "time_format" in element.attrib:
             datatype.date_format = element.attrib["time-format"]
 
         return datatype
 
 
 @register_type("email")
 class Email(ScalarType):
@@ -260,28 +296,36 @@
     """Element tag: `<percentage>`"""
 
 
 @register_type("list")
 class List(NonScalarType):
     """Element tag: `<list>`"""
 
-    def validate(self, key: str, value: Any, schema: Dict) -> Dict:
+    def validate(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
         # Validators in the main list data type are applied to the list overall.
 
-        for validator in self.validators:
-            schema = validator.validate_with_correction(key, value, schema)
+        self._iterate_validators(validation_logs, key, value, schema, metadata)
 
         if len(self._children) == 0:
             return schema
 
         item_type = list(self._children.values())[0]
 
         # TODO(shreya): Edge case: List of lists -- does this still work?
         for i, item in enumerate(value):
-            value = item_type.validate(i, item, value)
+            child_validation_logs = FieldValidationLogs()
+            validation_logs.children[i] = child_validation_logs
+            value = item_type.validate(child_validation_logs, i, item, value, metadata)
 
         return schema
 
     def set_children(self, element: ET._Element):
         for idx, child in enumerate(element, start=1):
             if idx > 1:
                 # Only one child is allowed in a list data type.
@@ -292,19 +336,25 @@
             self._children["item"] = child_data_type.from_xml(child)
 
 
 @register_type("object")
 class Object(NonScalarType):
     """Element tag: `<object>`"""
 
-    def validate(self, key: str, value: Any, schema: Dict) -> Dict:
+    def validate(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
         # Validators in the main object data type are applied to the object overall.
 
-        for validator in self.validators:
-            schema = validator.validate_with_correction(key, value, schema)
+        schema = self._iterate_validators(validation_logs, key, value, schema, metadata)
 
         if len(self._children) == 0:
             return schema
 
         # Types of supported children
         # 1. key_type
         # 2. value_type
@@ -313,16 +363,19 @@
         # TODO(shreya): Implement key type and value type later
 
         # Check for required keys
         for child_key, child_data_type in self._children.items():
             # Value should be a dictionary
             # child_key is an expected key that the schema defined
             # child_data_type is the data type of the expected key
+            child_value = value.get(child_key, None)
+            child_validation_logs = FieldValidationLogs()
+            validation_logs.children[child_key] = child_validation_logs
             value = child_data_type.validate(
-                child_key, value.get(child_key, None), value
+                child_validation_logs, child_key, child_value, value, metadata
             )
 
         schema[key] = value
 
         return schema
 
     def set_children(self, element: ET._Element):
@@ -336,23 +389,39 @@
     """Element tag: `<object>`"""
 
     def __init__(
         self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
     ) -> None:
         super().__init__(children, format_attr, element)
 
-    def validate(self, key: str, value: Any, schema: Dict) -> Dict:
+    def validate(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
+        # Until we refactor the discriminator into the choice object,
+        # we expose the schema to the choice validator via metadata
+        choice_metadata = {
+            **metadata,
+            "__schema": schema,
+        }
+
         # Call the validate method of the parent class
-        super().validate(key, value, schema)
+        super().validate(validation_logs, key, value, schema, choice_metadata)
 
         # Validate the selected choice
         selected_key = value
         selected_value = schema[selected_key]
 
-        self._children[selected_key].validate(selected_key, selected_value, schema)
+        self._children[selected_key].validate(
+            validation_logs, selected_key, selected_value, schema, metadata
+        )
 
         schema[key] = value
         return schema
 
     def set_children(self, element: ET._Element):
         for child in element:
             child_data_type = registry[child.tag]
@@ -377,17 +446,25 @@
     """Element tag: `<case>`"""
 
     def __init__(
         self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
     ) -> None:
         super().__init__(children, format_attr, element)
 
-    def validate(self, key: str, value: Any, schema: Dict) -> Dict:
+    def validate(
+        self,
+        validation_logs: FieldValidationLogs,
+        key: str,
+        value: Any,
+        schema: Dict,
+        metadata: Dict,
+    ) -> Dict:
         child = list(self._children.values())[0]
-        child.validate(key, value, schema)
+
+        child.validate(validation_logs, key, value, schema, metadata)
 
         schema[key] = value
 
         return schema
 
     def set_children(self, element: ET._Element):
         assert len(element) == 1, "Case must have exactly one child."
```

### Comparing `guardrails-ai-0.1.8/guardrails/document_store.py` & `guardrails-ai-0.2.0a1/guardrails/document_store.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/embedding.py` & `guardrails-ai-0.2.0a1/guardrails/embedding.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/guard.py` & `guardrails-ai-0.2.0a1/guardrails/guard.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import asyncio
 import logging
 from string import Formatter
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, Union
 
 from eliot import add_destinations, start_action
 from pydantic import BaseModel
 
-from guardrails.llm_providers import PromptCallable, get_llm_ask
+from guardrails.llm_providers import get_async_llm_ask, get_llm_ask
 from guardrails.prompt import Instructions, Prompt
 from guardrails.rail import Rail
-from guardrails.run import Runner
+from guardrails.run import AsyncRunner, Runner
 from guardrails.schema import Schema
 from guardrails.utils.logs_utils import GuardState
 from guardrails.utils.reask_utils import sub_reasks_with_fixed_values
 
 logger = logging.getLogger(__name__)
 actions_logger = logging.getLogger(f"{__name__}.actions")
 add_destinations(actions_logger.debug)
@@ -146,62 +147,172 @@
         rail = Rail.from_pydantic(
             output_class=output_class, prompt=prompt, instructions=instructions
         )
         return cls(rail, num_reasks=num_reasks, base_model=output_class)
 
     def __call__(
         self,
-        llm_api: Callable,
+        llm_api: Union[Callable, Callable[[Any], Awaitable[Any]]],
         prompt_params: Dict = None,
         num_reasks: Optional[int] = None,
+        metadata: Optional[Dict] = None,
         *args,
         **kwargs,
-    ) -> Tuple[str, Dict]:
-        """Call the LLM and validate the output.
+    ) -> Union[Tuple[str, Dict], Awaitable[Tuple[str, Dict]]]:
+        """Call the LLM and validate the output. Pass an async LLM API to
+        return a coroutine.
 
         Args:
-            llm_api: The LLM API to call (e.g. openai.Completion.create)
+            llm_api: The LLM API to call
+                     (e.g. openai.Completion.create or openai.Completion.acreate)
             prompt_params: The parameters to pass to the prompt.format() method.
             num_reasks: The max times to re-ask the LLM for invalid output.
 
         Returns:
             The raw text output from the LLM and the validated output.
         """
-
         if num_reasks is None:
             num_reasks = self.num_reasks
+        if metadata is None:
+            metadata = {}
 
+        # If the LLM API is async, return a coroutine
+        if asyncio.iscoroutinefunction(llm_api):
+            return self._call_async(
+                llm_api,
+                prompt_params=prompt_params,
+                num_reasks=num_reasks,
+                metadata=metadata,
+                *args,
+                **kwargs,
+            )
+        # Otherwise, call the LLM synchronously
+        return self._call_sync(
+            llm_api,
+            prompt_params=prompt_params,
+            num_reasks=num_reasks,
+            metadata=metadata,
+            *args,
+            **kwargs,
+        )
+
+    def _call_sync(
+        self,
+        llm_api: Callable,
+        prompt_params: Dict,
+        num_reasks: int,
+        metadata: Dict,
+        *args,
+        **kwargs,
+    ) -> Tuple[str, Dict]:
         with start_action(action_type="guard_call", prompt_params=prompt_params):
             if "instructions" in kwargs:
                 logger.info("Instructions overridden at call time")
                 # TODO(shreya): should we overwrite self.instructions for this run?
             runner = Runner(
                 instructions=kwargs.get("instructions", self.instructions),
                 prompt=self.prompt,
                 api=get_llm_ask(llm_api, *args, **kwargs),
                 input_schema=self.input_schema,
                 output_schema=self.output_schema,
                 num_reasks=num_reasks,
+                metadata=metadata,
                 reask_prompt=self.reask_prompt,
                 base_model=self.base_model,
+                guard_state=self.guard_state,
             )
             guard_history = runner(prompt_params=prompt_params)
-            self.guard_state = self.guard_state.push(guard_history)
+            return guard_history.output, guard_history.validated_output
+
+    async def _call_async(
+        self,
+        llm_api: Callable[[Any], Awaitable[Any]],
+        prompt_params: Dict,
+        num_reasks: int,
+        metadata: Dict,
+        *args,
+        **kwargs,
+    ) -> Tuple[str, Dict]:
+        """Call the LLM asynchronously and validate the output.
+
+        Args:
+            llm_api: The LLM API to call asynchronously (e.g. openai.Completion.acreate)
+            prompt_params: The parameters to pass to the prompt.format() method.
+            num_reasks: The max times to re-ask the LLM for invalid output.
+
+        Returns:
+            The raw text output from the LLM and the validated output.
+        """
+        with start_action(action_type="guard_call", prompt_params=prompt_params):
+            if "instructions" in kwargs:
+                logger.info("Instructions overridden at call time")
+                # TODO(shreya): should we overwrite self.instructions for this run?
+            runner = AsyncRunner(
+                instructions=kwargs.get("instructions", self.instructions),
+                prompt=self.prompt,
+                api=get_async_llm_ask(llm_api, *args, **kwargs),
+                input_schema=self.input_schema,
+                output_schema=self.output_schema,
+                num_reasks=num_reasks,
+                metadata=metadata,
+                reask_prompt=self.reask_prompt,
+                guard_state=self.guard_state,
+            )
+            guard_history = await runner.async_run(prompt_params=prompt_params)
             return guard_history.output, guard_history.validated_output
 
     def __repr__(self):
         return f"Guard(RAIL={self.rail})"
 
     def __rich_repr__(self):
         yield "RAIL", self.rail
 
     def parse(
         self,
         llm_output: str,
-        llm_api: PromptCallable = None,
+        llm_api: Union[Callable, Callable[[Any], Awaitable[Any]]] = None,
+        num_reasks: int = 1,
+        prompt_params: Dict = None,
+        *args,
+        **kwargs,
+    ) -> Union[Tuple[str, Dict], Awaitable[Tuple[str, Dict]]]:
+        """Alternate flow to using Guard where the llm_output is known.
+
+        Args:
+            llm_api: The LLM API to call
+                     (e.g. openai.Completion.create or openai.Completion.acreate)
+            num_reasks: The max times to re-ask the LLM for invalid output.
+
+        Returns:
+            The validated response.
+        """
+        # If the LLM API is async, return a coroutine
+        if asyncio.iscoroutinefunction(llm_api):
+            return self._async_parse(
+                llm_output,
+                llm_api=llm_api,
+                num_reasks=num_reasks,
+                prompt_params=prompt_params,
+                *args,
+                **kwargs,
+            )
+        # Otherwise, call the LLM synchronously
+        return self._sync_parse(
+            llm_output,
+            llm_api=llm_api,
+            num_reasks=num_reasks,
+            prompt_params=prompt_params,
+            *args,
+            **kwargs,
+        )
+
+    def _sync_parse(
+        self,
+        llm_output: str,
+        llm_api: Callable = None,
         num_reasks: int = 1,
         prompt_params: Dict = None,
         *args,
         **kwargs,
     ) -> Dict:
         """Alternate flow to using Guard where the llm_output is known.
 
@@ -219,11 +330,45 @@
                 prompt=None,
                 api=get_llm_ask(llm_api, *args, **kwargs) if llm_api else None,
                 input_schema=None,
                 output_schema=self.output_schema,
                 num_reasks=num_reasks,
                 output=llm_output,
                 reask_prompt=self.reask_prompt,
+                guard_state=self.guard_state,
             )
             guard_history = runner(prompt_params=prompt_params)
-            self.guard_state = self.guard_state.push(guard_history)
+            return sub_reasks_with_fixed_values(guard_history.validated_output)
+
+    async def _async_parse(
+        self,
+        llm_output: str,
+        llm_api: Callable[[Any], Awaitable[Any]] = None,
+        num_reasks: int = 1,
+        prompt_params: Dict = None,
+        *args,
+        **kwargs,
+    ) -> Dict:
+        """Alternate flow to using Guard where the llm_output is known.
+
+        Args:
+            llm_output: The output from the LLM.
+            llm_api: The LLM API to use to re-ask the LLM.
+            num_reasks: The max times to re-ask the LLM for invalid output.
+
+        Returns:
+            The validated response.
+        """
+        with start_action(action_type="guard_parse"):
+            runner = AsyncRunner(
+                instructions=None,
+                prompt=None,
+                api=get_async_llm_ask(llm_api, *args, **kwargs) if llm_api else None,
+                input_schema=None,
+                output_schema=self.output_schema,
+                num_reasks=num_reasks,
+                output=llm_output,
+                reask_prompt=self.reask_prompt,
+                guard_state=self.guard_state,
+            )
+            guard_history = await runner.async_run(prompt_params=prompt_params)
             return sub_reasks_with_fixed_values(guard_history.validated_output)
```

### Comparing `guardrails-ai-0.1.8/guardrails/prompt/base_prompt.py` & `guardrails-ai-0.2.0a1/guardrails/prompt/base_prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/prompt/instructions.py` & `guardrails-ai-0.2.0a1/guardrails/prompt/instructions.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/prompt/prompt.py` & `guardrails-ai-0.2.0a1/guardrails/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/rail.py` & `guardrails-ai-0.2.0a1/guardrails/rail.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         for expr in self.find_expressions(body):
             # The replacement should be inserted as a Python expression, inside
             # curly braces.
             replacement = self(expr)
             # If a string, wrap it in '' quotes.
             if isinstance(replacement, str):
                 replacement = f"'{replacement}'"
+            # Escape any double quotes.
+            replacement = str(replacement).replace('"', "&quot;")
+            # Replace the expression with the evaluated value.
             body = body.replace(f"{{{expr}}}", f"{{{replacement}}}")
 
         return body
 
     def __call__(self, expr: str):
         """Eval expression in the script's namespace."""
         return eval(expr, {**globals(), **self.variables})
```

### Comparing `guardrails-ai-0.1.8/guardrails/run.py` & `guardrails-ai-0.2.0a1/guardrails/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from eliot import add_destinations, start_action
 from pydantic import BaseModel
 
-from guardrails.llm_providers import PromptCallable
+from guardrails.llm_providers import AsyncPromptCallable, PromptCallable
 from guardrails.prompt import Instructions, Prompt
 from guardrails.schema import Schema
-from guardrails.utils.logs_utils import GuardHistory, GuardLogs
+from guardrails.utils.logs_utils import GuardHistory, GuardLogs, GuardState
 from guardrails.utils.reask_utils import (
+    FieldReAsk,
     ReAsk,
     prune_obj_for_reasking,
     reasks_to_dict,
     sub_reasks_with_fixed_values,
 )
 
 logger = logging.getLogger(__name__)
@@ -42,23 +43,26 @@
     """
 
     instructions: Optional[Instructions]
     prompt: Prompt
     api: PromptCallable
     input_schema: Schema
     output_schema: Schema
+    guard_state: GuardState
     num_reasks: int = 0
+    metadata: Dict[str, Any] = field(default_factory=dict)
     output: str = None
     reask_prompt: Optional[Prompt] = None
     guard_history: GuardHistory = field(default_factory=lambda: GuardHistory([]))
     base_model: Optional[BaseModel] = None
 
     def _reset_guard_history(self):
         """Reset the guard history."""
         self.guard_history = GuardHistory([])
+        self.guard_state.push(self.guard_history)
 
     def __post_init__(self):
         assert (self.prompt and self.api and not self.output) or (
             self.output and not self.prompt
         ), "Must provide either prompt and api or output."
 
     def __call__(self, prompt_params: Dict = None) -> GuardHistory:
@@ -78,14 +82,15 @@
             action_type="run",
             instructions=self.instructions,
             prompt=self.prompt,
             api=self.api,
             input_schema=self.input_schema,
             output_schema=self.output_schema,
             num_reasks=self.num_reasks,
+            metadata=self.metadata,
         ):
             instructions, prompt, input_schema, output_schema = (
                 self.instructions,
                 self.prompt,
                 self.input_schema,
                 self.output_schema,
             )
@@ -121,14 +126,17 @@
         instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
         input_schema: Schema,
         output_schema: Schema,
         output: str = None,
     ):
+        guard_logs = GuardLogs()
+        self.guard_history.push(guard_logs)
+
         """Run a full step."""
         with start_action(
             action_type="step",
             index=index,
             instructions=instructions,
             prompt=prompt,
             prompt_params=prompt_params,
@@ -146,49 +154,54 @@
                     input_schema,
                     output_schema,
                 )
             else:
                 instructions = None
                 prompt = None
 
+            guard_logs.prompt = prompt
+            guard_logs.instructions = instructions
+
             # Call: run the API.
             output = self.call(index, instructions, prompt, api, output)
 
+            guard_logs.output = output
+
             # Parse: parse the output.
             parsed_output = self.parse(index, output, output_schema)
 
+            guard_logs.parsed_output = parsed_output
+
             # Validate: run output validation.
-            validated_output = self.validate(index, parsed_output, output_schema)
+            validated_output = self.validate(
+                guard_logs, index, parsed_output, output_schema
+            )
+
+            guard_logs.set_validated_output(validated_output)
 
             # Introspect: inspect validated output for reasks.
             reasks = self.introspect(index, validated_output, output_schema)
 
+            guard_logs.reasks = reasks
+
             # Replace reask values with fixed values if terminal step.
             if not self.do_loop(index, reasks):
                 validated_output = sub_reasks_with_fixed_values(validated_output)
 
-            # Log: step information.
-            self.log(
-                prompt=prompt,
-                instructions=instructions,
-                output=output,
-                parsed_output=parsed_output,
-                validated_output=validated_output,
-                reasks=reasks,
-            )
+            guard_logs.set_validated_output(validated_output)
 
             return validated_output, reasks
 
     def prepare(
         self,
         index: int,
         instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
-        api: PromptCallable,
+        api: Union[PromptCallable, AsyncPromptCallable],
         input_schema: Schema,
         output_schema: Schema,
     ) -> Tuple[Instructions, Prompt]:
         """Prepare by running pre-processing and input validation."""
         with start_action(action_type="prepare", index=index) as action:
             if prompt_params is None:
                 prompt_params = {}
@@ -274,83 +287,220 @@
                 error=error,
             )
 
             return parsed_output
 
     def validate(
         self,
+        guard_logs: GuardLogs,
         index: int,
         parsed_output: Any,
         output_schema: Schema,
     ):
         """Validate the output."""
         with start_action(action_type="validate", index=index) as action:
-            validated_output = output_schema.validate(parsed_output)
+            validated_output = output_schema.validate(
+                guard_logs, parsed_output, self.metadata
+            )
 
             action.log(
                 message_type="info",
                 validated_output=reasks_to_dict(validated_output),
             )
 
             return validated_output
 
     def introspect(
         self,
         index: int,
         validated_output: Any,
         output_schema: Schema,
-    ) -> List[ReAsk]:
+    ) -> List[FieldReAsk]:
         """Introspect the validated output."""
         with start_action(action_type="introspect", index=index) as action:
             if validated_output is None:
                 return []
             reasks = output_schema.introspect(validated_output)
 
             action.log(
                 message_type="info",
                 reasks=[r.__dict__ for r in reasks],
             )
 
             return reasks
 
-    def log(
-        self,
-        prompt: Prompt,
-        instructions: Optional[str],
-        output: str,
-        parsed_output: Any,
-        validated_output: Any,
-        reasks: list,
-    ) -> None:
-        """Log the step."""
-        self.guard_history = self.guard_history.push(
-            GuardLogs(
-                prompt=prompt,
-                instructions=instructions,
-                output=output,
-                parsed_output=parsed_output,
-                validated_output=validated_output,
-                reasks=reasks,
-            )
-        )
-
     def do_loop(self, index: int, reasks: List[ReAsk]) -> bool:
         """Determine if we should loop again."""
         if reasks and index < self.num_reasks:
             return True
         return False
 
     def prepare_to_loop(
         self,
         reasks: list,
         validated_output: Optional[Dict],
         output_schema: Schema,
     ) -> Tuple[Prompt, Schema]:
         """Prepare to loop again."""
-        output_schema = output_schema.get_reask_schema(
+        output_schema, prompt = output_schema.get_reask_schema_and_prompt(
             reasks=reasks,
-        )
-        prompt = output_schema.get_reask_prompt(
             reask_value=prune_obj_for_reasking(validated_output),
             reask_prompt_template=self.reask_prompt,
         )
         return prompt, output_schema
+
+
+class AsyncRunner(Runner):
+    api: AsyncPromptCallable
+
+    async def async_run(self, prompt_params: Dict = None) -> GuardHistory:
+        """Execute the runner by repeatedly calling step until the reask budget
+        is exhausted.
+
+        Args:
+            prompt_params: Parameters to pass to the prompt in order to
+                generate the prompt string.
+
+        Returns:
+            The guard history.
+        """
+        self._reset_guard_history()
+
+        with start_action(
+            action_type="run",
+            instructions=self.instructions,
+            prompt=self.prompt,
+            api=self.api,
+            input_schema=self.input_schema,
+            output_schema=self.output_schema,
+            num_reasks=self.num_reasks,
+            metadata=self.metadata,
+        ):
+            instructions, prompt, input_schema, output_schema = (
+                self.instructions,
+                self.prompt,
+                self.input_schema,
+                self.output_schema,
+            )
+            for index in range(self.num_reasks + 1):
+                # Run a single step.
+                validated_output, reasks = await self.async_step(
+                    index=index,
+                    api=self.api,
+                    instructions=instructions,
+                    prompt=prompt,
+                    prompt_params=prompt_params,
+                    input_schema=input_schema,
+                    output_schema=output_schema,
+                    output=self.output if index == 0 else None,
+                )
+
+                # Loop again?
+                if not self.do_loop(index, reasks):
+                    break
+                # Get new prompt and output schema.
+                prompt, output_schema = self.prepare_to_loop(
+                    reasks,
+                    validated_output,
+                    output_schema,
+                )
+
+            return self.guard_history
+
+    async def async_step(
+        self,
+        index: int,
+        api: AsyncPromptCallable,
+        instructions: Optional[Instructions],
+        prompt: Prompt,
+        prompt_params: Dict,
+        input_schema: Schema,
+        output_schema: Schema,
+        output: str = None,
+    ):
+        guard_logs = GuardLogs()
+        self.guard_history.push(guard_logs)
+
+        """Run a full step."""
+        with start_action(
+            action_type="step",
+            index=index,
+            instructions=instructions,
+            prompt=prompt,
+            prompt_params=prompt_params,
+            input_schema=input_schema,
+            output_schema=output_schema,
+        ):
+            # Prepare: run pre-processing, and input validation.
+            if not output:
+                instructions, prompt = self.prepare(
+                    index,
+                    instructions,
+                    prompt,
+                    prompt_params,
+                    api,
+                    input_schema,
+                    output_schema,
+                )
+            else:
+                instructions = None
+                prompt = None
+
+            guard_logs.prompt = prompt
+            guard_logs.instructions = instructions
+
+            # Call: run the API.
+            output = await self.async_call(index, instructions, prompt, api, output)
+
+            guard_logs.output = output
+
+            # Parse: parse the output.
+            parsed_output = self.parse(index, output, output_schema)
+
+            guard_logs.parsed_output = parsed_output
+
+            # Validate: run output validation.
+            validated_output = self.validate(
+                guard_logs, index, parsed_output, output_schema
+            )
+
+            guard_logs.set_validated_output(validated_output)
+
+            # Introspect: inspect validated output for reasks.
+            reasks = self.introspect(index, validated_output, output_schema)
+
+            guard_logs.reasks = reasks
+
+            # Replace reask values with fixed values if terminal step.
+            if not self.do_loop(index, reasks):
+                validated_output = sub_reasks_with_fixed_values(validated_output)
+
+            guard_logs.set_validated_output(validated_output)
+
+            return validated_output, reasks
+
+    async def async_call(
+        self,
+        index: int,
+        instructions: Optional[Instructions],
+        prompt: Prompt,
+        api: AsyncPromptCallable,
+        output: str = None,
+    ) -> str:
+        """Run a step.
+
+        1. Query the LLM API,
+        2. Convert the response string to a dict,
+        3. Log the output
+        """
+        with start_action(action_type="call", index=index, prompt=prompt) as action:
+            if prompt and instructions:
+                output = await api(prompt.source, instructions=instructions.source)
+            elif prompt:
+                output = await api(prompt.source)
+
+            action.log(
+                message_type="info",
+                output=output,
+            )
+
+            return output
```

### Comparing `guardrails-ai-0.1.8/guardrails/schema.py` & `guardrails-ai-0.2.0a1/guardrails/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 from lxml import etree as ET
 from lxml.builder import E
 
 from guardrails.datatypes import DataType, String
 from guardrails.llm_providers import PromptCallable, openai_chat_wrapper, openai_wrapper
 from guardrails.prompt import Instructions, Prompt
 from guardrails.utils.constants import constants
+from guardrails.utils.json_utils import verify_schema_against_json
+from guardrails.utils.logs_utils import FieldValidationLogs, GuardLogs
 from guardrails.utils.reask_utils import (
-    ReAsk,
+    FieldReAsk,
+    SkeletonReAsk,
     gather_reasks,
     get_pruned_tree,
     get_reasks_by_element,
 )
 from guardrails.validators import Validator, check_refrain_in_dict, filter_in_dict
 
 if TYPE_CHECKING:
@@ -305,15 +308,15 @@
         """Parse the schema specification.
 
         Args:
             root: The root element of the schema specification.
         """
         raise NotImplementedError
 
-    def validate(self, data: Any) -> Any:
+    def validate(self, guard_logs: GuardLogs, data: Any, metadata: Dict) -> Any:
         """Validate a dictionary of data against the schema.
 
         Args:
             data: The data to validate.
 
         Returns:
             The validated data.
@@ -325,73 +328,53 @@
         large language model.
 
         Returns:
             The prompt.
         """
         raise NotImplementedError
 
-    def get_reask_schema(
-        self,
-        reasks: List[ReAsk],
-    ) -> "Schema":
-        """Construct a schema for reasking.
-
-        Args:
-            reasks: List of tuples, where each tuple contains the path to the
-                reasked element, and the ReAsk object (which contains the error
-                message describing why the reask is necessary).
-
-        Returns:
-            The prompt.
-        """
-        raise NotImplementedError
-
     def parse(self, output: str) -> Tuple[Any, Optional[Exception]]:
         """Parse the output from the large language model.
 
         Args:
             output: The output from the large language model.
 
         Returns:
             The parsed output, and the exception that was raised (if any).
         """
         raise NotImplementedError
 
-    def introspect(self, data: Any) -> List[ReAsk]:
+    def introspect(self, data: Any) -> List[FieldReAsk]:
         """Inspect the data for reasks.
 
         Args:
             data: The data to introspect.
 
         Returns:
             A list of ReAsk objects.
         """
         raise NotImplementedError
 
-    def get_default_reask_prompt(self) -> Prompt:
-        """Get the default reask prompt for the schema.
-
-        Returns:
-            The default reask prompt.
-        """
-        raise NotImplementedError
-
-    def get_reask_prompt(
+    def get_reask_schema_and_prompt(
         self,
+        reasks: List[FieldReAsk],
         reask_value: Any,
         reask_prompt_template: Optional[Prompt] = None,
-    ) -> Prompt:
-        """Get a reask prompt for the schema.
+    ) -> Tuple["Schema", Prompt]:
+        """Construct a schema for reasking, and a prompt for reasking.
 
         Args:
+            reasks: List of tuples, where each tuple contains the path to the
+                reasked element, and the ReAsk object (which contains the error
+                message describing why the reask is necessary).
             reask_value: The value that was returned from the API, with reasks.
             reask_prompt_template: The template to use for the reask prompt.
 
         Returns:
-            The reask prompt.
+            The schema for reasking, and the prompt for reasking.
         """
         raise NotImplementedError
 
     def preprocess_prompt(
         self,
         prompt_callable: PromptCallable,
         instructions: Optional[Instructions],
@@ -405,50 +388,60 @@
             instructions: The instructions to preprocess.
             prompt: The prompt to preprocess.
         """
         raise NotImplementedError
 
 
 class JsonSchema(Schema):
-    def get_reask_schema(
+    def get_reask_schema_and_prompt(
         self,
-        reasks: List[ReAsk],
-    ) -> "Schema":
+        reasks: List[FieldReAsk],
+        reask_value: Any,
+        reask_prompt_template: Optional[Prompt] = None,
+    ) -> Tuple["Schema", Prompt]:
         parsed_rail = deepcopy(self.root)
 
-        # Get the elements that are to be reasked
-        reask_elements = get_reasks_by_element(reasks, parsed_rail)
+        is_skeleton_reask = not any(isinstance(reask, FieldReAsk) for reask in reasks)
 
-        # Get the pruned tree so that it only contains ReAsk objects
-        pruned_tree = get_pruned_tree(parsed_rail, list(reask_elements.keys()))
-        pruned_tree_schema = type(self)(pruned_tree)
+        if not is_skeleton_reask:
+            # Get the elements that are to be reasked
+            reask_elements = get_reasks_by_element(reasks, parsed_rail)
+
+            # Get the pruned tree so that it only contains ReAsk objects
+            pruned_tree = get_pruned_tree(parsed_rail, list(reask_elements.keys()))
+            pruned_tree_schema = type(self)(pruned_tree)
+        else:
+            pruned_tree_schema = self
 
-        return pruned_tree_schema
-
-    def get_reask_prompt(
-        self,
-        reask_value: Any,
-        reask_prompt_template: Optional[Prompt] = None,
-    ) -> Prompt:
-        pruned_tree_string = self.transpile()
+        pruned_tree_string = pruned_tree_schema.transpile()
 
         if reask_prompt_template is None:
-            reask_prompt_template = self.get_default_reask_prompt()
+            if is_skeleton_reask:
+                reask_prompt_template = Prompt(
+                    constants["high_level_skeleton_reask_prompt"]
+                    + constants["complete_json_suffix"]
+                )
+            else:
+                reask_prompt_template = Prompt(
+                    constants["high_level_json_reask_prompt"]
+                    + constants["complete_json_suffix"]
+                )
 
         def reask_decoder(obj):
             return {
                 k: v for k, v in obj.__dict__.items() if k not in ["path", "fix_value"]
             }
 
-        return reask_prompt_template.format(
+        prompt = reask_prompt_template.format(
             previous_response=json.dumps(reask_value, indent=2, default=reask_decoder)
             .replace("{", "{{")
             .replace("}", "}}"),
             output_schema=pruned_tree_string,
         )
+        return pruned_tree_schema, prompt
 
     def setup_schema(self, root: ET._Element) -> None:
         from guardrails.datatypes import registry as types_registry
 
         strict = False
         if "strict" in root.attrib and root.attrib["strict"] == "true":
             strict = True
@@ -475,23 +468,19 @@
         try:
             output_as_dict = json.loads(output, strict=False)
         except json.decoder.JSONDecodeError as e:
             output_as_dict = None
             error = e
         return output_as_dict, error
 
-    def get_default_reask_prompt(self):
-        return Prompt(
-            constants["high_level_json_reask_prompt"]
-            + constants["complete_json_suffix"]
-        )
-
     def validate(
         self,
+        guard_logs: GuardLogs,
         data: Optional[Dict[str, Any]],
+        metadata: Dict,
     ) -> Optional[Dict[str, Any]]:
         """Validate a dictionary of data against the schema.
 
         Args:
             data: The data to validate.
 
         Returns:
@@ -501,39 +490,64 @@
             return None
 
         if not isinstance(data, dict):
             raise TypeError(f"Argument `data` must be a dictionary, not {type(data)}.")
 
         validated_response = deepcopy(data)
 
+        if not verify_schema_against_json(
+            self.root,
+            validated_response,
+            prune_extra_keys=True,
+            coerce_types=True,
+        ):
+            return SkeletonReAsk(
+                incorrect_value=validated_response,
+                fix_value=None,
+                error_message="JSON does not match schema",
+            )
+
         for field, value in validated_response.items():
             if field not in self:
                 # This is an extra field that is not in the schema.
                 # We remove it from the validated response.
                 logger.debug(f"Field {field} not in schema.")
                 continue
 
+            logger.debug(f"Validating field {field} with value {value}.")
+
+            validation_logs = FieldValidationLogs()
+            guard_logs.field_validation_logs[field] = validation_logs
+
             validated_response = self[field].validate(
+                validation_logs=validation_logs,
                 key=field,
                 value=value,
                 schema=validated_response,
+                metadata=metadata,
+            )
+
+            logger.debug(
+                f"Validated field {field} with value {validated_response[field]}."
             )
 
         if check_refrain_in_dict(validated_response):
             # If the data contains a `Refain` value, we return an empty
             # dictionary.
             logger.debug("Refrain detected.")
             validated_response = {}
 
         # Remove all keys that have `Filter` values.
         validated_response = filter_in_dict(validated_response)
 
         return validated_response
 
-    def introspect(self, data: Dict) -> list:
+    def introspect(self, data: Any) -> list:
+        if isinstance(data, SkeletonReAsk):
+            return [data]
         return gather_reasks(data)
 
     def preprocess_prompt(
         self,
         prompt_callable: PromptCallable,
         instructions: Optional[Instructions],
         prompt: Prompt,
@@ -572,48 +586,43 @@
         else:
             self.string_key = root.attrib["name"] = "string"
 
         # make root tag into a string tag
         root_string = ET.Element("string", root.attrib)
         self[self.string_key] = String.from_xml(root_string)
 
-    def get_reask_schema(
+    def get_reask_schema_and_prompt(
         self,
-        reasks: List[ReAsk],
-    ) -> "Schema":
-        return self
-
-    def get_default_reask_prompt(self):
-        return Prompt(
-            constants["high_level_string_reask_prompt"]
-            + constants["complete_string_suffix"]
-        )
-
-    def get_reask_prompt(
-        self,
-        reask_value: ReAsk,
+        reasks: List[FieldReAsk],
+        reask_value: FieldReAsk,
         reask_prompt_template: Optional[Prompt] = None,
-    ) -> Prompt:
+    ) -> Tuple[Schema, Prompt]:
         pruned_tree_string = self.transpile()
 
         if reask_prompt_template is None:
-            reask_prompt_template = self.get_default_reask_prompt()
+            reask_prompt_template = Prompt(
+                constants["high_level_string_reask_prompt"]
+                + constants["complete_string_suffix"]
+            )
 
-        return reask_prompt_template.format(
+        prompt = reask_prompt_template.format(
             previous_response=reask_value.incorrect_value,
             error_messages=f"- {reask_value.error_message}",
             output_schema=pruned_tree_string,
         )
+        return self, prompt
 
     def parse(self, output: str) -> Tuple[Any, Optional[Exception]]:
         return output, None
 
     def validate(
         self,
+        guard_logs: GuardLogs,
         data: Any,
+        metadata: Dict,
     ) -> Any:
         """Validate a dictionary of data against the schema.
 
         Args:
             data: The data to validate.
 
         Returns:
@@ -621,20 +630,25 @@
         """
         if data is None:
             return None
 
         if not isinstance(data, str):
             raise TypeError(f"Argument `data` must be a string, not {type(data)}.")
 
+        validation_logs = FieldValidationLogs()
+        guard_logs.field_validation_logs[self.string_key] = validation_logs
+
         validated_response = self[self.string_key].validate(
+            validation_logs=validation_logs,
             key=self.string_key,
             value=data,
             schema={
                 self.string_key: data,
             },
+            metadata=metadata,
         )
 
         if check_refrain_in_dict(validated_response):
             # If the data contains a `Refain` value, we return an empty
             # dictionary.
             logger.debug("Refrain detected.")
             validated_response = {}
@@ -642,16 +656,16 @@
         # Remove all keys that have `Filter` values.
         validated_response = filter_in_dict(validated_response)
 
         if self.string_key in validated_response:
             return validated_response[self.string_key]
         return None
 
-    def introspect(self, data: Any) -> List[ReAsk]:
-        if isinstance(data, ReAsk):
+    def introspect(self, data: Any) -> List[FieldReAsk]:
+        if isinstance(data, FieldReAsk):
             return [data]
         return []
 
     def preprocess_prompt(
         self,
         prompt_callable: PromptCallable,
         instructions: Optional[Instructions],
```

### Comparing `guardrails-ai-0.1.8/guardrails/utils/constants.py` & `guardrails-ai-0.2.0a1/guardrails/utils/constants.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/utils/docs_utils.py` & `guardrails-ai-0.2.0a1/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/utils/logs_utils.py` & `guardrails-ai-0.2.0a1/guardrails/utils/logs_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 from copy import deepcopy
-from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Optional, Union
 
 from rich.console import Group
 from rich.panel import Panel
 from rich.pretty import pretty_repr
 from rich.tree import Tree
 
 from guardrails.prompt import Prompt
 from guardrails.utils.reask_utils import ReAsk, gather_reasks, prune_obj_for_reasking
 
 
 @dataclass
+class ValidatorLogs:
+    """Logs for a single validator."""
+
+    validator_name: str
+    value_before_validation: Any
+    value_after_validation: Optional[Any] = None
+
+
+@dataclass
+class FieldValidationLogs:
+    """Logs for a single field."""
+
+    validator_logs: List[ValidatorLogs] = field(default_factory=list)
+    children: Dict[Union[int, str], "FieldValidationLogs"] = field(default_factory=dict)
+
+
+@dataclass
 class GuardLogs:
-    prompt: Prompt
-    instructions: Optional[str]
-    output: str
-    parsed_output: dict
-    validated_output: dict
-    reasks: List[ReAsk]
+    prompt: Optional[Prompt] = None
+    instructions: Optional[str] = None
+    output: Optional[str] = None
+    parsed_output: Optional[dict] = None
+    validated_output: Optional[dict] = None
+    reasks: Optional[List[ReAsk]] = None
+
+    field_validation_logs: Dict[Union[int, str], FieldValidationLogs] = field(
+        default_factory=dict
+    )
+
+    _previous_logs: Optional["GuardLogs"] = None
+
+    def set_validated_output(self, validated_output):
+        if self._previous_logs is not None:
+            validated_output = merge_reask_output(
+                self._previous_logs.validated_output, validated_output
+            )
+        self.validated_output = validated_output
 
     @property
     def failed_validations(self) -> List[ReAsk]:
         """Returns the failed validations."""
         return gather_reasks(self.validated_output)
 
     @property
@@ -60,20 +90,20 @@
             )
 
 
 @dataclass
 class GuardHistory:
     history: List[GuardLogs]
 
-    def push(self, guard_log: GuardLogs) -> "GuardHistory":
+    def push(self, guard_log: GuardLogs) -> None:
         if len(self.history) > 0:
             last_log = self.history[-1]
-            guard_log.validated_output = merge_reask_output(last_log, guard_log)
+            guard_log._previous_logs = last_log
 
-        return GuardHistory(self.history + [guard_log])
+        self.history += [guard_log]
 
     @property
     def tree(self) -> Tree:
         """Returns the tree."""
         tree = Tree("Logs")
         for i, log in enumerate(self.history):
             tree.add(Panel(log.rich_group, title=f"Step {i}"))
@@ -100,16 +130,16 @@
         return [log.failed_validations for log in self.history]
 
 
 @dataclass
 class GuardState:
     all_histories: List[GuardHistory]
 
-    def push(self, guard_history: GuardHistory) -> "GuardState":
-        return GuardState(self.all_histories + [guard_history])
+    def push(self, guard_history: GuardHistory) -> None:
+        self.all_histories += [guard_history]
 
     @property
     def most_recent_call(self) -> GuardHistory:
         """Returns the most recent call."""
         if not len(self.all_histories):
             return None
         return self.all_histories[-1]
@@ -124,28 +154,26 @@
         value: The value to be updated.
     """
     for key in path[:-1]:
         output = output[key]
     output[path[-1]] = value
 
 
-def merge_reask_output(prev_logs: GuardLogs, current_logs: GuardLogs) -> Dict:
+def merge_reask_output(previous_response, reask_response) -> Dict:
     """Merge the reask output into the original output.
 
     Args:
         prev_logs: GuardLogs object from the previous iteration.
         current_logs: GuardLogs object from the current iteration.
 
     Returns:
         The merged output.
     """
     from guardrails.validators import PydanticReAsk
 
-    previous_response = prev_logs.validated_output
-    reask_response = current_logs.validated_output
     if isinstance(previous_response, ReAsk):
         return reask_response
 
     pruned_reask_json = prune_obj_for_reasking(previous_response)
 
     # Reask output and reask json have the same structure, except that values
     # of the reask json are ReAsk objects. We want to replace the ReAsk objects
```

### Comparing `guardrails-ai-0.1.8/guardrails/utils/pydantic_utils.py` & `guardrails-ai-0.2.0a1/guardrails/utils/pydantic_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,16 +181,17 @@
 
     return type_annotation
 
 
 def type_annotation_to_string(type_annotation: Any) -> str:
     """Map a type_annotation to the name of the corresponding field type.
 
-    This function checks if the type_annotation is a list, dict, or a primitive type,
-    and returns the corresponding type name, e.g. "list", "object", "bool", "date", etc.
+    This function checks if the type_annotation is a list, dict, or a
+    primitive type, and returns the corresponding type name, e.g.
+    "list", "object", "bool", "date", etc.
     """
 
     # Get the type annotation from the type_annotation
     type_annotation = prepare_type_annotation(type_annotation)
 
     # Map the type annotation to the corresponding field type
     if is_list(type_annotation):
@@ -212,15 +213,15 @@
     elif type_annotation == HttpUrl:
         return "url"
     else:
         raise ValueError(f"Unsupported type: {type_annotation}")
 
 
 def add_validators_to_xml_element(field_info: ModelField, element: Element) -> Element:
-    """Extract validators from a pydantic ModelField and add to XML element
+    """Extract validators from a pydantic ModelField and add to XML element.
 
     Args:
         field_info: The field info to extract validators from
         element: The XML element to add the validators to
 
     Returns:
         The XML element with the validators added
@@ -281,14 +282,19 @@
     element = add_validators_to_xml_element(field, element)
 
     # Add description attribute
     if isinstance(field, ModelField):
         if field.field_info.description is not None:
             element.set("description", field.field_info.description)
 
+        # Add other attributes from the field_info
+        for key, value in field.field_info.extra.items():
+            if key not in ["validators", "description", "when"]:
+                element.set(key, value)
+
     # Create XML elements for the field's children
     if field_type in ["list", "object"]:
         type_annotation = prepare_type_annotation(field)
 
         if is_list(type_annotation):
             inner_type = get_args(type_annotation)
             if len(inner_type) == 0:
@@ -459,15 +465,14 @@
         model: A pydantic BaseModel.
 
     Returns:
         A dictionary mapping field names to ModelField objects.
     """
 
     def process_validators(vals, fld):
-
         if not vals:
             return
 
         for val in vals:
             gd_validator = convert_pydantic_validator_to_guardrails_validator(
                 model, val
             )
```

### Comparing `guardrails-ai-0.1.8/guardrails/utils/reask_utils.py` & `guardrails-ai-0.2.0a1/guardrails/utils/reask_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,27 @@
 
 
 @dataclass
 class ReAsk:
     incorrect_value: Any
     error_message: str
     fix_value: Any
+
+
+@dataclass
+class FieldReAsk(ReAsk):
     path: List[Any] = None
 
 
-def gather_reasks(validated_output: Dict) -> List[ReAsk]:
+@dataclass
+class SkeletonReAsk(ReAsk):
+    pass
+
+
+def gather_reasks(validated_output: Dict) -> List[FieldReAsk]:
     """Traverse output and gather all ReAsk objects.
 
     Args:
         validated_output (Dict): The output of a model. Each value can be a ReAsk,
             a list, a dictionary, or a single value.
 
     Returns:
@@ -26,15 +35,15 @@
     from guardrails.validators import PydanticReAsk
 
     reasks = []
 
     def _gather_reasks_in_dict(output: Dict, path: List[str] = []) -> None:
         is_pydantic = isinstance(output, PydanticReAsk)
         for field, value in output.items():
-            if isinstance(value, ReAsk):
+            if isinstance(value, FieldReAsk):
                 if is_pydantic:
                     value.path = path
                 else:
                     value.path = path + [field]
                 reasks.append(value)
 
             if isinstance(value, dict):
@@ -42,29 +51,29 @@
 
             if isinstance(value, list):
                 _gather_reasks_in_list(value, path + [field])
         return
 
     def _gather_reasks_in_list(output: List, path: List[str] = []) -> None:
         for idx, item in enumerate(output):
-            if isinstance(item, ReAsk):
+            if isinstance(item, FieldReAsk):
                 item.path = path + [idx]
                 reasks.append(item)
             elif isinstance(item, dict):
                 _gather_reasks_in_dict(item, path + [idx])
             elif isinstance(item, list):
                 _gather_reasks_in_list(item, path + [idx])
         return
 
     _gather_reasks_in_dict(validated_output)
     return reasks
 
 
 def get_reasks_by_element(
-    reasks: List[ReAsk],
+    reasks: List[FieldReAsk],
     parsed_rail: ET._Element,
 ) -> Dict[ET._Element, List[tuple]]:
     """Cluster reasks by the XML element they are associated with."""
     # This should be guaranteed to work, since the path corresponding
     # to a ReAsk should always be valid in the element tree.
 
     # This is because ReAsk objects are only created for elements
@@ -159,15 +168,15 @@
                 pruned_list.append(pruned_output)
         if len(pruned_list):
             return pruned_list
         return None
     elif isinstance(obj, dict):
         pruned_json = {}
         for key, value in obj.items():
-            if isinstance(value, ReAsk) or isinstance(value, PydanticReAsk):
+            if isinstance(value, FieldReAsk) or isinstance(value, PydanticReAsk):
                 pruned_json[key] = value
             elif isinstance(value, dict):
                 pruned_output = prune_obj_for_reasking(value)
                 if pruned_output is not None:
                     pruned_json[key] = pruned_output
             elif isinstance(value, list):
                 pruned_list = []
@@ -188,15 +197,15 @@
     """If a ReAsk object exists in the dict, return it as a dictionary."""
 
     def _(dict_object: Any) -> Any:
         if isinstance(dict_object, dict):
             return {key: _(value) for key, value in dict_object.items()}
         elif isinstance(dict_object, list):
             return [_(item) for item in dict_object]
-        elif isinstance(dict_object, ReAsk):
+        elif isinstance(dict_object, FieldReAsk):
             return dict_object.__dict__
         else:
             return dict_object
 
     return _(dict_with_reasks)
 
 
@@ -211,11 +220,11 @@
     """
     if isinstance(value, list):
         for index, item in enumerate(value):
             value[index] = sub_reasks_with_fixed_values(item)
     elif isinstance(value, dict):
         for dict_key, dict_value in value.items():
             value[dict_key] = sub_reasks_with_fixed_values(dict_value)
-    elif isinstance(value, ReAsk):
+    elif isinstance(value, FieldReAsk):
         value = value.fix_value
 
     return value
```

### Comparing `guardrails-ai-0.1.8/guardrails/utils/sql_utils.py` & `guardrails-ai-0.2.0a1/guardrails/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/validators.py` & `guardrails-ai-0.2.0a1/guardrails/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 """
 import ast
 import logging
 import os
 import re
 from collections import defaultdict
 from copy import deepcopy
-from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, Type, Union
 
 import openai
+import pydantic
 from pydantic import BaseModel, ValidationError
 
 from guardrails.datatypes import registry as types_registry
 from guardrails.utils.docs_utils import sentence_split
-from guardrails.utils.reask_utils import ReAsk
+from guardrails.utils.reask_utils import FieldReAsk
 from guardrails.utils.sql_utils import SQLDriver, create_sql_driver
 
 try:
     import numpy as np
 except ImportError:
     _HAS_NUMPY = False
 else:
@@ -169,23 +169,28 @@
         validators_registry[name] = cls
         cls.rail_alias = name
         return cls
 
     return decorator
 
 
-@dataclass
-class EventDetail(BaseException):
-    """Event detail."""
-
-    key: str
-    value: Any
-    schema: Dict[str, Any]
+class ValidationResult(pydantic.BaseModel):
+    outcome: str
+    metadata: Optional[Dict[str, Any]] = None
+
+
+class PassResult(ValidationResult):
+    outcome: Literal["pass"] = "pass"
+
+
+class FailResult(ValidationResult):
+    outcome: Literal["fail"] = "fail"
+
     error_message: str
-    fix_value: Any
+    fix_value: Optional[Any] = None
 
 
 class Validator:
     """Base class for validators."""
 
     def __init__(self, on_fail: Optional[Callable] = None, **kwargs):
         if isinstance(on_fail, str):
@@ -196,79 +201,86 @@
         # Store the kwargs for the validator.
         self._kwargs = kwargs
 
         assert (
             self.rail_alias in validators_registry
         ), f"Validator {self.__class__.__name__} is not registered. "
 
-    def validate_with_correction(self, key, value, schema) -> Dict:
-        try:
-            return self.validate(key, value, schema)
-        except EventDetail as e:
+    def validate_with_correction(self, value: Any, metadata: Dict) -> Any:
+        """Validate a value and return either:
+
+        - the value
+        - a fixed value
+        - a reask object
+        - a refrain object
+        - a filter object
+        """
+        result = self.validate(value, metadata)
+        if result.metadata is None:
+            result.metadata = metadata
+
+        if isinstance(result, FailResult):
             logger.debug(
-                f"Validator {self.__class__.__name__} failed for {key} with error {e}."
+                f"Validator {self.__class__.__name__} failed for {value} "
+                f"with error {result.error_message}."
             )
-            return self.on_fail(e)
+            return self.on_fail(value, result)
+        return value
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
-        """Validate a value."""
+    def validate(self, value: Any, metadata: Dict[str, Any]) -> ValidationResult:
+        """Validate a value and return a validation result."""
         raise NotImplementedError
 
-    def fix(self, error: EventDetail) -> Dict:
+    def fix(self, value: Any, error: FailResult) -> Any:
         """Debug the incorrect value."""
-        error.schema[error.key] = error.fix_value
-        return error.schema
+        return error.fix_value
 
-    def reask(self, error: EventDetail) -> Dict:
+    def reask(self, value: Any, error: FailResult) -> Any:
         """Reask disambiguates the validation failure into a helpful error
         message."""
-
-        error.schema[error.key] = ReAsk(
-            incorrect_value=error.value,
+        return FieldReAsk(
+            incorrect_value=value,
             error_message=error.error_message,
             fix_value=error.fix_value,
         )
-        return error.schema
 
-    def filter(self, error: EventDetail) -> Dict:
+    def filter(self, value: Any, error: FailResult) -> Any:
         """If validation fails, filter the offending key from the schema."""
-        logger.debug(f"Filtering {error.key} from schema...")
+        # logger.debug(f"Filtering {error.key} from schema...")
+        return Filter()
 
-        error.schema[error.key] = Filter()
-
-        return error.schema
-
-    def refrain(self, error: EventDetail) -> Optional[Dict]:
+    def refrain(self, value: Any, error: FailResult) -> Any:
         """If validation fails, refrain from answering."""
-        logger.debug(f"Refusing to answer {error.key}...")
-
-        error.schema[error.key] = Refrain()
-        return error.schema
+        # logger.debug(f"Refusing to answer {error.key}...")
+        return Refrain()
 
-    def noop(self, error: EventDetail) -> Dict:
+    def noop(self, value: Any, error: FailResult) -> Any:
         """If validation fails, do nothing."""
-        logger.debug(
-            f"Validator {self.__class__.__name__} failed for {error.key}, "
-            "but doing nothing..."
-        )
+        # logger.debug(
+        #     f"Validator {self.__class__.__name__} failed for {error.key}, "
+        #     "but doing nothing..."
+        # )
+        return value
 
-        return error.schema
-
-    def exception(self, error: EventDetail) -> None:
+    def exception(self, value: Any, error: FailResult) -> None:
         """Raise an exception."""
         raise ValidatorError(error.error_message)
 
-    def fix_reask(self, error: EventDetail) -> Dict:
+    def fix_reask(self, value: Any, error: FailResult) -> Dict:
         """If validation fails, fix the value and reask."""
-        schema = self.fix(error)
+        fixed_value = self.fix(value, error)
 
-        try:
-            self.validate(error.key, error.fix_value, schema)
-        except EventDetail as e:
-            return self.reask(e)
+        result = self.validate(fixed_value, error.metadata)
+        if result.metadata is None:
+            result.metadata = error.metadata
+
+        if isinstance(result, FailResult):
+            return self.reask(fixed_value, result)
+
+        return fixed_value
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         """Convert the validator to a prompt.
 
         E.g. ValidLength(5, 10) -> "length: 5 10" when with_keywords is False.
         ValidLength(5, 10) -> "length: min=5 max=10" when with_keywords is True.
 
@@ -304,15 +316,15 @@
                 str_arg = "{" + str_arg + "}" if " " in str_arg else str_arg
                 validator_args.append(str_arg)
 
         params = " ".join(validator_args)
         return f"{self.rail_alias}: {params}"
 
     def __call__(self, v: Any) -> Any:
-        return self.validate("dummy_key", v, {"dummy_key": v})["dummy_key"]
+        return self.validate_with_correction(v, {})
 
 
 # @register_validator('required', 'all')
 # class Required(Validator):
 #     """Validate that a value is not None."""
 
 #     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> bool:
@@ -344,17 +356,15 @@
         model: Type[BaseModel],
         on_fail: Optional[Callable] = None,
     ):
         super().__init__(on_fail=on_fail)
 
         self.model = model
 
-    def validate_with_correction(
-        self, key: str, value: Dict, schema: Union[Dict, List]
-    ) -> Dict:
+    def validate_with_correction(self, value: Dict, metadata: Dict) -> Any:
         """Validate an object using Pydantic.
 
         For example, consider the following data for a `Person` model
         with fields `name`, `age`, and `zipcode`:
         {
             "user" : {
                 "name": "John",
@@ -383,64 +393,60 @@
                     path=None,
                 )
             }
         }
         """
         try:
             # Run the Pydantic model on the value.
-            schema[key] = self.model(**value)
+            return self.model(**value)
         except ValidationError as e:
             # Create a copy of the value so that we can modify it
             # to insert e.g. ReAsk objects.
             new_value = deepcopy(value)
             for error in e.errors():
                 assert (
                     len(error["loc"]) == 1
                 ), "Pydantic validation errors should only have one location."
 
                 field_name = error["loc"][0]
-                event_detail = EventDetail(
-                    key=field_name,
-                    value=new_value[field_name],
-                    schema=new_value,
+                field_value = value[field_name]
+
+                fail_result = FailResult(
                     error_message=error["msg"],
                     fix_value=None,
                 )
                 # Call the on_fail method and reassign the value.
-                new_value = self.on_fail(event_detail)
+                new_value[field_name] = self.on_fail(field_value, fail_result)
 
             # Insert the new `value` dictionary into the schema.
             # This now contains e.g. ReAsk objects.
-            schema[key] = PydanticReAsk(new_value)
-
-        return schema
+            return PydanticReAsk(new_value)
 
 
 @register_validator(name="pydantic_field_validator", data_type="all")
 class PydanticFieldValidator(Validator):
     def __init__(
         self,
         field_validator: Callable,
         on_fail: Optional[Callable[..., Any]] = None,
         **kwargs,
     ):
         self.field_validator = field_validator
         super().__init__(on_fail, **kwargs)
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate_with_correction(self, value: Any, metadata: Dict) -> ValidationResult:
         try:
-            return self.field_validator(value)
+            validated_field = self.field_validator(value)
         except Exception as e:
-            raise EventDetail(
-                key=key,
-                value=value,
-                schema=schema,
+            result = FailResult(
                 error_message=str(e),
                 fix_value=None,
             )
+            return self.on_fail(value, result)
+        return validated_field
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         return self.field_validator.__func__.__name__
 
 
 @register_validator(name="choice", data_type="choice")
 class Choice(Validator):
@@ -456,54 +462,51 @@
         choices: List[str],
         on_fail: Optional[Callable] = None,
     ):
         super().__init__(on_fail=on_fail, choices=choices)
 
         self._choices = choices
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         """Validate that a value is one of a set of choices."""
         logger.debug(f"Validating {value} is in {self._choices}...")
 
+        # This validator is only
+        assert (
+            "__schema" in metadata
+        ), "Validator should only be invoked by Choice datatype"
+        schema = metadata["__schema"]
+
         if value not in self._choices:
-            raise EventDetail(
-                key=key,
-                value=value,
-                schema=schema,
+            return FailResult(
                 error_message=f"{value} is not in {self._choices}",
                 fix_value=None,
             )
 
         selected_choice = value
         if selected_choice not in schema:
-            raise EventDetail(
-                key=key,
-                value=value,
-                schema=schema,
+            return FailResult(
                 error_message=f"{schema} must contain a key called {value}",
                 fix_value=None,
             )
 
         # Make sure that no other choice is selected.
         for choice in self._choices:
             if choice == selected_choice:
                 continue
             if choice in schema:
-                raise EventDetail(
-                    key=key,
-                    value=value,
-                    schema=schema,
+                return FailResult(
                     error_message=(
                         f"{schema} must not contain a key called {choice}, "
                         f"since {selected_choice} is selected"
                     ),
                     fix_value=None,
                 )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="valid-range", data_type=["integer", "float", "percentage"])
 class ValidRange(Validator):
     """Validate that a value is within a range.
 
     - Name for `format` attribute: `valid-range`
@@ -515,39 +518,33 @@
         self, min: int = None, max: int = None, on_fail: Optional[Callable] = None
     ):
         super().__init__(on_fail=on_fail, min=min, max=max)
 
         self._min = min
         self._max = max
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         """Validate that a value is within a range."""
         logger.debug(f"Validating {value} is in range {self._min} - {self._max}...")
 
         val_type = type(value)
 
         if self._min is not None and value < val_type(self._min):
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is less than {self._min}.",
-                self._min,
+            return FailResult(
+                error_message=f"Value {value} is less than {self._min}.",
+                fix_value=self._min,
             )
 
         if self._max is not None and value > val_type(self._max):
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is greater than {self._max}.",
-                self._max,
+            return FailResult(
+                error_message=f"Value {value} is greater than {self._max}.",
+                fix_value=self._max,
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="valid-choices", data_type="all")
 class ValidChoices(Validator):
     """Validate that a value is within the acceptable choices.
 
     - Name for `format` attribute: `valid-choices`
@@ -555,76 +552,66 @@
     - Programmatic fix: None.
     """
 
     def __init__(self, choices: List[Any], on_fail: Optional[Callable] = None):
         super().__init__(on_fail=on_fail, choices=choices)
         self._choices = choices
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         """Validate that a value is within a range."""
         logger.debug(f"Validating {value} is in choices {self._choices}...")
 
         if value not in self._choices:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is not in choices {self._choices}.",
-                None,
+            return FailResult(
+                error_message=f"Value {value} is not in choices {self._choices}.",
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="lower-case", data_type="string")
 class LowerCase(Validator):
     """Validate that a value is lower case.
 
     - Name for `format` attribute: `lower-case`
     - Supported data types: `string`
     - Programmatic fix: Manually convert to lower case.
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is lower case...")
 
         if value.lower() != value:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is not lower case.",
-                value.lower(),
+            return FailResult(
+                error_message=f"Value {value} is not lower case.",
+                fix_value=value.lower(),
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="upper-case", data_type="string")
 class UpperCase(Validator):
     """Validate that a value is upper case.
 
     - Name for `format` attribute: `upper-case`
     - Supported data types: `string`
     - Programmatic fix: Manually convert to upper case.
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is upper case...")
 
         if value.upper() != value:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is not upper case.",
-                value.upper(),
+            return FailResult(
+                error_message=f"Value {value} is not upper case.",
+                fix_value=value.upper(),
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="length", data_type=["string", "list"])
 class ValidLength(Validator):
     """Validate that the length of value is within the expected range.
 
     - Name for `format` attribute: `length`
@@ -636,15 +623,15 @@
     def __init__(
         self, min: int = None, max: int = None, on_fail: Optional[Callable] = None
     ):
         super().__init__(on_fail=on_fail, min=min, max=max)
         self._min = int(min) if min is not None else None
         self._max = int(max) if max is not None else None
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         """Validate that a value is within a range."""
         logger.debug(
             f"Validating {value} is in length range {self._min} - {self._max}..."
         )
 
         if self._min is not None and len(value) < self._min:
             logger.debug(f"Value {value} is less than {self._min}.")
@@ -652,122 +639,142 @@
             # Repeat the last character to make the value the correct length.
             if isinstance(value, str):
                 last_val = value[-1]
             else:
                 last_val = [value[-1]]
 
             corrected_value = value + last_val * (self._min - len(value))
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value has length less than {self._min}. "
+            return FailResult(
+                error_message=f"Value has length less than {self._min}. "
                 f"Please return a longer output, "
                 f"that is shorter than {self._max} characters.",
-                corrected_value,
+                fix_value=corrected_value,
             )
 
         if self._max is not None and len(value) > self._max:
             logger.debug(f"Value {value} is greater than {self._max}.")
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value has length greater than {self._max}. "
+            return FailResult(
+                error_message=f"Value has length greater than {self._max}. "
                 f"Please return a shorter output, "
                 f"that is shorter than {self._max} characters.",
-                value[: self._max],
+                fix_value=value[: self._max],
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="two-words", data_type="string")
 class TwoWords(Validator):
     """Validate that a value is two words.
 
     - Name for `format` attribute: `two-words`
     - Supported data types: `string`
     - Programmatic fix: Pick the first two words.
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is two words...")
 
         if len(value.split()) != 2:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                "must be exactly two words",
-                " ".join(value.split()[:2]),
+            return FailResult(
+                error_message="must be exactly two words",
+                fix_value=" ".join(value.split()[:2]),
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="one-line", data_type="string")
 class OneLine(Validator):
     """Validate that a value is a single line or sentence.
 
     - Name for `format` attribute: `one-line`
     - Supported data types: `string`
     - Programmatic fix: Pick the first line.
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is a single line...")
 
         if len(value.splitlines()) > 1:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is not a single line.",
-                value.splitlines()[0],
+            return FailResult(
+                error_message=f"Value {value} is not a single line.",
+                fix_value=value.splitlines()[0],
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="valid-url", data_type=["string", "url"])
-class ValidUrl(Validator):
+class ValidURL(Validator):
     """Validate that a value is a valid URL.
 
     - Name for `format` attribute: `valid-url`
     - Supported data types: `string`, `url`
     - Programmatic fix: None
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
+        logger.debug(f"Validating {value} is a valid URL...")
+
+        from urllib.parse import urlparse
+
+        # Check that the URL is valid
+        try:
+            result = urlparse(value)
+            # Check that the URL has a scheme and network location
+            if not result.scheme or not result.netloc:
+                return FailResult(
+                    error_message=f"URL {value} is not valid.",
+                )
+        except ValueError:
+            return FailResult(
+                error_message=f"URL {value} is not valid.",
+            )
+
+        return PassResult()
+
+
+@register_validator(name="is-reachable", data_type=["string", "url"])
+class EndpointIsReachable(Validator):
+    """Validate that a value is a reachable URL.
+
+    - Name for `format` attribute: `is-reachable`
+    - Supported data types: `string`, `url`
+    - Programmatic fix: None
+    """
+
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is a valid URL...")
 
         import requests
 
         # Check that the URL exists and can be reached
         try:
             response = requests.get(value)
             if response.status_code != 200:
-                raise EventDetail(
-                    key,
-                    value,
-                    schema,
-                    f"URL {value} returned status code {response.status_code}",
-                    None,
+                return FailResult(
+                    error_message=f"URL {value} returned "
+                    f"status code {response.status_code}",
                 )
         except requests.exceptions.ConnectionError:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"URL {value} could not be reached",
-                None,
+            return FailResult(
+                error_message=f"URL {value} could not be reached",
+            )
+        except requests.exceptions.InvalidSchema:
+            return FailResult(
+                error_message=f"URL {value} does not specify "
+                f"a valid connection adapter",
+            )
+        except requests.exceptions.MissingSchema:
+            return FailResult(
+                error_message=f"URL {value} does not contain " f"a http schema",
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="bug-free-python", data_type="pythoncode")
 class BugFreePython(Validator):
     """Validate that there are no Python syntactic bugs in the generated code.
 
     This validator checks for syntax errors by running `ast.parse(code)`,
@@ -775,30 +782,26 @@
     Only the packages in the `python` environment are available to the code snippet.
 
     - Name for `format` attribute: `bug-free-python`
     - Supported data types: `pythoncode`
     - Programmatic fix: None
     """
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is not a bug...")
 
         # The value is a Python code snippet. We need to check for syntax errors.
         try:
             ast.parse(value)
         except SyntaxError as e:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                e,
-                None,
+            return FailResult(
+                error_message=f"Syntax error: {e.msg}",
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="bug-free-sql", data_type="sql")
 class BugFreeSQL(Validator):
     """Validate that there are no SQL syntactic bugs in the generated code.
 
     This is a very minimal implementation that uses the Pypi `sqlvalidator` package
@@ -815,96 +818,86 @@
         conn: Optional[str] = None,
         schema_file: Optional[str] = None,
         on_fail: Optional[Callable] = None,
     ):
         super().__init__(on_fail=on_fail)
         self._driver: SQLDriver = create_sql_driver(schema_file=schema_file, conn=conn)
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         errors = self._driver.validate_sql(value)
         if len(errors) > 0:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                ". ".join(errors),
-                None,
+            return FailResult(
+                error_message=". ".join(errors),
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="sql-column-presence", data_type="sql")
 class SqlColumnPresence(Validator):
     """Validate that all columns in the SQL query are present in the schema.
 
     - Name for `format` attribute: `sql-column-presence`
     - Supported data types: `string`
     """
 
     def __init__(self, cols: List[str], on_fail: Optional[Callable] = None):
         super().__init__(on_fail=on_fail, cols=cols)
         self._cols = set(cols)
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         from sqlglot import exp, parse
 
         expressions = parse(value)
         cols = set()
         for expression in expressions:
             for col in expression.find_all(exp.Column):
                 cols.add(col.alias_or_name)
 
         diff = cols.difference(self._cols)
         if len(diff) > 0:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Columns [{', '.join(diff)}] not in [{', '.join(self._cols)}]",
-                None,
+            return FailResult(
+                error_message=f"Columns [{', '.join(diff)}] "
+                f"not in [{', '.join(self._cols)}]",
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="exclude-sql-predicates", data_type="sql")
 class ExcludeSqlPredicates(Validator):
     """Validate that the SQL query does not contain certain predicates.
 
     - Name for `format` attribute: `exclude-sql-predicates`
     - Supported data types: `sql`
     """
 
     def __init__(self, predicates: List[str], on_fail: Optional[Callable] = None):
         super().__init__(on_fail=on_fail, predicates=predicates)
         self._predicates = set(predicates)
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         from sqlglot import exp, parse
 
         expressions = parse(value)
         for expression in expressions:
             if expression is None:
                 continue
             for pred in self._predicates:
                 try:
                     getattr(exp, pred)
                 except AttributeError:
                     raise ValueError(f"Predicate {pred} does not exist")
                 if len(list(expression.find_all(getattr(exp, pred)))):
-                    raise EventDetail(
-                        key,
-                        value,
-                        schema,
-                        f"SQL query contains predicate {pred}",
-                        "",
+                    return FailResult(
+                        error_message=f"SQL query contains predicate {pred}",
+                        fix_value="",
                     )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="similar-to-document", data_type="string")
 class SimilarToDocument(Validator):
     """Validate that a value is similar to the document.
 
     This validator checks if the value is similar to the document by checking
@@ -947,37 +940,34 @@
             b: The second vector.
 
         Returns:
             float: The cosine similarity between the two vectors.
         """
         return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} is similar to document...")
 
         value_embedding = np.array(
             openai.Embedding.create(input=[value], model=self._model)["data"][0][
                 "embedding"
             ]
         )
 
         similarity = SimilarToDocument.cosine_similarity(
             self._document_embedding,
             value_embedding,
         )
         if similarity < self._threshold:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"Value {value} is not similar enough to document {self._document}.",
-                None,
+            return FailResult(
+                error_message=f"Value {value} is not similar enough "
+                f"to document {self._document}.",
             )
 
-        return schema
+        return PassResult()
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         return ""
 
 
 @register_validator(name="is-profanity-free", data_type="string")
 class IsProfanityFree(Validator):
@@ -987,33 +977,31 @@
     contains profanity language.
 
     - Name for `format` attribute: `is-profanity-free`
     - Supported data types: `string`
     - Programmatic fix: ""
     """
 
-    def validate(self, key, value, schema) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         try:
             from profanity_check import predict
         except ImportError:
             raise ImportError(
                 "`is-profanity-free` validator requires the `alt-profanity-check`"
                 "package. Please install it with `pip install profanity-check`."
             )
 
         prediction = predict([value])
         if prediction[0] == 1:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"{value} contains profanity. Please return a profanity-free output.",
-                "",
+            return FailResult(
+                error_message=f"{value} contains profanity. "
+                f"Please return a profanity-free output.",
+                fix_value="",
             )
-        return schema
+        return PassResult()
 
 
 @register_validator(name="is-high-quality-translation", data_type="string")
 class IsHighQualityTranslation(Validator):
     """Using inpiredco.critique to check if a translation is high quality.
 
     - Name for `format` attribute: `is-high-quality-translation`
@@ -1030,31 +1018,34 @@
 
         except ImportError:
             raise ImportError(
                 "`is-high-quality-translation` validator requires the `inspiredco`"
                 "package. Please install it with `pip install inspiredco`."
             )
 
-    def validate(self, key, value, schema) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
+        if "translation_source" not in metadata:
+            raise RuntimeError(
+                "is-high-quality-translation validator expects "
+                "`translation_source` key in metadata"
+            )
+        src = metadata["translation_source"]
         prediction = self.critique.evaluate(
             metric="comet",
             config={"model": "unbabel_comet/wmt21-comet-qe-da"},
-            dataset=[{"source": key, "target": value}],
+            dataset=[{"source": src, "target": value}],
         )
         quality = prediction["examples"][0]["value"]
         if quality < -0.1:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"{value} is a low quality translation."
+            return FailResult(
+                error_message=f"{value} is a low quality translation."
                 "Please return a higher quality output.",
-                "",
+                fix_value="",
             )
-        return schema
+        return PassResult()
 
 
 @register_validator(name="ends-with", data_type="list")
 class EndsWith(Validator):
     """Validate that a list ends with a given value.
 
     - Name for `format` attribute: `ends-with`
@@ -1062,143 +1053,156 @@
     - Programmatic fix: Append the given value to the list.
     """
 
     def __init__(self, end: str, on_fail: str = "fix"):
         super().__init__(on_fail=on_fail, end=end)
         self._end = end
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(f"Validating {value} ends with {self._end}...")
 
         if not value[-1] == self._end:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"{value} must end with {self._end}",
-                value + [self._end],
+            return FailResult(
+                error_message=f"{value} must end with {self._end}",
+                fix_value=value + [self._end],
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="extracted-summary-sentences-match", data_type="string")
 class ExtractedSummarySentencesMatch(Validator):
     """Validate that the extracted summary sentences match the original text by
     performing a cosine similarity in the embedding space."""
 
     def __init__(
         self,
-        documents_dir: str,
         threshold: float = 0.7,
-        embedding_model: Optional["EmbeddingBase"] = None,  # noqa: F821
-        vector_db: Optional["VectorDBBase"] = None,  # noqa: F821
-        document_store: Optional["DocumentStoreBase"] = None,  # noqa: F821
         on_fail: Optional[Callable] = None,
         **kwargs,
     ):
         super().__init__(on_fail, **kwargs)
         # TODO(shreya): Pass embedding_model, vector_db, document_store from spec
 
-        if document_store is None:
-            from guardrails.document_store import EphemeralDocumentStore
-
-            if vector_db is None:
-                from guardrails.vectordb import Faiss
+        self._threshold = float(threshold)
 
-                if embedding_model is None:
-                    from guardrails.embedding import OpenAIEmbedding
+    @staticmethod
+    def _instantiate_store(metadata):
+        if "document_store" in metadata:
+            return metadata["document_store"]
 
-                    embedding_model = OpenAIEmbedding()
+        from guardrails.document_store import EphemeralDocumentStore
 
-                vector_db = Faiss.new_flat_ip_index(
-                    embedding_model.output_dim, embedder=embedding_model
-                )
-            self.store = EphemeralDocumentStore(vector_db)
+        if "vector_db" in metadata:
+            vector_db = metadata["vector_db"]
         else:
-            self.store = document_store
+            from guardrails.vectordb import Faiss
 
-        for doc_path in os.listdir(documents_dir):
-            with open(os.path.join(documents_dir, doc_path)) as f:
-                doc = f.read()
-                self.store.add_text(
-                    doc, {"path": os.path.join(documents_dir, doc_path)}
-                )
+            if "embedding_model" in metadata:
+                embedding_model = metadata["embedding_model"]
+            else:
+                from guardrails.embedding import OpenAIEmbedding
 
-        self._threshold = float(threshold)
+                embedding_model = OpenAIEmbedding()
+
+            vector_db = Faiss.new_flat_ip_index(
+                embedding_model.output_dim, embedder=embedding_model
+            )
+
+        return EphemeralDocumentStore(vector_db)
+
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
+        if "filepaths" not in metadata:
+            raise RuntimeError(
+                "extracted-sentences-summary-match validator expects "
+                "`filepaths` key in metadata"
+            )
+        filepaths = metadata["filepaths"]
+
+        store = self._instantiate_store(metadata)
+
+        sources = []
+        for filepath in filepaths:
+            with open(filepath) as f:
+                doc = f.read()
+                store.add_text(doc, {"path": filepath})
+                sources.append(filepath)
 
-    def validate(self, key, value, schema) -> Dict:
         # Split the value into sentences.
         sentences = re.split(r"(?<=[.!?]) +", value)
 
         # Check if any of the sentences in the value match any of the sentences
         # in the documents.
         unverified = []
         verified = []
-        citations = []
-        for sentence in sentences:
-            page = self.store.search_with_threshold(sentence, self._threshold)
-            if not page:
+        citations = {}
+        for id_, sentence in enumerate(sentences):
+            page = store.search_with_threshold(sentence, self._threshold)
+            if not page or page[0].metadata["path"] not in sources:
                 unverified.append(sentence)
             else:
-                citation_count = len(citations) + 1
-                verified.append(sentence + f" [{citation_count}] ")
-                citations.append(f"\n[{citation_count}] {page[0].metadata['path']}")
-
-        fixed_summary = " ".join(verified) + "\n\n" + "".join(citations)
+                sentence_id = id_ + 1
+                citation_path = page[0].metadata["path"]
+                citation_id = sources.index(citation_path) + 1
+
+                citations[sentence_id] = citation_id
+                verified.append(sentence + f" [{citation_id}]")
+
+        fixed_summary = (
+            " ".join(verified)
+            + "\n\n"
+            + "\n".join(f"[{i + 1}] {s}" for i, s in enumerate(sources))
+        )
+        metadata["summary_with_citations"] = fixed_summary
+        metadata["citations"] = citations
 
         if unverified:
             unverified_sentences = "\n".join(unverified)
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                (
+            return FailResult(
+                metadata=metadata,
+                error_message=(
                     f"The summary \nSummary: {value}\n has sentences\n"
                     f"{unverified_sentences}\n that are not similar to any document."
                 ),
-                fixed_summary,
+                fix_value=fixed_summary,
             )
 
-        schema[key] = fixed_summary
-        return schema
+        return PassResult(metadata=metadata)
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         return ""
 
 
 @register_validator(name="reading-time", data_type="string")
 class ReadingTime(Validator):
     """Validate that the a string can be read in less than a certain amount of
     time."""
 
     def __init__(self, reading_time: int, on_fail: str = "fix"):
         super().__init__(on_fail=on_fail, max_time=reading_time)
         self._max_time = reading_time
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         logger.debug(
             f"Validating {value} can be read in less than {self._max_time} seconds..."
         )
 
         # Estimate the reading time of the string
         reading_time = len(value.split()) / 200 * 60
         logger.debug(f"Estimated reading time {reading_time} seconds...")
 
         if abs(reading_time - self._max_time) > 1:
             logger.error(f"{value} took {reading_time} to read")
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                f"String should be readable within {self._max_time} minutes.",
-                value,
+            return FailResult(
+                error_message=f"String should be readable "
+                f"within {self._max_time} minutes.",
+                fix_value=value,
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="extractive-summary", data_type="string")
 class ExtractiveSummary(Validator):
     """Validate that a string is a valid extractive summary of a given
     document.
 
@@ -1208,32 +1212,38 @@
     After the validation, the summary is updated to include the
     sentences from the document that were matched, and the citations for
     those sentences are added to the end of the summary.
     """
 
     def __init__(
         self,
-        documents_dir: str,
         threshold: int = 85,
         on_fail: Optional[Callable] = None,
         **kwargs,
     ):
         super().__init__(on_fail, **kwargs)
 
         self.threshold = threshold
 
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
+        """Make sure each sentence was precisely copied from the document."""
+
+        if "filepaths" not in metadata:
+            raise RuntimeError(
+                "extractive-summary validator expects " "`filepaths` key in metadata"
+            )
+
+        filepaths = metadata["filepaths"]
+
         # Load documents
-        self._document_store = {}
-        for doc_path in os.listdir(documents_dir):
-            with open(os.path.join(documents_dir, doc_path)) as f:
+        store = {}
+        for filepath in filepaths:
+            with open(filepath) as f:
                 doc = f.read()
-            self._document_store[doc_path] = sentence_split(doc)
-
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
-        """Make sure each sentence was precisely copied from the document."""
+            store[filepath] = sentence_split(doc)
 
         try:
             from thefuzz import fuzz
         except ImportError:
             raise ImportError(
                 "`thefuzz` library is required for `extractive-summary` validator. "
                 "Please install it with `pip install thefuzz`."
@@ -1242,55 +1252,62 @@
         # Split the value into sentences.
         sentences = sentence_split(value)
 
         # Check if any of the sentences in the value match any of the sentences
         # # in the documents.
         unverified = []
         verified = []
-        citations = []
+        citations = {}
 
-        for sentence in sentences:
+        for id_, sentence in enumerate(sentences):
             highest_ratio = 0
             highest_ratio_doc = None
 
             # Check fuzzy match against all sentences in all documents
-            for doc_path, doc_sentences in self._document_store.items():
+            for doc_path, doc_sentences in store.items():
                 for doc_sentence in doc_sentences:
                     ratio = fuzz.ratio(sentence, doc_sentence)
                     if ratio > highest_ratio:
                         highest_ratio = ratio
                         highest_ratio_doc = doc_path
 
             if highest_ratio < self.threshold:
                 unverified.append(sentence)
             else:
-                citation_count = len(citations) + 1
-                verified.append(f"{sentence} [{citation_count}]")
-                citations.append(f"[{citation_count}] {highest_ratio_doc}\n")
+                sentence_id = id_ + 1
+                citation_id = list(store).index(highest_ratio_doc) + 1
+
+                citations[sentence_id] = citation_id
+                verified.append(sentence + f" [{citation_id}]")
+
+        verified_sentences = (
+            " ".join(verified)
+            + "\n\n"
+            + "\n".join(f"[{i + 1}] {s}" for i, s in enumerate(store))
+        )
 
-        verified_sentences = " ".join(verified) + "\n\n" + "".join(citations)
+        metadata["summary_with_citations"] = verified_sentences
+        metadata["citations"] = citations
 
         if len(unverified):
             unverified_sentences = "\n".join(
                 "- " + s for i, s in enumerate(sentences) if i in unverified
             )
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                (
+            return FailResult(
+                metadata=metadata,
+                error_message=(
                     f"The summary \nSummary: {value}\n has sentences\n"
                     f"{unverified_sentences}\n that are not similar to any document."
                 ),
-                verified_sentences,
+                fix_value="\n".join(verified_sentences),
             )
 
-        schema[key] = verified_sentences
-
-        return schema
+        return PassResult(
+            metadata=metadata,
+        )
 
 
 @register_validator(name="remove-redundant-sentences", data_type="string")
 class RemoveRedundantSentences(Validator):
     """Remove redundant sentences from a string.
 
     This validator removes sentences from a string that are similar to
@@ -1300,15 +1317,15 @@
 
     def __init__(
         self, threshold: int = 70, on_fail: Optional[Callable] = None, **kwargs
     ):
         super().__init__(on_fail, **kwargs)
         self.threshold = threshold
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         """Remove redundant sentences from a string."""
 
         try:
             from thefuzz import fuzz
         except ImportError:
             raise ImportError(
                 "`thefuzz` library is required for `remove-redundant-sentences` "
@@ -1337,26 +1354,23 @@
             sentence = unique_sentences[0]
             other_sentences = unique_sentences[1:]
 
         filtered_summary = " ".join(filtered_sentences)
 
         if len(redundant_sentences):
             redundant_sentences = "\n".join(redundant_sentences)
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                (
+            return FailResult(
+                error_message=(
                     f"The summary \nSummary: {value}\n has sentences\n"
                     f"{redundant_sentences}\n that are similar to other sentences."
                 ),
-                filtered_summary,
+                fix_value=filtered_summary,
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="saliency-check", data_type="string")
 class SaliencyCheck(Validator):
     """Check that the summary covers the list of topics present in the
     document."""
 
@@ -1435,34 +1449,31 @@
 </rail>
     """
 
         guard = Guard.from_rail_string(spec)
         _, validated_output = guard(llm_api=self.llm_callable)
         return validated_output["topics"]
 
-    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
         topics_in_summary = self._get_topics(value, topics=self.topics)
 
         # Compute overlap between topics in document and summary
         intersection = set(topics_in_summary).intersection(set(self.topics))
         overlap = len(intersection) / len(self.topics)
 
         if overlap < self.threshold:
-            raise EventDetail(
-                key,
-                value,
-                schema,
-                (
+            return FailResult(
+                error_message=(
                     f"The summary \nSummary: {value}\n does not cover these topics:\n"
                     f"{set(self.topics).difference(intersection)}"
                 ),
-                "",
+                fix_value="",
             )
 
-        return schema
+        return PassResult()
 
 
 @register_validator(name="qa-relevance-llm-eval", data_type="string")
 class QARelevanceLLMEval(Validator):
     def __init__(
         self,
         llm_callable: Callable = None,
@@ -1499,25 +1510,28 @@
 
         return guard(
             self.llm_callable,
             max_tokens=10,
             temperature=0.1,
         )[1]
 
-    def validate(self, key, value, schema) -> Dict:
-        assert "question" in schema, "The schema must contain a `question` key."
+    def validate(self, value: Any, metadata: Dict) -> ValidationResult:
+        if "question" not in metadata:
+            raise RuntimeError(
+                "qa-relevance-llm-eval validator expects " "`question` key in metadata"
+            )
+
+        question = metadata["question"]
 
-        relevant = self.selfeval(schema["question"], value)["relevant"]
+        relevant = self.selfeval(question, value)["relevant"]
         if relevant:
-            return schema
+            return PassResult()
 
         fixed_answer = "No relevant answer found."
-        raise EventDetail(
-            key,
-            value,
-            schema,
-            f"The answer {value} is not relevant to the question {schema['question']}.",
-            fixed_answer,
+        return FailResult(
+            error_message=f"The answer {value} is not relevant "
+            f"to the question {question}.",
+            fix_value=fixed_answer,
         )
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         return ""
```

### Comparing `guardrails-ai-0.1.8/guardrails/vectordb/base.py` & `guardrails-ai-0.2.0a1/guardrails/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails/vectordb/faiss.py` & `guardrails-ai-0.2.0a1/guardrails/vectordb/faiss.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.8/guardrails_ai.egg-info/PKG-INFO` & `guardrails-ai-0.2.0a1/guardrails_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.8
+Version: 0.2.0a1
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `guardrails-ai-0.1.8/guardrails_ai.egg-info/SOURCES.txt` & `guardrails-ai-0.2.0a1/guardrails_ai.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 guardrails/prompt/__init__.py
 guardrails/prompt/base_prompt.py
 guardrails/prompt/instructions.py
 guardrails/prompt/prompt.py
 guardrails/utils/__init__.py
 guardrails/utils/constants.py
 guardrails/utils/docs_utils.py
+guardrails/utils/json_utils.py
 guardrails/utils/logs_utils.py
 guardrails/utils/misc.py
 guardrails/utils/pydantic_utils.py
 guardrails/utils/reask_utils.py
 guardrails/utils/sql_utils.py
 guardrails/vectordb/__init__.py
 guardrails/vectordb/base.py
```

### Comparing `guardrails-ai-0.1.8/setup.py` & `guardrails-ai-0.2.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # What packages are required for this module to be executed?
 REQUIRED = [
     "lxml",
     "openai",
     "rich",
     "eliot",
     "eliot-tree",
-    "pydantic",
+    "pydantic==1.10.9",
     "typer",
     "griffe",
     "tenacity>=8.1.0",
 ]
 
 # Read in docs/requirements.txt
 with open("docs/requirements.txt") as f:
@@ -58,14 +58,15 @@
         "docformatter>=1.4",
         "pytest-cov>=2.10.1",
         "pre-commit>=2.9.3",
         "twine",
         "pytest-mock",
         "pypdfium2",
         "pytest",
+        "pytest-asyncio",
         *SQL_REQUIREMENTS,
         *VECTORDB_REQUIREMENTS,
     ]
     + DOCS_REQUIREMENTS,
     "sql": SQL_REQUIREMENTS,
     "manifest": "manifest-ml",
     "vectordb": VECTORDB_REQUIREMENTS,
```

