# Comparing `tmp/deepgram-sdk-2.8.0.tar.gz` & `tmp/deepgram-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-2.8.0.tar", last modified: Fri Jun 23 16:46:06 2023, max compression
+gzip compressed data, was "deepgram-sdk-2.9.0.tar", last modified: Thu Jul 20 12:18:31 2023, max compression
```

## Comparing `deepgram-sdk-2.8.0.tar` & `deepgram-sdk-2.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/deepgram/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/deepgram/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 16:46:06.000000 deepgram-sdk-2.8.0/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:46:06.280755 deepgram-sdk-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/mock_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-23 16:45:51.000000 deepgram-sdk-2.8.0/tests/test_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:18:31.960115 deepgram-sdk-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-20 12:18:31.960115 deepgram-sdk-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:18:31.956114 deepgram-sdk-2.9.0/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 12:18:17.000000 deepgram-sdk-2.9.0/deepgram/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/deepgram/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:18:31.956114 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-20 12:18:31.000000 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 12:18:31.000000 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:18:31.000000 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 12:18:31.000000 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 12:18:31.000000 deepgram-sdk-2.9.0/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:18:31.960115 deepgram-sdk-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:18:31.960115 deepgram-sdk-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/tests/mock_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/tests/test_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-20 12:18:16.000000 deepgram-sdk-2.9.0/tests/test_transcription.py
```

### Comparing `deepgram-sdk-2.8.0/LICENSE` & `deepgram-sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/PKG-INFO` & `deepgram-sdk-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -87,19 +87,15 @@
 import asyncio
 import aiohttp
 
 # Your Deepgram API Key
 DEEPGRAM_API_KEY = 'YOUR_API_KEY'
 
 # URL for the audio you would like to stream
-# URL for the example resource will change depending on whether user is outside or inside the UK
-# Outside the UK
-URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourlw_online_nonuk'
-# Inside the UK
-# URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourfm'
+URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_world_service'
 
 async def main():
   # Initialize the Deepgram SDK
   deepgram = Deepgram(DEEPGRAM_API_KEY)
 
   # Create a websocket connection to Deepgram
   # In this example, punctuation is turned on, interim results are turned off, and language is set to US English.
```

### Comparing `deepgram-sdk-2.8.0/README.md` & `deepgram-sdk-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,19 +73,15 @@
 import asyncio
 import aiohttp
 
 # Your Deepgram API Key
 DEEPGRAM_API_KEY = 'YOUR_API_KEY'
 
 # URL for the audio you would like to stream
-# URL for the example resource will change depending on whether user is outside or inside the UK
-# Outside the UK
-URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourlw_online_nonuk'
-# Inside the UK
-# URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourfm'
+URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_world_service'
 
 async def main():
   # Initialize the Deepgram SDK
   deepgram = Deepgram(DEEPGRAM_API_KEY)
 
   # Create a websocket connection to Deepgram
   # In this example, punctuation is turned on, interim results are turned off, and language is set to US English.
```

### Comparing `deepgram-sdk-2.8.0/deepgram/__init__.py` & `deepgram-sdk-2.9.0/deepgram/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/_types.py` & `deepgram-sdk-2.9.0/deepgram/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # or cutting-edge options to not break the client for older SDK versions;
 # as such, everything is implemented using TypedDicts
 # instead of, say, dataclasses.
 
 import sys
 from datetime import datetime
 from typing import Optional, List, Union, Any, Dict
+
 if sys.version_info >= (3, 8):
     from typing import TypedDict, Literal
 else:
     from typing_extensions import TypedDict, Literal
 if sys.version_info >= (3, 9, 2):
     from collections.abc import Callable, Awaitable
 else:
@@ -36,32 +37,35 @@
     buffer: bytes
     mimetype: str
 
 
 TranscriptionSource = Union[UrlSource, BufferSource]
 
 
-BoostedKeyword = TypedDict('BoostedKeyword', {
-    'word': str,
-    'boost': float,
-})
+BoostedKeyword = TypedDict(
+    "BoostedKeyword",
+    {
+        "word": str,
+        "boost": float,
+    },
+)
 Keyword = Union[str, BoostedKeyword]
 
 
 class TranscriptionOptions(TypedDict, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
     # https://developers.deepgram.com/documentation/features/
     model: str
     version: str
     language: str
     punctuate: bool
     profanity_filter: bool
     redact: List[str]
-    diarize: Literal['false', 'true']
+    diarize: Literal["false", "true"]
     diarize_version: str
     version: str
     multichannel: bool
     alternatives: int
     # numerals will be deprecated in the future
     numerals: bool
     numbers: bool
@@ -74,26 +78,26 @@
     tier: str
     dates: bool
     date_format: str
     times: bool
     dictation: bool
     measurements: bool
     smart_format: bool
-    replace: str
+    replace: str | List[str]
     tag: List[str]
 
 
 class PrerecordedOptions(TranscriptionOptions, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
     # https://developers.deepgram.com/documentation/features/
     utterances: bool
     utt_split: float
     detect_entities: bool
-    summarize: Union[bool, str] 
+    summarize: Union[bool, str]
     paragraphs: bool
     detect_language: bool
     detect_topics: bool
     translate: List[str]
     analyze_sentiment: bool
     sentiment: bool
     sentiment_threshold: float
@@ -106,17 +110,19 @@
     interim_results: bool
     endpointing: bool
     vad_turnoff: int
     encoding: str
     channels: int
     sample_rate: int
 
+
 class ToggleConfigOptions(TypedDict):
     numerals: bool
 
+
 class WordBase(TypedDict):
     word: str
     start: float
     end: float
     confidence: float
     speaker: Optional[int]
     speaker_confidence: Optional[float]
@@ -204,45 +210,65 @@
     transcript: str
     words: List[WordBase]
     speaker: Optional[int]
     speaker_confidence: Optional[float]
     id: str
 
 
+class Warning(TypedDict):
+    parameter: str
+    type: Literal[
+        "unsupported_language",
+        "unsupported_model",
+        "unsupported_encoding",
+        "deprecated",
+    ]
+    message: str
+
+
 class SummaryV2(TypedDict):
     short: str
+    result: Literal["success", "failure"]
+
 
 class Metadata(TypedDict):
     request_id: str
     transaction_key: str
     sha256: str
     created: str
     duration: float
     channels: int
     models: List[str]
     model_info: Dict[str, Any]
+    warnings: List[Warning]
 
 
-TranscriptionResults = TypedDict('TranscriptionResults', {
-    'channels': List[Channel],
-    'utterances': Optional[List[Utterance]],
-    'summary': Optional[SummaryV2],
-})
+TranscriptionResults = TypedDict(
+    "TranscriptionResults",
+    {
+        "channels": List[Channel],
+        "utterances": Optional[List[Utterance]],
+        "summary": Optional[SummaryV2],
+    },
+)
 
 
 class PrerecordedTranscriptionResponse(TypedDict, total=False):
     request_id: str
     metadata: Metadata
     results: TranscriptionResults
 
 
-StreamingMetadata = TypedDict('StreamingMetadata', {
-    'request_id': str,
-    'model_uuid': str,
-})
+StreamingMetadata = TypedDict(
+    "StreamingMetadata",
+    {
+        "request_id": str,
+        "model_uuid": str,
+    },
+)
 
 
 class LiveTranscriptionResponse(TypedDict):
     channel_index: List[int]
     duration: float
     start: float
     is_final: bool
@@ -260,14 +286,15 @@
 class Key(TypedDict):
     api_key_id: str
     key: Optional[str]
     comment: str
     created: datetime
     scopes: List[str]
 
+
 # Members
 
 
 class Member(TypedDict):
     email: str
     first_name: str
     last_name: str
@@ -300,25 +327,25 @@
 
 
 class UsageRequestListOptions(TypedDict):
     start: Optional[str]
     end: Optional[str]
     page: Optional[int]
     limit: Optional[int]
-    status: Literal['succeeded', 'failed']
+    status: Literal["succeeded", "failed"]
 
 
 class UsageRequestDetails(TypedDict):
     usd: float
     dutation: float
     total_audio: float
     channels: int
     streams: int
     model: str
-    method: Literal['sync', 'async', 'streaming']
+    method: Literal["sync", "async", "streaming"]
     tags: List[str]
     features: List[str]
     config: Dict[str, bool]  # TODO: add all possible request options
 
 
 class UsageRequestDetail(TypedDict):
     details: UsageRequestDetails
@@ -349,32 +376,32 @@
 
 
 class UsageOptions(TypedDict, total=False):
     start: str
     end: str
     accessor: str
     tag: List[str]
-    method: Literal['sync', 'async', 'streaming']
+    method: Literal["sync", "async", "streaming"]
     model: str
     multichannel: bool
     interim_results: bool
     punctuate: bool
     ner: bool
     utterances: bool
-    replace: bool
+    replace: str | List[str]
     profanity_filter: bool
     keywords: bool
     diarize: bool
     detect_language: bool
     search: bool
     redact: bool
     alternatives: bool
     numerals: bool
     detect_entities: bool
-    summarize: Union[bool, str] 
+    summarize: Union[bool, str]
     paragraphs: bool
     detect_language: bool
     detect_topics: bool
     translate: bool
     analyze_sentiment: bool
     sentiment_threshold: float
 
@@ -382,18 +409,17 @@
 class UsageResponseDetail(TypedDict):
     start: str
     end: str
     hours: float
     requests: int
 
 
-UsageResponseResolution = TypedDict("UsageResponseResolution", {
-    'units': str,
-    'amount': int
-})
+UsageResponseResolution = TypedDict(
+    "UsageResponseResolution", {"units": str, "amount": int}
+)
 
 
 class UsageResponse(TypedDict):
     start: str
     end: str
     resolution: UsageResponseResolution
     results: List[UsageResponseDetail]
@@ -407,14 +433,15 @@
 class UsageField(TypedDict):
     tags: List[str]
     models: List[str]
     processing_methods: List[str]
     languages: List[str]
     features: List[str]
 
+
 # Billing
 
 
 class Balance(TypedDict):
     balance_id: str
     amount: float
     units: str
@@ -423,20 +450,22 @@
 
 class BalanceResponse(TypedDict):
     projects: List[Balance]
 
 
 # Scope
 
+
 class Scope(TypedDict):
     scopes: List[str]
 
 
 # Invitation
 
+
 class Invitation(TypedDict):
     email: str
     scope: str
 
 
 class InvitationResponse(TypedDict):
     message: str
```

### Comparing `deepgram-sdk-2.8.0/deepgram/_utils.py` & `deepgram-sdk-2.9.0/deepgram/_utils.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/billing.py` & `deepgram-sdk-2.9.0/deepgram/billing.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/extra.py` & `deepgram-sdk-2.9.0/deepgram/extra.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,24 @@
             warnings.warn(
                 "Enabling the Utterances feature is strongly recommended for captioning. Utterances allow "
                 "captions to be delimited by pauses. Add request parameter `'utterances': True`."
             )
             utterances = response["results"]["channels"][0]["alternatives"]
         captions = []
         line_counter = 1
+        if format is Caption.WEBVTT:
+            captions.append("WEBVTT")
         for utt_index, utt in enumerate(utterances):
             words = utterances[utt_index]["words"]
+            word_text = "punctuated_word" if "punctuated_word" in words[0] else "word"
             for i in range(0, len(words), line_length):
                 start_time = words[i]["start"]
                 end_index = min(len(words) - 1, i + line_length - 1)
                 end_time = words[end_index]["end"]
-                text = " ".join([w["word"] for w in words[i:end_index + 1]])
+                text = " ".join([w[word_text] for w in words[i:end_index + 1]])
                 separator = "," if format is Caption.SRT else '.'
                 prefix = "" if format is Caption.SRT else "- "
                 caption = (
                     f"{line_counter}\n"
                     f"{self._format_timestamp(start_time, separator)} --> "
                     f"{self._format_timestamp(end_time, separator)}\n"
                     f"{prefix}{text}"
```

### Comparing `deepgram-sdk-2.8.0/deepgram/invitations.py` & `deepgram-sdk-2.9.0/deepgram/invitations.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/keys.py` & `deepgram-sdk-2.9.0/deepgram/keys.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/members.py` & `deepgram-sdk-2.9.0/deepgram/members.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/projects.py` & `deepgram-sdk-2.9.0/deepgram/projects.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/scopes.py` & `deepgram-sdk-2.9.0/deepgram/scopes.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/transcription.py` & `deepgram-sdk-2.9.0/deepgram/transcription.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram/usage.py` & `deepgram-sdk-2.9.0/deepgram/usage.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-2.9.0/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -87,19 +87,15 @@
 import asyncio
 import aiohttp
 
 # Your Deepgram API Key
 DEEPGRAM_API_KEY = 'YOUR_API_KEY'
 
 # URL for the audio you would like to stream
-# URL for the example resource will change depending on whether user is outside or inside the UK
-# Outside the UK
-URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourlw_online_nonuk'
-# Inside the UK
-# URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_radio_fourfm'
+URL = 'http://stream.live.vc.bbcmedia.co.uk/bbc_world_service'
 
 async def main():
   # Initialize the Deepgram SDK
   deepgram = Deepgram(DEEPGRAM_API_KEY)
 
   # Create a websocket connection to Deepgram
   # In this example, punctuation is turned on, interim results are turned off, and language is set to US English.
```

### Comparing `deepgram-sdk-2.8.0/deepgram_sdk.egg-info/SOURCES.txt` & `deepgram-sdk-2.9.0/deepgram_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 deepgram_sdk.egg-info/SOURCES.txt
 deepgram_sdk.egg-info/dependency_links.txt
 deepgram_sdk.egg-info/requires.txt
 deepgram_sdk.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/mock_response.py
-tests/test_extra.py
+tests/test_extra.py
+tests/test_transcription.py
```

### Comparing `deepgram-sdk-2.8.0/setup.py` & `deepgram-sdk-2.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 import os.path
 
 # from official Python version-detection recommendations: https://packaging.python.org/guides/single-sourcing-package-version/
 
-with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'deepgram', '_version.py')) as file:
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'deepgram', '_version.py'), encoding="utf8") as file:
     exec(file.read())
 # imports as __version__
 
-with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')) as file:
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding="utf8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name='deepgram-sdk',
     version=__version__, # type: ignore
     description='The official Python SDK for the Deepgram automated speech recognition platform.',
     long_description=long_description,
```

### Comparing `deepgram-sdk-2.8.0/tests/mock_response.py` & `deepgram-sdk-2.9.0/tests/mock_response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.8.0/tests/test_extra.py` & `deepgram-sdk-2.9.0/tests/test_extra.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 api_key = pytest.api_key
 assert api_key, "Pass Deepgram API key as an argument: `pytest --api-key <key> tests/`"
 
 deepgram = Deepgram(api_key)
 
 MOCK_SRT = "1\n00:00:05,519 --> 00:00:06,019\nYep.\n\n2\n00:00:07,094 --> 00:00:08,615\nI said it before, and I'll say it\n\n3\n00:00:08,615 --> 00:00:09,115\nagain.\n\n4\n00:00:09,974 --> 00:00:11,514\nLife moves pretty fast.\n\n5\n00:00:11,974 --> 00:00:13,654\nYou don't stop and look around once in\n\n6\n00:00:13,654 --> 00:00:15,701\na while. you could miss it."
-MOCK_WEBVTT = "1\n00:00:05.519 --> 00:00:06.019\n- Yep.\n\n2\n00:00:07.094 --> 00:00:08.615\n- I said it before, and I'll say it\n\n3\n00:00:08.615 --> 00:00:09.115\n- again.\n\n4\n00:00:09.974 --> 00:00:11.514\n- Life moves pretty fast.\n\n5\n00:00:11.974 --> 00:00:13.654\n- You don't stop and look around once in\n\n6\n00:00:13.654 --> 00:00:15.701\n- a while. you could miss it."
+MOCK_WEBVTT = "WEBVTT\n\n1\n00:00:05.519 --> 00:00:06.019\n- Yep.\n\n2\n00:00:07.094 --> 00:00:08.615\n- I said it before, and I'll say it\n\n3\n00:00:08.615 --> 00:00:09.115\n- again.\n\n4\n00:00:09.974 --> 00:00:11.514\n- Life moves pretty fast.\n\n5\n00:00:11.974 --> 00:00:13.654\n- You don't stop and look around once in\n\n6\n00:00:13.654 --> 00:00:15.701\n- a while. you could miss it."
 
 """
 Happy case of captions in SRT format.
 """
 def test_get_SRT():
     assert deepgram.extra.to_SRT(MOCK_RESPONSE, readable=False) == MOCK_SRT
 
@@ -28,9 +28,9 @@
 
 """
 A response without Utterances cannot be captioned.
 """
 def test_get_SRT_no_utterances():
     response_no_utts = MOCK_RESPONSE
     del response_no_utts["results"]["utterances"]
-    with pytest.raises(AssertionError):
+    with pytest.warns(UserWarning):
         deepgram.extra.to_SRT(response_no_utts)
```

