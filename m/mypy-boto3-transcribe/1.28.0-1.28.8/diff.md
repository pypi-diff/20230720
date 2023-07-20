# Comparing `tmp/mypy-boto3-transcribe-1.28.0.tar.gz` & `tmp/mypy-boto3-transcribe-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.28.0.tar", last modified: Thu Jul  6 21:00:47 2023, max compression
+gzip compressed data, was "mypy-boto3-transcribe-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-transcribe-1.28.0.tar` & `mypy-boto3-transcribe-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.954452 mypy-boto3-transcribe-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:47.954452 mypy-boto3-transcribe-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15165 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.934452 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29715 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29669 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39193 2023-07-06 20:57:19.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39162 2023-07-06 20:57:19.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:47.954452 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:47.000000 mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:47.954452 mypy-boto3-transcribe-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:57:18.000000 mypy-boto3-transcribe-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-07-20 19:47:45.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/setup.py
```

### Comparing `mypy-boto3-transcribe-1.28.0/LICENSE` & `mypy-boto3-transcribe-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.0/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.0
-Summary: Type annotations for boto3.TranscribeService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,14 +292,15 @@
     ParticipantRoleType,
     PiiEntityTypeType,
     RedactionOutputType,
     RedactionTypeType,
     SentimentValueType,
     SpecialtyType,
     SubtitleFormatType,
+    ToxicityCategoryType,
     TranscriptFilterTypeType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyFilterMethodType,
     VocabularyStateType,
     TranscribeServiceServiceName,
     ServiceName,
@@ -317,102 +318,122 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
+    ContentRedactionOutputTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
     SentimentFilterTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
@@ -423,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.0/README.md` & `mypy-boto3-transcribe-1.28.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -260,14 +260,15 @@
     ParticipantRoleType,
     PiiEntityTypeType,
     RedactionOutputType,
     RedactionTypeType,
     SentimentValueType,
     SpecialtyType,
     SubtitleFormatType,
+    ToxicityCategoryType,
     TranscriptFilterTypeType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyFilterMethodType,
     VocabularyStateType,
     TranscribeServiceServiceName,
     ServiceName,
@@ -285,102 +286,122 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
+    ContentRedactionOutputTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
     SentimentFilterTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
@@ -391,15 +412,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/__main__.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.TranscribeService 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/client.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -551,15 +552,16 @@
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
         ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
+        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_transcription_job)
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/client.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     RuleTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -511,15 +512,16 @@
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
         ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
+        LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/client/#start_transcription_job)
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/literals.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "ParticipantRoleType",
     "PiiEntityTypeType",
     "RedactionOutputType",
     "RedactionTypeType",
     "SentimentValueType",
     "SpecialtyType",
     "SubtitleFormatType",
+    "ToxicityCategoryType",
     "TranscriptFilterTypeType",
     "TranscriptionJobStatusType",
     "TypeType",
     "VocabularyFilterMethodType",
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
@@ -113,14 +114,15 @@
     "SSN",
 ]
 RedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
 RedactionTypeType = Literal["PII"]
 SentimentValueType = Literal["MIXED", "NEGATIVE", "NEUTRAL", "POSITIVE"]
 SpecialtyType = Literal["PRIMARYCARE"]
 SubtitleFormatType = Literal["srt", "vtt"]
+ToxicityCategoryType = Literal["ALL"]
 TranscriptFilterTypeType = Literal["EXACT"]
 TranscriptionJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
 TypeType = Literal["CONVERSATION", "DICTATION"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VocabularyStateType = Literal["FAILED", "PENDING", "READY"]
 TranscribeServiceServiceName = Literal["transcribe"]
 ServiceName = Literal[
@@ -336,14 +338,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/literals.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "ParticipantRoleType",
     "PiiEntityTypeType",
     "RedactionOutputType",
     "RedactionTypeType",
     "SentimentValueType",
     "SpecialtyType",
     "SubtitleFormatType",
+    "ToxicityCategoryType",
     "TranscriptFilterTypeType",
     "TranscriptionJobStatusType",
     "TypeType",
     "VocabularyFilterMethodType",
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
@@ -111,14 +112,15 @@
     "SSN",
 ]
 RedactionOutputType = Literal["redacted", "redacted_and_unredacted"]
 RedactionTypeType = Literal["PII"]
 SentimentValueType = Literal["MIXED", "NEGATIVE", "NEUTRAL", "POSITIVE"]
 SpecialtyType = Literal["PRIMARYCARE"]
 SubtitleFormatType = Literal["srt", "vtt"]
+ToxicityCategoryType = Literal["ALL"]
 TranscriptFilterTypeType = Literal["EXACT"]
 TranscriptionJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
 TypeType = Literal["CONVERSATION", "DICTATION"]
 VocabularyFilterMethodType = Literal["mask", "remove", "tag"]
 VocabularyStateType = Literal["FAILED", "PENDING", "READY"]
 TranscribeServiceServiceName = Literal["transcribe"]
 ServiceName = Literal[
@@ -334,14 +336,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/type_defs.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -42,102 +42,122 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
+    "ContentRedactionOutputTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
     "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
-    "GetVocabularyResponseTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
-    "ResponseMetadataTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "UpdateVocabularyResponseTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
+    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
     "SentimentFilterTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
@@ -147,36 +167,64 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
+    {
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+        "PiiEntityTypes": List[PiiEntityTypeType],
+    },
+)
+
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+)
+
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
 _OptionalContentRedactionTypeDef = TypedDict(
     "_OptionalContentRedactionTypeDef",
     {
-        "PiiEntityTypes": List[PiiEntityTypeType],
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
     },
     total=False,
 )
 
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
@@ -199,44 +247,60 @@
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -257,45 +321,20 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
     },
 )
 
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
@@ -354,21 +393,14 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -389,83 +421,64 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
     {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
     },
 )
 
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -473,15 +486,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -533,15 +545,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -555,24 +566,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -604,23 +622,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -628,30 +665,40 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
     },
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
@@ -671,22 +718,35 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": Sequence[Literal["ALL"]],
+    },
+)
+
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
+)
+
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -698,25 +758,14 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -733,24 +782,14 @@
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -767,75 +806,159 @@
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": Sequence[LanguageCodeType],
+        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
     {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
     {
-        "ModelName": str,
-        "CreateTime": datetime,
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
@@ -930,28 +1053,90 @@
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
+    {
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+    },
+)
+
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
+    {
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "Negate": bool,
+    },
+)
+
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
+    {
+        "Threshold": int,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "Negate": bool,
+    },
+)
+
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+)
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+        "Targets": List[str],
     },
 )
 
 InterruptionFilterTypeDef = TypedDict(
     "InterruptionFilterTypeDef",
     {
         "Threshold": int,
@@ -1021,68 +1206,76 @@
 
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1111,35 +1304,14 @@
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1159,76 +1331,97 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
+    },
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1254,24 +1447,34 @@
     pass
 
 
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
+        "TranscriptFilter": TranscriptFilterOutputTypeDef,
+        "SentimentFilter": SentimentFilterOutputTypeDef,
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
@@ -1282,78 +1485,77 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
@@ -1398,35 +1600,35 @@
     pass
 
 
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "GetCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
         "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe/type_defs.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -41,102 +41,122 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
+    "ContentRedactionOutputTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
     "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
+    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
-    "GetVocabularyResponseTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
-    "ResponseMetadataTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
+    "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
+    "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "UpdateVocabularyResponseTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
+    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
     "SentimentFilterTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
-    "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
+    "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
@@ -146,36 +166,64 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
+    {
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+        "PiiEntityTypes": List[PiiEntityTypeType],
+    },
+)
+
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+)
+
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
 _OptionalContentRedactionTypeDef = TypedDict(
     "_OptionalContentRedactionTypeDef",
     {
-        "PiiEntityTypes": List[PiiEntityTypeType],
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
     },
     total=False,
 )
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
@@ -196,44 +244,60 @@
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -252,45 +316,20 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
     {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
     },
 )
 
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
@@ -349,21 +388,14 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -384,83 +416,64 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
     {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
     },
 )
 
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -468,15 +481,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -528,15 +540,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -550,24 +561,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -599,23 +617,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -623,30 +660,40 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
     },
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
@@ -666,22 +713,35 @@
     {
         "Formats": Sequence[SubtitleFormatType],
         "OutputStartIndex": int,
     },
     total=False,
 )
 
+ToxicityDetectionSettingsTypeDef = TypedDict(
+    "ToxicityDetectionSettingsTypeDef",
+    {
+        "ToxicityCategories": Sequence[Literal["ALL"]],
+    },
+)
+
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
+)
+
+ToxicityDetectionSettingsOutputTypeDef = TypedDict(
+    "ToxicityDetectionSettingsOutputTypeDef",
+    {
+        "ToxicityCategories": List[Literal["ALL"]],
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -693,25 +753,14 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -726,24 +775,14 @@
 
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -758,75 +797,159 @@
 )
 
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": Sequence[LanguageCodeType],
+        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
     {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
     {
-        "ModelName": str,
-        "CreateTime": datetime,
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
@@ -913,28 +1036,90 @@
 )
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
+    {
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+    },
+)
+
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
+    {
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "Negate": bool,
+    },
+)
+
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
+    {
+        "Threshold": int,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "Negate": bool,
+    },
+)
+
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+)
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+        "Targets": List[str],
     },
 )
 
 InterruptionFilterTypeDef = TypedDict(
     "InterruptionFilterTypeDef",
     {
         "Threshold": int,
@@ -1000,68 +1185,76 @@
 
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1088,35 +1281,14 @@
 
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
-TranscriptionJobSummaryTypeDef = TypedDict(
-    "TranscriptionJobSummaryTypeDef",
-    {
-        "TranscriptionJobName": str,
-        "CreationTime": datetime,
-        "StartTime": datetime,
-        "CompletionTime": datetime,
-        "LanguageCode": LanguageCodeType,
-        "TranscriptionJobStatus": TranscriptionJobStatusType,
-        "FailureReason": str,
-        "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "IdentifyLanguage": bool,
-        "IdentifyMultipleLanguages": bool,
-        "IdentifiedLanguageScore": float,
-        "LanguageCodes": List[LanguageCodeItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredStartTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1136,74 +1308,95 @@
         "ContentRedaction": ContentRedactionTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": Sequence[LanguageCodeType],
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "ToxicityDetection": Sequence[ToxicityDetectionSettingsTypeDef],
     },
     total=False,
 )
 
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
+TranscriptionJobSummaryTypeDef = TypedDict(
+    "TranscriptionJobSummaryTypeDef",
+    {
+        "TranscriptionJobName": str,
+        "CreationTime": datetime,
+        "StartTime": datetime,
+        "CompletionTime": datetime,
+        "LanguageCode": LanguageCodeType,
+        "TranscriptionJobStatus": TranscriptionJobStatusType,
+        "FailureReason": str,
+        "OutputLocationType": OutputLocationTypeType,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "IdentifyLanguage": bool,
+        "IdentifyMultipleLanguages": bool,
+        "IdentifiedLanguageScore": float,
+        "LanguageCodes": List[LanguageCodeItemTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
+    },
+)
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
+        "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1227,24 +1420,34 @@
 ):
     pass
 
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
+        "TranscriptFilter": TranscriptFilterOutputTypeDef,
+        "SentimentFilter": SentimentFilterOutputTypeDef,
     },
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
@@ -1255,78 +1458,77 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
@@ -1367,35 +1569,35 @@
 ):
     pass
 
 CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "CreateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "GetCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesResponseTypeDef",
     {
         "NextToken": str,
         "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
     "UpdateCallAnalyticsCategoryResponseTypeDef",
     {
         "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.0
-Summary: Type annotations for boto3.TranscribeService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,14 +292,15 @@
     ParticipantRoleType,
     PiiEntityTypeType,
     RedactionOutputType,
     RedactionTypeType,
     SentimentValueType,
     SpecialtyType,
     SubtitleFormatType,
+    ToxicityCategoryType,
     TranscriptFilterTypeType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyFilterMethodType,
     VocabularyStateType,
     TranscribeServiceServiceName,
     ServiceName,
@@ -317,102 +318,122 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
+    ContentRedactionOutputTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
     LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
+    ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
+    ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
     SentimentFilterTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
-    TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
+    TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
@@ -423,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.0/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.0/setup.py` & `mypy-boto3-transcribe-1.28.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TranscribeService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.TranscribeService 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

