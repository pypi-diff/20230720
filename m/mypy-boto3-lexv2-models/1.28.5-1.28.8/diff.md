# Comparing `tmp/mypy-boto3-lexv2-models-1.28.5.tar.gz` & `tmp/mypy-boto3-lexv2-models-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-models-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-models-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-lexv2-models-1.28.5.tar` & `mypy-boto3-lexv2-models-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37086 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35582 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73416 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19542 2023-07-18 19:32:20.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    19540 2023-07-18 19:32:20.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   196677 2023-07-18 19:32:24.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   196483 2023-07-18 19:32:22.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37086 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-lexv2-models-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-07-20 19:47:56.016775 mypy-boto3-lexv2-models-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35558 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73297 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73190 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-20 19:46:57.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-07-20 19:46:57.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   196451 2023-07-20 19:47:02.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   196257 2023-07-20 19:46:59.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-lexv2-models-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-20 19:46:56.000000 mypy-boto3-lexv2-models-1.28.8/setup.py
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/LICENSE` & `mypy-boto3-lexv2-models-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/PKG-INFO` & `mypy-boto3-lexv2-models-1.28.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-models
-Version: 1.28.5
-Summary: Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.8
+Summary: Type annotations for boto3.LexModelsV2 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -346,15 +346,14 @@
     AnalyticsUtteranceMetricNameType,
     AnalyticsUtteranceSortByNameType,
     AssociatedTranscriptFilterNameType,
     AudioRecognitionStrategyType,
     BotAliasAvailableWaiterName,
     BotAliasStatusType,
     BotAvailableWaiterName,
-    BotChannelTypeType,
     BotExportCompletedWaiterName,
     BotFilterNameType,
     BotFilterOperatorType,
     BotImportCompletedWaiterName,
     BotLocaleBuiltWaiterName,
     BotLocaleCreatedWaiterName,
     BotLocaleExpressTestingAvailableWaiterName,
@@ -485,14 +484,15 @@
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationOutputTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemOutputTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     CustomVocabularyItemTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetOutputTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationOutputTypeDef,
@@ -516,15 +516,14 @@
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsOutputTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonOutputTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationOutputTypeDef,
@@ -550,90 +549,74 @@
     SampleUtteranceTypeDef,
     DialogCodeHookSettingsOutputTypeDef,
     InputContextOutputTypeDef,
     KendraConfigurationOutputTypeDef,
     OutputContextOutputTypeDef,
     SampleUtteranceOutputTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
     MultipleValuesSettingOutputTypeDef,
     ObfuscationSettingOutputTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadOutputTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationOutputTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationOutputTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
     DateRangeFilterOutputTypeDef,
     DateRangeFilterTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingOutputTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityOutputTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationOutputTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingOutputTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationOutputTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceOutputTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
@@ -648,15 +631,14 @@
     SessionDataSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     UtteranceDataSortByTypeDef,
     PlainTextMessageOutputTypeDef,
     SSMLMessageOutputTypeDef,
     PlainTextMessageTypeDef,
@@ -664,66 +646,83 @@
     OverallTestResultItemTypeDef,
     PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationOutputTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationOutputTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueOutputTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
     SlotPriorityTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueOutputTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterOutputTypeDef,
     SlotValueRegexFilterTypeDef,
     TestSetStorageLocationTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationOutputTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     AnalyticsIntentResultTypeDef,
     ListIntentMetricsRequestRequestTypeDef,
-    ListIntentPathsResponseTypeDef,
     AnalyticsIntentStageResultTypeDef,
     ListIntentStageMetricsRequestRequestTypeDef,
     ListIntentPathsRequestRequestTypeDef,
     AnalyticsSessionResultTypeDef,
     ListSessionMetricsRequestRequestTypeDef,
     AnalyticsUtteranceResultTypeDef,
     ListUtteranceMetricsRequestRequestTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationOutputTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationOutputTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetOutputTypeDef,
     TestExecutionTargetTypeDef,
     BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/README.md` & `mypy-boto3-lexv2-models-1.28.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -314,15 +314,14 @@
     AnalyticsUtteranceMetricNameType,
     AnalyticsUtteranceSortByNameType,
     AssociatedTranscriptFilterNameType,
     AudioRecognitionStrategyType,
     BotAliasAvailableWaiterName,
     BotAliasStatusType,
     BotAvailableWaiterName,
-    BotChannelTypeType,
     BotExportCompletedWaiterName,
     BotFilterNameType,
     BotFilterOperatorType,
     BotImportCompletedWaiterName,
     BotLocaleBuiltWaiterName,
     BotLocaleCreatedWaiterName,
     BotLocaleExpressTestingAvailableWaiterName,
@@ -453,14 +452,15 @@
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationOutputTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemOutputTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     CustomVocabularyItemTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetOutputTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationOutputTypeDef,
@@ -484,15 +484,14 @@
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsOutputTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonOutputTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationOutputTypeDef,
@@ -518,90 +517,74 @@
     SampleUtteranceTypeDef,
     DialogCodeHookSettingsOutputTypeDef,
     InputContextOutputTypeDef,
     KendraConfigurationOutputTypeDef,
     OutputContextOutputTypeDef,
     SampleUtteranceOutputTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
     MultipleValuesSettingOutputTypeDef,
     ObfuscationSettingOutputTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadOutputTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationOutputTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationOutputTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
     DateRangeFilterOutputTypeDef,
     DateRangeFilterTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingOutputTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityOutputTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationOutputTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingOutputTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationOutputTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceOutputTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
@@ -616,15 +599,14 @@
     SessionDataSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     UtteranceDataSortByTypeDef,
     PlainTextMessageOutputTypeDef,
     SSMLMessageOutputTypeDef,
     PlainTextMessageTypeDef,
@@ -632,66 +614,83 @@
     OverallTestResultItemTypeDef,
     PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationOutputTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationOutputTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueOutputTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
     SlotPriorityTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueOutputTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterOutputTypeDef,
     SlotValueRegexFilterTypeDef,
     TestSetStorageLocationTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationOutputTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     AnalyticsIntentResultTypeDef,
     ListIntentMetricsRequestRequestTypeDef,
-    ListIntentPathsResponseTypeDef,
     AnalyticsIntentStageResultTypeDef,
     ListIntentStageMetricsRequestRequestTypeDef,
     ListIntentPathsRequestRequestTypeDef,
     AnalyticsSessionResultTypeDef,
     ListSessionMetricsRequestRequestTypeDef,
     AnalyticsUtteranceResultTypeDef,
     ListUtteranceMetricsRequestRequestTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationOutputTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationOutputTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetOutputTypeDef,
     TestExecutionTargetTypeDef,
     BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.pyi` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__main__.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelsV2 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        "Type annotations for boto3.LexModelsV2 1.28.8\nVersion:         1.28.8\nBuilder version:"
         " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.5")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1064,15 +1064,15 @@
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListIntentStageMetricsResponseTypeDef:
         """
-        Retrieves summary metrics for the intent stages in your bot.
+        Retrieves summary metrics for the stages within intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_stage_metrics)
         """
 
     def list_intents(
         self,
@@ -1251,15 +1251,15 @@
         endDateTime: Union[datetime, str],
         sortBy: UtteranceDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListUtteranceAnalyticsDataResponseTypeDef:
         """
-        Retrieves a list of metadata for individual user utterances to your bot.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_analytics_data)
         """
 
     def list_utterance_metrics(
         self,
@@ -1272,15 +1272,15 @@
         groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
         attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListUtteranceMetricsResponseTypeDef:
         """
-        Retrieves summary metrics for the utterances in your bot.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_metrics)
         """
 
     def search_associated_transcripts(
         self,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.pyi` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -996,15 +996,15 @@
         binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
         groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
         filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListIntentStageMetricsResponseTypeDef:
         """
-        Retrieves summary metrics for the intent stages in your bot.
+        Retrieves summary metrics for the stages within intents in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_stage_metrics)
         """
     def list_intents(
         self,
         *,
@@ -1171,15 +1171,15 @@
         endDateTime: Union[datetime, str],
         sortBy: UtteranceDataSortByTypeDef = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListUtteranceAnalyticsDataResponseTypeDef:
         """
-        Retrieves a list of metadata for individual user utterances to your bot.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_analytics_data)
         """
     def list_utterance_metrics(
         self,
         *,
@@ -1191,15 +1191,15 @@
         groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
         attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
         filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListUtteranceMetricsResponseTypeDef:
         """
-        Retrieves summary metrics for the utterances in your bot.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_metrics)
         """
     def search_associated_transcripts(
         self,
         *,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "AnalyticsUtteranceMetricNameType",
     "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
-    "BotChannelTypeType",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
     "BotFilterOperatorType",
     "BotImportCompletedWaiterName",
     "BotLocaleBuiltWaiterName",
     "BotLocaleCreatedWaiterName",
     "BotLocaleExpressTestingAvailableWaiterName",
@@ -202,15 +201,14 @@
 AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
 AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
-BotChannelTypeType = Literal["Facebook", "Slack", "TwilioSms"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
 BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
@@ -540,14 +538,15 @@
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

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.pyi` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "AnalyticsUtteranceMetricNameType",
     "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
-    "BotChannelTypeType",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
     "BotFilterOperatorType",
     "BotImportCompletedWaiterName",
     "BotLocaleBuiltWaiterName",
     "BotLocaleCreatedWaiterName",
     "BotLocaleExpressTestingAvailableWaiterName",
@@ -200,15 +199,14 @@
 AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
 AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
-BotChannelTypeType = Literal["Facebook", "Slack", "TwilioSms"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
 BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
@@ -538,14 +536,15 @@
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

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     AnalyticsSessionSortByNameType,
     AnalyticsSortOrderType,
     AnalyticsUtteranceFieldType,
     AnalyticsUtteranceFilterNameType,
     AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
-    BotChannelTypeType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
@@ -149,14 +148,15 @@
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationOutputTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemOutputTypeDef",
     "FailedCustomVocabularyItemTypeDef",
+    "ResponseMetadataTypeDef",
     "CustomVocabularyEntryIdTypeDef",
     "CustomVocabularyItemTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
     "BotAliasTestExecutionTargetOutputTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
     "BotExportSpecificationOutputTypeDef",
@@ -180,15 +180,14 @@
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsOutputTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
-    "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
     "ButtonOutputTypeDef",
     "ButtonTypeDef",
     "CloudWatchLogGroupLogDestinationOutputTypeDef",
@@ -214,90 +213,74 @@
     "SampleUtteranceTypeDef",
     "DialogCodeHookSettingsOutputTypeDef",
     "InputContextOutputTypeDef",
     "KendraConfigurationOutputTypeDef",
     "OutputContextOutputTypeDef",
     "SampleUtteranceOutputTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
-    "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
-    "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
     "MultipleValuesSettingOutputTypeDef",
     "ObfuscationSettingOutputTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "CustomPayloadOutputTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationOutputTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationOutputTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
     "DateRangeFilterOutputTypeDef",
     "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
-    "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
-    "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
-    "DeleteBotResponseTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
-    "DeleteBotVersionResponseTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
-    "DeleteCustomVocabularyResponseTypeDef",
     "DeleteExportRequestRequestTypeDef",
-    "DeleteExportResponseTypeDef",
     "DeleteImportRequestRequestTypeDef",
-    "DeleteImportResponseTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
-    "DeleteResourcePolicyStatementResponseTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingOutputTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
     "SlotPriorityOutputTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationOutputTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingOutputTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionSettingTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationOutputTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
     "GrammarSlotTypeSourceOutputTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
@@ -312,15 +295,14 @@
     "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
     "UtteranceDataSortByTypeDef",
     "PlainTextMessageOutputTypeDef",
     "SSMLMessageOutputTypeDef",
     "PlainTextMessageTypeDef",
@@ -328,66 +310,83 @@
     "OverallTestResultItemTypeDef",
     "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationOutputTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationOutputTypeDef",
     "RelativeAggregationDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueOutputTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotPriorityTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
     "SlotValueOutputTypeDef",
     "SlotValueTypeDef",
     "SlotValueRegexFilterOutputTypeDef",
     "SlotValueRegexFilterTypeDef",
     "TestSetStorageLocationTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
-    "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     "TestSetImportInputLocationOutputTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
-    "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
     "AnalyticsIntentResultTypeDef",
     "ListIntentMetricsRequestRequestTypeDef",
-    "ListIntentPathsResponseTypeDef",
     "AnalyticsIntentStageResultTypeDef",
     "ListIntentStageMetricsRequestRequestTypeDef",
     "ListIntentPathsRequestRequestTypeDef",
     "AnalyticsSessionResultTypeDef",
     "ListSessionMetricsRequestRequestTypeDef",
     "AnalyticsUtteranceResultTypeDef",
     "ListUtteranceMetricsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
-    "SearchAssociatedTranscriptsResponseTypeDef",
     "AudioAndDTMFInputSpecificationOutputTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationOutputTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
-    "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
+    "BuildBotLocaleResponseTypeDef",
+    "CreateResourcePolicyResponseTypeDef",
+    "CreateResourcePolicyStatementResponseTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "DeleteBotAliasResponseTypeDef",
+    "DeleteBotLocaleResponseTypeDef",
+    "DeleteBotResponseTypeDef",
+    "DeleteBotVersionResponseTypeDef",
+    "DeleteCustomVocabularyResponseTypeDef",
+    "DeleteExportResponseTypeDef",
+    "DeleteImportResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "ListCustomVocabularyItemsResponseTypeDef",
+    "ListIntentPathsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    "StopBotRecommendationResponseTypeDef",
+    "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetOutputTypeDef",
     "TestExecutionTargetTypeDef",
     "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
@@ -1119,14 +1118,25 @@
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
     },
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
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
@@ -1419,26 +1429,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-BuildBotLocaleResponseTypeDef = TypedDict(
-    "BuildBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "lastBuildSubmittedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuiltInIntentSortByTypeDef = TypedDict(
     "BuiltInIntentSortByTypeDef",
     {
         "attribute": Literal["IntentSignature"],
         "order": SortOrderType,
     },
 )
@@ -1705,41 +1703,23 @@
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
 
-CreateResourcePolicyResponseTypeDef = TypedDict(
-    "CreateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "service": str,
         "arn": str,
     },
     total=False,
 )
 
-CreateResourcePolicyStatementResponseTypeDef = TypedDict(
-    "CreateResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MultipleValuesSettingTypeDef = TypedDict(
     "MultipleValuesSettingTypeDef",
     {
         "allowMultipleValues": bool,
     },
     total=False,
 )
@@ -1761,23 +1741,14 @@
 ObfuscationSettingOutputTypeDef = TypedDict(
     "ObfuscationSettingOutputTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "importId": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomPayloadOutputTypeDef = TypedDict(
     "CustomPayloadOutputTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1858,44 +1829,23 @@
 
 class DeleteBotAliasRequestRequestTypeDef(
     _RequiredDeleteBotAliasRequestRequestTypeDef, _OptionalDeleteBotAliasRequestRequestTypeDef
 ):
     pass
 
 
-DeleteBotAliasResponseTypeDef = TypedDict(
-    "DeleteBotAliasResponseTypeDef",
-    {
-        "botAliasId": str,
-        "botId": str,
-        "botAliasStatus": BotAliasStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBotLocaleRequestRequestTypeDef = TypedDict(
     "DeleteBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteBotLocaleResponseTypeDef = TypedDict(
-    "DeleteBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDeleteBotRequestRequestTypeDef = TypedDict(
@@ -1909,23 +1859,14 @@
 
 class DeleteBotRequestRequestTypeDef(
     _RequiredDeleteBotRequestRequestTypeDef, _OptionalDeleteBotRequestRequestTypeDef
 ):
     pass
 
 
-DeleteBotResponseTypeDef = TypedDict(
-    "DeleteBotResponseTypeDef",
-    {
-        "botId": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -1940,76 +1881,37 @@
 
 class DeleteBotVersionRequestRequestTypeDef(
     _RequiredDeleteBotVersionRequestRequestTypeDef, _OptionalDeleteBotVersionRequestRequestTypeDef
 ):
     pass
 
 
-DeleteBotVersionResponseTypeDef = TypedDict(
-    "DeleteBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCustomVocabularyRequestRequestTypeDef = TypedDict(
     "DeleteCustomVocabularyRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteCustomVocabularyResponseTypeDef = TypedDict(
-    "DeleteCustomVocabularyResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExportRequestRequestTypeDef = TypedDict(
     "DeleteExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-DeleteExportResponseTypeDef = TypedDict(
-    "DeleteExportResponseTypeDef",
-    {
-        "exportId": str,
-        "exportStatus": ExportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImportRequestRequestTypeDef = TypedDict(
     "DeleteImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-DeleteImportResponseTypeDef = TypedDict(
-    "DeleteImportResponseTypeDef",
-    {
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIntentRequestRequestTypeDef = TypedDict(
     "DeleteIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2034,23 +1936,14 @@
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
     },
 )
@@ -2066,23 +1959,14 @@
 class DeleteResourcePolicyStatementRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSlotRequestRequestTypeDef = TypedDict(
     "DeleteSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2216,27 +2100,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExportRequestRequestTypeDef = TypedDict(
     "DescribeExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
@@ -2268,24 +2139,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSlotRequestRequestTypeDef = TypedDict(
     "DescribeSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2412,21 +2273,14 @@
 class ElicitationCodeHookInvocationSettingTypeDef(
     _RequiredElicitationCodeHookInvocationSettingTypeDef,
     _OptionalElicitationCodeHookInvocationSettingTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionSettingTypeDef = TypedDict(
     "EncryptionSettingTypeDef",
     {
         "kmsKeyArn": str,
         "botLocaleExportPassword": str,
         "associatedTranscriptsPassword": str,
     },
@@ -2467,23 +2321,14 @@
 GetTestExecutionArtifactsUrlRequestRequestTypeDef = TypedDict(
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     {
         "testExecutionId": str,
     },
 )
 
-GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
-    {
-        "testExecutionId": str,
-        "downloadArtifactsUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrammarSlotTypeSourceOutputTypeDef = TypedDict(
     "GrammarSlotTypeSourceOutputTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
         "kmsKeyArn": str,
     },
@@ -2746,22 +2591,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TestExecutionSortByTypeDef = TypedDict(
     "TestExecutionSortByTypeDef",
     {
         "attribute": TestExecutionSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2884,25 +2721,14 @@
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -3008,26 +2834,14 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-StopBotRecommendationResponseTypeDef = TypedDict(
-    "StopBotRecommendationResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationStatus": BotRecommendationStatusType,
-        "botRecommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -3131,23 +2945,14 @@
 class UpdateResourcePolicyRequestRequestTypeDef(
     _RequiredUpdateResourcePolicyRequestRequestTypeDef,
     _OptionalUpdateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateResourcePolicyResponseTypeDef = TypedDict(
-    "UpdateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTestSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
     },
 )
@@ -3234,22 +3039,14 @@
 
 class ListIntentMetricsRequestRequestTypeDef(
     _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
 ):
     pass
 
 
-ListIntentPathsResponseTypeDef = TypedDict(
-    "ListIntentPathsResponseTypeDef",
-    {
-        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnalyticsIntentStageResultTypeDef = TypedDict(
     "AnalyticsIntentStageResultTypeDef",
     {
         "binKeys": List[AnalyticsBinKeyTypeDef],
         "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
         "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
     },
@@ -3410,28 +3207,14 @@
 class SearchAssociatedTranscriptsRequestRequestTypeDef(
     _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef,
     _OptionalSearchAssociatedTranscriptsRequestRequestTypeDef,
 ):
     pass
 
 
-SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
-    "SearchAssociatedTranscriptsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "nextIndex": int,
-        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
-        "totalResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AudioAndDTMFInputSpecificationOutputTypeDef = TypedDict(
     "AudioAndDTMFInputSpecificationOutputTypeDef",
     {
         "startTimeoutMs": int,
         "audioSpecification": AudioSpecificationOutputTypeDef,
         "dtmfSpecification": DTMFSpecificationOutputTypeDef,
     },
@@ -3479,59 +3262,275 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[NewCustomVocabularyItemTypeDef],
     },
 )
 
-ListCustomVocabularyItemsResponseTypeDef = TypedDict(
-    "ListCustomVocabularyItemsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BuildBotLocaleResponseTypeDef = TypedDict(
+    "BuildBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "lastBuildSubmittedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyResponseTypeDef = TypedDict(
+    "CreateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyStatementResponseTypeDef = TypedDict(
+    "CreateResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "importId": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotAliasResponseTypeDef = TypedDict(
+    "DeleteBotAliasResponseTypeDef",
+    {
+        "botAliasId": str,
+        "botId": str,
+        "botAliasStatus": BotAliasStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotLocaleResponseTypeDef = TypedDict(
+    "DeleteBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotResponseTypeDef = TypedDict(
+    "DeleteBotResponseTypeDef",
+    {
+        "botId": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotVersionResponseTypeDef = TypedDict(
+    "DeleteBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomVocabularyResponseTypeDef = TypedDict(
+    "DeleteCustomVocabularyResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExportResponseTypeDef = TypedDict(
+    "DeleteExportResponseTypeDef",
+    {
+        "exportId": str,
+        "exportStatus": ExportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImportResponseTypeDef = TypedDict(
+    "DeleteImportResponseTypeDef",
+    {
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "policy": str,
+        "revisionId": str,
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
+GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    {
+        "testExecutionId": str,
+        "downloadArtifactsUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVocabularyItemsResponseTypeDef = TypedDict(
+    "ListCustomVocabularyItemsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "nextIndex": int,
+        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
+        "totalResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopBotRecommendationResponseTypeDef = TypedDict(
+    "StopBotRecommendationResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationStatus": BotRecommendationStatusType,
+        "botRecommendationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourcePolicyResponseTypeDef = TypedDict(
+    "UpdateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
@@ -3553,15 +3552,15 @@
 
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionTargetOutputTypeDef = TypedDict(
     "TestExecutionTargetOutputTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetOutputTypeDef,
@@ -3632,15 +3631,15 @@
         "localeName": str,
         "localeId": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsOutputTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotLocaleResponseTypeDef = TypedDict(
     "DescribeBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -3655,15 +3654,15 @@
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
         "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotLocaleResponseTypeDef = TypedDict(
     "UpdateBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -3674,15 +3673,15 @@
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsOutputTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
@@ -3784,15 +3783,15 @@
 ListBotLocalesResponseTypeDef = TypedDict(
     "ListBotLocalesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
@@ -3803,15 +3802,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
@@ -3822,15 +3821,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "botId": str,
@@ -3840,15 +3839,15 @@
         "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "botName": str,
@@ -3915,15 +3914,15 @@
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationSummaries": List[BotRecommendationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsRequestRequestTypeDef = TypedDict(
     "ListBotsRequestRequestTypeDef",
     {
         "sortBy": BotSortByTypeDef,
@@ -3935,28 +3934,28 @@
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "botId": str,
         "description": str,
         "botVersion": str,
         "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsOutputTypeDef],
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
@@ -4003,15 +4002,15 @@
 
 ListBotVersionsResponseTypeDef = TypedDict(
     "ListBotVersionsResponseTypeDef",
     {
         "botId": str,
         "botVersionSummaries": List[BotVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInIntentsRequestRequestTypeDef",
     {
         "localeId": str,
@@ -4037,15 +4036,15 @@
 
 ListBuiltInIntentsResponseTypeDef = TypedDict(
     "ListBuiltInIntentsResponseTypeDef",
     {
         "builtInIntentSummaries": List[BuiltInIntentSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInSlotTypesRequestRequestTypeDef",
     {
         "localeId": str,
@@ -4071,15 +4070,15 @@
 
 ListBuiltInSlotTypesResponseTypeDef = TypedDict(
     "ListBuiltInSlotTypesResponseTypeDef",
     {
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageResponseCardOutputTypeDef = TypedDict(
     "ImageResponseCardOutputTypeDef",
     {
         "title": str,
@@ -4458,15 +4457,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetResponseTypeDef = TypedDict(
     "DescribeTestSetResponseTypeDef",
     {
         "testSetId": str,
@@ -4475,15 +4474,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
     "TestSetSummaryTypeDef",
     {
         "testSetId": str,
@@ -4508,15 +4507,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DialogStateOutputTypeDef = TypedDict(
     "DialogStateOutputTypeDef",
     {
         "dialogAction": DialogActionOutputTypeDef,
@@ -4614,15 +4613,15 @@
     "ListImportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "importSummaries": List[ImportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
@@ -4668,15 +4667,15 @@
 
 SessionSpecificationTypeDef = TypedDict(
     "SessionSpecificationTypeDef",
     {
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
-        "channel": BotChannelTypeType,
+        "channel": str,
         "sessionId": str,
         "conversationStartTime": datetime,
         "conversationEndTime": datetime,
         "conversationDurationSeconds": int,
         "conversationEndState": ConversationEndStateType,
         "mode": AnalyticsModalityType,
         "numberOfTurns": int,
@@ -4690,15 +4689,15 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
     {
         "botId": str,
@@ -4755,15 +4754,15 @@
     "ListSlotTypesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "slotTypeSummaries": List[SlotTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotsRequestRequestTypeDef",
     {
         "botId": str,
@@ -5037,45 +5036,45 @@
 
 ListIntentMetricsResponseTypeDef = TypedDict(
     "ListIntentMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsIntentResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntentStageMetricsResponseTypeDef = TypedDict(
     "ListIntentStageMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsIntentStageResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionMetricsResponseTypeDef = TypedDict(
     "ListSessionMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsSessionResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUtteranceMetricsResponseTypeDef = TypedDict(
     "ListUtteranceMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsUtteranceResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromptAttemptSpecificationOutputTypeDef = TypedDict(
     "PromptAttemptSpecificationOutputTypeDef",
     {
         "allowInterrupt": bool,
@@ -5133,28 +5132,28 @@
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
         "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
     "TestExecutionSummaryTypeDef",
     {
         "testExecutionId": str,
@@ -5327,15 +5326,15 @@
     "ListIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TranscriptFilterOutputTypeDef = TypedDict(
     "TranscriptFilterOutputTypeDef",
     {
         "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
@@ -5351,42 +5350,42 @@
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
@@ -5403,15 +5402,15 @@
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExportRequestRequestTypeDef",
     {
         "resourceSpecification": ExportResourceSpecificationTypeDef,
@@ -5457,15 +5456,15 @@
 
 ListSessionAnalyticsDataResponseTypeDef = TypedDict(
     "ListSessionAnalyticsDataResponseTypeDef",
     {
         "botId": str,
         "nextToken": str,
         "sessions": List[SessionSpecificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAggregatedUtterancesResponseTypeDef = TypedDict(
     "ListAggregatedUtterancesResponseTypeDef",
     {
         "botId": str,
@@ -5474,15 +5473,15 @@
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationOutputTypeDef,
         "aggregationWindowStartTime": datetime,
         "aggregationWindowEndTime": datetime,
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
@@ -5523,15 +5522,15 @@
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
@@ -5539,15 +5538,15 @@
         "creationDateTime": datetime,
         "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     {
         "testSetId": str,
@@ -5586,15 +5585,15 @@
 )
 
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MessageGroupOutputTypeDef = TypedDict(
     "MessageGroupOutputTypeDef",
     {
         "message": MessageOutputTypeDef,
@@ -5605,15 +5604,15 @@
 UtteranceSpecificationTypeDef = TypedDict(
     "UtteranceSpecificationTypeDef",
     {
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
         "sessionId": str,
-        "channel": BotChannelTypeType,
+        "channel": str,
         "mode": AnalyticsModalityType,
         "conversationStartTime": datetime,
         "conversationEndTime": datetime,
         "utterance": str,
         "utteranceTimestamp": datetime,
         "audioVoiceDurationMillis": int,
         "utteranceUnderstood": bool,
@@ -5676,15 +5675,15 @@
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestSetGenerationResponseTypeDef = TypedDict(
     "StartTestSetGenerationResponseTypeDef",
     {
         "testSetGenerationId": str,
@@ -5692,15 +5691,15 @@
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
         "testSetName": str,
@@ -5765,15 +5764,15 @@
     "ListExportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSlotTypeResponseTypeDef = TypedDict(
     "CreateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5784,15 +5783,15 @@
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSlotTypeResponseTypeDef = TypedDict(
     "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5804,15 +5803,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSlotTypeResponseTypeDef = TypedDict(
     "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5824,15 +5823,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeName": str,
@@ -5906,27 +5905,27 @@
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
@@ -6023,15 +6022,15 @@
 
 ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
     "ListUtteranceAnalyticsDataResponseTypeDef",
     {
         "botId": str,
         "nextToken": str,
         "utterances": List[UtteranceSpecificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
@@ -6158,15 +6157,15 @@
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
         "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotAliasResponseTypeDef = TypedDict(
     "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
@@ -6178,15 +6177,15 @@
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotAliasResponseTypeDef = TypedDict(
     "UpdateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
@@ -6196,15 +6195,15 @@
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
         "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotAliasRequestRequestTypeDef",
     {
         "botAliasName": str,
@@ -6428,30 +6427,30 @@
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
@@ -6459,15 +6458,15 @@
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredStartBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
@@ -6516,15 +6515,15 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConditionalSpecificationOutputTypeDef = TypedDict(
     "ConditionalSpecificationOutputTypeDef",
     {
         "active": bool,
@@ -6583,15 +6582,15 @@
 )
 
 ListTestSetRecordsResponseTypeDef = TypedDict(
     "ListTestSetRecordsResponseTypeDef",
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntentClosingSettingOutputTypeDef = TypedDict(
     "IntentClosingSettingOutputTypeDef",
     {
         "closingResponse": ResponseSpecificationOutputTypeDef,
@@ -6785,15 +6784,15 @@
 )
 
 ListTestExecutionResultItemsResponseTypeDef = TypedDict(
     "ListTestExecutionResultItemsResponseTypeDef",
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitialResponseSettingOutputTypeDef = TypedDict(
     "InitialResponseSettingOutputTypeDef",
     {
         "initialResponse": ResponseSpecificationOutputTypeDef,
@@ -6910,15 +6909,15 @@
         "outputContexts": List[OutputContextOutputTypeDef],
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIntentResponseTypeDef = TypedDict(
     "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
@@ -6936,15 +6935,15 @@
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIntentResponseTypeDef = TypedDict(
     "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
@@ -6962,15 +6961,15 @@
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SlotValueElicitationSettingOutputTypeDef = TypedDict(
     "SlotValueElicitationSettingOutputTypeDef",
     {
         "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
@@ -7089,15 +7088,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSlotResponseTypeDef = TypedDict(
     "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
@@ -7110,15 +7109,15 @@
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSlotResponseTypeDef = TypedDict(
     "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
@@ -7131,15 +7130,15 @@
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSlotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlotRequestRequestTypeDef",
     {
         "slotName": str,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.pyi` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     AnalyticsSessionSortByNameType,
     AnalyticsSortOrderType,
     AnalyticsUtteranceFieldType,
     AnalyticsUtteranceFilterNameType,
     AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
-    BotChannelTypeType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
@@ -148,14 +147,15 @@
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
     "S3BucketLogDestinationOutputTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
     "CustomVocabularyItemOutputTypeDef",
     "FailedCustomVocabularyItemTypeDef",
+    "ResponseMetadataTypeDef",
     "CustomVocabularyEntryIdTypeDef",
     "CustomVocabularyItemTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
     "BotAliasTestExecutionTargetOutputTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
     "BotExportSpecificationOutputTypeDef",
@@ -179,15 +179,14 @@
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
     "BotVersionLocaleDetailsOutputTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
-    "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
     "ButtonOutputTypeDef",
     "ButtonTypeDef",
     "CloudWatchLogGroupLogDestinationOutputTypeDef",
@@ -213,90 +212,74 @@
     "SampleUtteranceTypeDef",
     "DialogCodeHookSettingsOutputTypeDef",
     "InputContextOutputTypeDef",
     "KendraConfigurationOutputTypeDef",
     "OutputContextOutputTypeDef",
     "SampleUtteranceOutputTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
-    "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
-    "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
     "MultipleValuesSettingOutputTypeDef",
     "ObfuscationSettingOutputTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "CustomPayloadOutputTypeDef",
     "CustomPayloadTypeDef",
     "CustomVocabularyExportSpecificationOutputTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
     "CustomVocabularyImportSpecificationOutputTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
     "DateRangeFilterOutputTypeDef",
     "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
-    "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
-    "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
-    "DeleteBotResponseTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
-    "DeleteBotVersionResponseTypeDef",
     "DeleteCustomVocabularyRequestRequestTypeDef",
-    "DeleteCustomVocabularyResponseTypeDef",
     "DeleteExportRequestRequestTypeDef",
-    "DeleteExportResponseTypeDef",
     "DeleteImportRequestRequestTypeDef",
-    "DeleteImportResponseTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteResourcePolicyStatementRequestRequestTypeDef",
-    "DeleteResourcePolicyStatementResponseTypeDef",
     "DeleteSlotRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
     "EncryptionSettingOutputTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
     "SlotPriorityOutputTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
-    "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
     "TestSetStorageLocationOutputTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
     "ElicitationCodeHookInvocationSettingOutputTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionSettingTypeDef",
     "ExportFilterTypeDef",
     "TestSetExportSpecificationOutputTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
     "GrammarSlotTypeSourceOutputTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
@@ -311,15 +294,14 @@
     "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
     "UtteranceDataSortByTypeDef",
     "PlainTextMessageOutputTypeDef",
     "SSMLMessageOutputTypeDef",
     "PlainTextMessageTypeDef",
@@ -327,66 +309,83 @@
     "OverallTestResultItemTypeDef",
     "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
     "TextInputSpecificationOutputTypeDef",
     "TextInputSpecificationTypeDef",
     "RelativeAggregationDurationOutputTypeDef",
     "RelativeAggregationDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
     "SampleValueOutputTypeDef",
     "SampleValueTypeDef",
     "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotPriorityTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
     "SlotValueOutputTypeDef",
     "SlotValueTypeDef",
     "SlotValueRegexFilterOutputTypeDef",
     "SlotValueRegexFilterTypeDef",
     "TestSetStorageLocationTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
-    "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     "TestSetImportInputLocationOutputTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
-    "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
     "AnalyticsIntentResultTypeDef",
     "ListIntentMetricsRequestRequestTypeDef",
-    "ListIntentPathsResponseTypeDef",
     "AnalyticsIntentStageResultTypeDef",
     "ListIntentStageMetricsRequestRequestTypeDef",
     "ListIntentPathsRequestRequestTypeDef",
     "AnalyticsSessionResultTypeDef",
     "ListSessionMetricsRequestRequestTypeDef",
     "AnalyticsUtteranceResultTypeDef",
     "ListUtteranceMetricsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
-    "SearchAssociatedTranscriptsResponseTypeDef",
     "AudioAndDTMFInputSpecificationOutputTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
     "AudioLogDestinationOutputTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
-    "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
+    "BuildBotLocaleResponseTypeDef",
+    "CreateResourcePolicyResponseTypeDef",
+    "CreateResourcePolicyStatementResponseTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "DeleteBotAliasResponseTypeDef",
+    "DeleteBotLocaleResponseTypeDef",
+    "DeleteBotResponseTypeDef",
+    "DeleteBotVersionResponseTypeDef",
+    "DeleteCustomVocabularyResponseTypeDef",
+    "DeleteExportResponseTypeDef",
+    "DeleteImportResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "ListCustomVocabularyItemsResponseTypeDef",
+    "ListIntentPathsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    "StopBotRecommendationResponseTypeDef",
+    "UpdateResourcePolicyResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
     "TestExecutionTargetOutputTypeDef",
     "TestExecutionTargetTypeDef",
     "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
@@ -1104,14 +1103,25 @@
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
     },
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
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
@@ -1400,26 +1410,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-BuildBotLocaleResponseTypeDef = TypedDict(
-    "BuildBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "lastBuildSubmittedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BuiltInIntentSortByTypeDef = TypedDict(
     "BuiltInIntentSortByTypeDef",
     {
         "attribute": Literal["IntentSignature"],
         "order": SortOrderType,
     },
 )
@@ -1684,41 +1682,23 @@
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
 
-CreateResourcePolicyResponseTypeDef = TypedDict(
-    "CreateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "service": str,
         "arn": str,
     },
     total=False,
 )
 
-CreateResourcePolicyStatementResponseTypeDef = TypedDict(
-    "CreateResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MultipleValuesSettingTypeDef = TypedDict(
     "MultipleValuesSettingTypeDef",
     {
         "allowMultipleValues": bool,
     },
     total=False,
 )
@@ -1740,23 +1720,14 @@
 ObfuscationSettingOutputTypeDef = TypedDict(
     "ObfuscationSettingOutputTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "importId": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomPayloadOutputTypeDef = TypedDict(
     "CustomPayloadOutputTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1835,44 +1806,23 @@
 )
 
 class DeleteBotAliasRequestRequestTypeDef(
     _RequiredDeleteBotAliasRequestRequestTypeDef, _OptionalDeleteBotAliasRequestRequestTypeDef
 ):
     pass
 
-DeleteBotAliasResponseTypeDef = TypedDict(
-    "DeleteBotAliasResponseTypeDef",
-    {
-        "botAliasId": str,
-        "botId": str,
-        "botAliasStatus": BotAliasStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBotLocaleRequestRequestTypeDef = TypedDict(
     "DeleteBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteBotLocaleResponseTypeDef = TypedDict(
-    "DeleteBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botLocaleStatus": BotLocaleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalDeleteBotRequestRequestTypeDef = TypedDict(
@@ -1884,23 +1834,14 @@
 )
 
 class DeleteBotRequestRequestTypeDef(
     _RequiredDeleteBotRequestRequestTypeDef, _OptionalDeleteBotRequestRequestTypeDef
 ):
     pass
 
-DeleteBotResponseTypeDef = TypedDict(
-    "DeleteBotResponseTypeDef",
-    {
-        "botId": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -1913,76 +1854,37 @@
 )
 
 class DeleteBotVersionRequestRequestTypeDef(
     _RequiredDeleteBotVersionRequestRequestTypeDef, _OptionalDeleteBotVersionRequestRequestTypeDef
 ):
     pass
 
-DeleteBotVersionResponseTypeDef = TypedDict(
-    "DeleteBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "botStatus": BotStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCustomVocabularyRequestRequestTypeDef = TypedDict(
     "DeleteCustomVocabularyRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DeleteCustomVocabularyResponseTypeDef = TypedDict(
-    "DeleteCustomVocabularyResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteExportRequestRequestTypeDef = TypedDict(
     "DeleteExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-DeleteExportResponseTypeDef = TypedDict(
-    "DeleteExportResponseTypeDef",
-    {
-        "exportId": str,
-        "exportStatus": ExportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImportRequestRequestTypeDef = TypedDict(
     "DeleteImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-DeleteImportResponseTypeDef = TypedDict(
-    "DeleteImportResponseTypeDef",
-    {
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIntentRequestRequestTypeDef = TypedDict(
     "DeleteIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2005,23 +1907,14 @@
 
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
     },
 )
@@ -2035,23 +1928,14 @@
 
 class DeleteResourcePolicyStatementRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyStatementRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
-DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyStatementResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSlotRequestRequestTypeDef = TypedDict(
     "DeleteSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2181,27 +2065,14 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
-    "DescribeCustomVocabularyMetadataResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyStatus": CustomVocabularyStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExportRequestRequestTypeDef = TypedDict(
     "DescribeExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
@@ -2233,24 +2104,14 @@
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
     "DescribeResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-DescribeResourcePolicyResponseTypeDef = TypedDict(
-    "DescribeResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSlotRequestRequestTypeDef = TypedDict(
     "DescribeSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
@@ -2373,21 +2234,14 @@
 
 class ElicitationCodeHookInvocationSettingTypeDef(
     _RequiredElicitationCodeHookInvocationSettingTypeDef,
     _OptionalElicitationCodeHookInvocationSettingTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionSettingTypeDef = TypedDict(
     "EncryptionSettingTypeDef",
     {
         "kmsKeyArn": str,
         "botLocaleExportPassword": str,
         "associatedTranscriptsPassword": str,
     },
@@ -2428,23 +2282,14 @@
 GetTestExecutionArtifactsUrlRequestRequestTypeDef = TypedDict(
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     {
         "testExecutionId": str,
     },
 )
 
-GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
-    "GetTestExecutionArtifactsUrlResponseTypeDef",
-    {
-        "testExecutionId": str,
-        "downloadArtifactsUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrammarSlotTypeSourceOutputTypeDef = TypedDict(
     "GrammarSlotTypeSourceOutputTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
         "kmsKeyArn": str,
     },
@@ -2697,22 +2542,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TestExecutionSortByTypeDef = TypedDict(
     "TestExecutionSortByTypeDef",
     {
         "attribute": TestExecutionSortAttributeType,
         "order": SortOrderType,
     },
 )
@@ -2833,25 +2670,14 @@
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
@@ -2955,26 +2781,14 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-StopBotRecommendationResponseTypeDef = TypedDict(
-    "StopBotRecommendationResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationStatus": BotRecommendationStatusType,
-        "botRecommendationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -3074,23 +2888,14 @@
 
 class UpdateResourcePolicyRequestRequestTypeDef(
     _RequiredUpdateResourcePolicyRequestRequestTypeDef,
     _OptionalUpdateResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-UpdateResourcePolicyResponseTypeDef = TypedDict(
-    "UpdateResourcePolicyResponseTypeDef",
-    {
-        "resourceArn": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTestSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
     },
 )
@@ -3173,22 +2978,14 @@
 )
 
 class ListIntentMetricsRequestRequestTypeDef(
     _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
 ):
     pass
 
-ListIntentPathsResponseTypeDef = TypedDict(
-    "ListIntentPathsResponseTypeDef",
-    {
-        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnalyticsIntentStageResultTypeDef = TypedDict(
     "AnalyticsIntentStageResultTypeDef",
     {
         "binKeys": List[AnalyticsBinKeyTypeDef],
         "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
         "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
     },
@@ -3339,28 +3136,14 @@
 
 class SearchAssociatedTranscriptsRequestRequestTypeDef(
     _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef,
     _OptionalSearchAssociatedTranscriptsRequestRequestTypeDef,
 ):
     pass
 
-SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
-    "SearchAssociatedTranscriptsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "nextIndex": int,
-        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
-        "totalResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AudioAndDTMFInputSpecificationOutputTypeDef = TypedDict(
     "AudioAndDTMFInputSpecificationOutputTypeDef",
     {
         "startTimeoutMs": int,
         "audioSpecification": AudioSpecificationOutputTypeDef,
         "dtmfSpecification": DTMFSpecificationOutputTypeDef,
     },
@@ -3406,59 +3189,275 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[NewCustomVocabularyItemTypeDef],
     },
 )
 
-ListCustomVocabularyItemsResponseTypeDef = TypedDict(
-    "ListCustomVocabularyItemsResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
         "resources": List[CustomVocabularyItemOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BuildBotLocaleResponseTypeDef = TypedDict(
+    "BuildBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "lastBuildSubmittedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyResponseTypeDef = TypedDict(
+    "CreateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateResourcePolicyStatementResponseTypeDef = TypedDict(
+    "CreateResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "importId": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotAliasResponseTypeDef = TypedDict(
+    "DeleteBotAliasResponseTypeDef",
+    {
+        "botAliasId": str,
+        "botId": str,
+        "botAliasStatus": BotAliasStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotLocaleResponseTypeDef = TypedDict(
+    "DeleteBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botLocaleStatus": BotLocaleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotResponseTypeDef = TypedDict(
+    "DeleteBotResponseTypeDef",
+    {
+        "botId": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBotVersionResponseTypeDef = TypedDict(
+    "DeleteBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "botStatus": BotStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomVocabularyResponseTypeDef = TypedDict(
+    "DeleteCustomVocabularyResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteExportResponseTypeDef = TypedDict(
+    "DeleteExportResponseTypeDef",
+    {
+        "exportId": str,
+        "exportStatus": ExportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImportResponseTypeDef = TypedDict(
+    "DeleteImportResponseTypeDef",
+    {
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourcePolicyStatementResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyStatementResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomVocabularyMetadataResponseTypeDef = TypedDict(
+    "DescribeCustomVocabularyMetadataResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyStatus": CustomVocabularyStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "policy": str,
+        "revisionId": str,
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
+GetTestExecutionArtifactsUrlResponseTypeDef = TypedDict(
+    "GetTestExecutionArtifactsUrlResponseTypeDef",
+    {
+        "testExecutionId": str,
+        "downloadArtifactsUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVocabularyItemsResponseTypeDef = TypedDict(
+    "ListCustomVocabularyItemsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchAssociatedTranscriptsResponseTypeDef = TypedDict(
+    "SearchAssociatedTranscriptsResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "nextIndex": int,
+        "associatedTranscripts": List[AssociatedTranscriptTypeDef],
+        "totalResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopBotRecommendationResponseTypeDef = TypedDict(
+    "StopBotRecommendationResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationStatus": BotRecommendationStatusType,
+        "botRecommendationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateResourcePolicyResponseTypeDef = TypedDict(
+    "UpdateResourcePolicyResponseTypeDef",
+    {
+        "resourceArn": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
@@ -3480,15 +3479,15 @@
 
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionTargetOutputTypeDef = TypedDict(
     "TestExecutionTargetOutputTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetOutputTypeDef,
@@ -3557,15 +3556,15 @@
         "localeName": str,
         "localeId": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsOutputTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotLocaleResponseTypeDef = TypedDict(
     "DescribeBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -3580,15 +3579,15 @@
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
         "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotLocaleResponseTypeDef = TypedDict(
     "UpdateBotLocaleResponseTypeDef",
     {
         "botId": str,
@@ -3599,15 +3598,15 @@
         "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsOutputTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
@@ -3701,15 +3700,15 @@
 ListBotLocalesResponseTypeDef = TypedDict(
     "ListBotLocalesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
@@ -3720,15 +3719,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
@@ -3739,15 +3738,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "botId": str,
@@ -3757,15 +3756,15 @@
         "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "botName": str,
@@ -3828,15 +3827,15 @@
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationSummaries": List[BotRecommendationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsRequestRequestTypeDef = TypedDict(
     "ListBotsRequestRequestTypeDef",
     {
         "sortBy": BotSortByTypeDef,
@@ -3848,28 +3847,28 @@
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "botId": str,
         "description": str,
         "botVersion": str,
         "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsOutputTypeDef],
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
@@ -3912,15 +3911,15 @@
 
 ListBotVersionsResponseTypeDef = TypedDict(
     "ListBotVersionsResponseTypeDef",
     {
         "botId": str,
         "botVersionSummaries": List[BotVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInIntentsRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInIntentsRequestRequestTypeDef",
     {
         "localeId": str,
@@ -3944,15 +3943,15 @@
 
 ListBuiltInIntentsResponseTypeDef = TypedDict(
     "ListBuiltInIntentsResponseTypeDef",
     {
         "builtInIntentSummaries": List[BuiltInIntentSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListBuiltInSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListBuiltInSlotTypesRequestRequestTypeDef",
     {
         "localeId": str,
@@ -3976,15 +3975,15 @@
 
 ListBuiltInSlotTypesResponseTypeDef = TypedDict(
     "ListBuiltInSlotTypesResponseTypeDef",
     {
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageResponseCardOutputTypeDef = TypedDict(
     "ImageResponseCardOutputTypeDef",
     {
         "title": str,
@@ -4341,15 +4340,15 @@
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
         "botMembers": List[BotMemberOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetResponseTypeDef = TypedDict(
     "DescribeTestSetResponseTypeDef",
     {
         "testSetId": str,
@@ -4358,15 +4357,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
     "TestSetSummaryTypeDef",
     {
         "testSetId": str,
@@ -4391,15 +4390,15 @@
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DialogStateOutputTypeDef = TypedDict(
     "DialogStateOutputTypeDef",
     {
         "dialogAction": DialogActionOutputTypeDef,
@@ -4497,15 +4496,15 @@
     "ListImportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "importSummaries": List[ImportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
@@ -4549,15 +4548,15 @@
 
 SessionSpecificationTypeDef = TypedDict(
     "SessionSpecificationTypeDef",
     {
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
-        "channel": BotChannelTypeType,
+        "channel": str,
         "sessionId": str,
         "conversationStartTime": datetime,
         "conversationEndTime": datetime,
         "conversationDurationSeconds": int,
         "conversationEndState": ConversationEndStateType,
         "mode": AnalyticsModalityType,
         "numberOfTurns": int,
@@ -4571,15 +4570,15 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
     {
         "botId": str,
@@ -4632,15 +4631,15 @@
     "ListSlotTypesResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "slotTypeSummaries": List[SlotTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSlotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotsRequestRequestTypeDef",
     {
         "botId": str,
@@ -4906,45 +4905,45 @@
 
 ListIntentMetricsResponseTypeDef = TypedDict(
     "ListIntentMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsIntentResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIntentStageMetricsResponseTypeDef = TypedDict(
     "ListIntentStageMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsIntentStageResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionMetricsResponseTypeDef = TypedDict(
     "ListSessionMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsSessionResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUtteranceMetricsResponseTypeDef = TypedDict(
     "ListUtteranceMetricsResponseTypeDef",
     {
         "botId": str,
         "results": List[AnalyticsUtteranceResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromptAttemptSpecificationOutputTypeDef = TypedDict(
     "PromptAttemptSpecificationOutputTypeDef",
     {
         "allowInterrupt": bool,
@@ -5000,28 +4999,28 @@
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
         "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
     "TestExecutionSummaryTypeDef",
     {
         "testExecutionId": str,
@@ -5188,15 +5187,15 @@
     "ListIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TranscriptFilterOutputTypeDef = TypedDict(
     "TranscriptFilterOutputTypeDef",
     {
         "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
@@ -5212,42 +5211,42 @@
 )
 
 ListTestSetsResponseTypeDef = TypedDict(
     "ListTestSetsResponseTypeDef",
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
@@ -5264,15 +5263,15 @@
     {
         "exportId": str,
         "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExportRequestRequestTypeDef",
     {
         "resourceSpecification": ExportResourceSpecificationTypeDef,
@@ -5316,15 +5315,15 @@
 
 ListSessionAnalyticsDataResponseTypeDef = TypedDict(
     "ListSessionAnalyticsDataResponseTypeDef",
     {
         "botId": str,
         "nextToken": str,
         "sessions": List[SessionSpecificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAggregatedUtterancesResponseTypeDef = TypedDict(
     "ListAggregatedUtterancesResponseTypeDef",
     {
         "botId": str,
@@ -5333,15 +5332,15 @@
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationOutputTypeDef,
         "aggregationWindowStartTime": datetime,
         "aggregationWindowEndTime": datetime,
         "aggregationLastRefreshedDateTime": datetime,
         "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
@@ -5380,15 +5379,15 @@
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
         "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
@@ -5396,15 +5395,15 @@
         "creationDateTime": datetime,
         "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     {
         "testSetId": str,
@@ -5443,15 +5442,15 @@
 )
 
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MessageGroupOutputTypeDef = TypedDict(
     "MessageGroupOutputTypeDef",
     {
         "message": MessageOutputTypeDef,
@@ -5462,15 +5461,15 @@
 UtteranceSpecificationTypeDef = TypedDict(
     "UtteranceSpecificationTypeDef",
     {
         "botAliasId": str,
         "botVersion": str,
         "localeId": str,
         "sessionId": str,
-        "channel": BotChannelTypeType,
+        "channel": str,
         "mode": AnalyticsModalityType,
         "conversationStartTime": datetime,
         "conversationEndTime": datetime,
         "utterance": str,
         "utteranceTimestamp": datetime,
         "audioVoiceDurationMillis": int,
         "utteranceUnderstood": bool,
@@ -5531,15 +5530,15 @@
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTestSetGenerationResponseTypeDef = TypedDict(
     "StartTestSetGenerationResponseTypeDef",
     {
         "testSetGenerationId": str,
@@ -5547,15 +5546,15 @@
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "testSetName": str,
         "description": str,
         "storageLocation": TestSetStorageLocationOutputTypeDef,
         "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
         "testSetName": str,
@@ -5616,15 +5615,15 @@
     "ListExportsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSlotTypeResponseTypeDef = TypedDict(
     "CreateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5635,15 +5634,15 @@
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSlotTypeResponseTypeDef = TypedDict(
     "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5655,15 +5654,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSlotTypeResponseTypeDef = TypedDict(
     "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
@@ -5675,15 +5674,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeName": str,
@@ -5753,27 +5752,27 @@
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
@@ -5868,15 +5867,15 @@
 
 ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
     "ListUtteranceAnalyticsDataResponseTypeDef",
     {
         "botId": str,
         "nextToken": str,
         "utterances": List[UtteranceSpecificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
@@ -5993,15 +5992,15 @@
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
         "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBotAliasResponseTypeDef = TypedDict(
     "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
@@ -6013,15 +6012,15 @@
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotAliasResponseTypeDef = TypedDict(
     "UpdateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
@@ -6031,15 +6030,15 @@
         "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
         "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotAliasRequestRequestTypeDef",
     {
         "botAliasName": str,
@@ -6253,30 +6252,30 @@
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
@@ -6284,15 +6283,15 @@
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
         "encryptionSetting": EncryptionSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredStartBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
@@ -6339,15 +6338,15 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConditionalSpecificationOutputTypeDef = TypedDict(
     "ConditionalSpecificationOutputTypeDef",
     {
         "active": bool,
@@ -6404,15 +6403,15 @@
 )
 
 ListTestSetRecordsResponseTypeDef = TypedDict(
     "ListTestSetRecordsResponseTypeDef",
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntentClosingSettingOutputTypeDef = TypedDict(
     "IntentClosingSettingOutputTypeDef",
     {
         "closingResponse": ResponseSpecificationOutputTypeDef,
@@ -6602,15 +6601,15 @@
 )
 
 ListTestExecutionResultItemsResponseTypeDef = TypedDict(
     "ListTestExecutionResultItemsResponseTypeDef",
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitialResponseSettingOutputTypeDef = TypedDict(
     "InitialResponseSettingOutputTypeDef",
     {
         "initialResponse": ResponseSpecificationOutputTypeDef,
@@ -6725,15 +6724,15 @@
         "outputContexts": List[OutputContextOutputTypeDef],
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIntentResponseTypeDef = TypedDict(
     "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
@@ -6751,15 +6750,15 @@
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIntentResponseTypeDef = TypedDict(
     "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
@@ -6777,15 +6776,15 @@
         "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SlotValueElicitationSettingOutputTypeDef = TypedDict(
     "SlotValueElicitationSettingOutputTypeDef",
     {
         "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
@@ -6898,15 +6897,15 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSlotResponseTypeDef = TypedDict(
     "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
@@ -6919,15 +6918,15 @@
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSlotResponseTypeDef = TypedDict(
     "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
@@ -6940,15 +6939,15 @@
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
         "subSlotSetting": SubSlotSettingOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSlotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSlotRequestRequestTypeDef",
     {
         "slotName": str,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.py` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.pyi` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/PKG-INFO` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-models
-Version: 1.28.5
-Summary: Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.8
+Summary: Type annotations for boto3.LexModelsV2 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -346,15 +346,14 @@
     AnalyticsUtteranceMetricNameType,
     AnalyticsUtteranceSortByNameType,
     AssociatedTranscriptFilterNameType,
     AudioRecognitionStrategyType,
     BotAliasAvailableWaiterName,
     BotAliasStatusType,
     BotAvailableWaiterName,
-    BotChannelTypeType,
     BotExportCompletedWaiterName,
     BotFilterNameType,
     BotFilterOperatorType,
     BotImportCompletedWaiterName,
     BotLocaleBuiltWaiterName,
     BotLocaleCreatedWaiterName,
     BotLocaleExpressTestingAvailableWaiterName,
@@ -485,14 +484,15 @@
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
     S3BucketLogDestinationOutputTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
     CustomVocabularyItemOutputTypeDef,
     FailedCustomVocabularyItemTypeDef,
+    ResponseMetadataTypeDef,
     CustomVocabularyEntryIdTypeDef,
     CustomVocabularyItemTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
     BotAliasTestExecutionTargetOutputTypeDef,
     BotAliasTestExecutionTargetTypeDef,
     BotExportSpecificationOutputTypeDef,
@@ -516,15 +516,14 @@
     BotSortByTypeDef,
     BotSummaryTypeDef,
     BotVersionLocaleDetailsOutputTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
-    BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
     ButtonOutputTypeDef,
     ButtonTypeDef,
     CloudWatchLogGroupLogDestinationOutputTypeDef,
@@ -550,90 +549,74 @@
     SampleUtteranceTypeDef,
     DialogCodeHookSettingsOutputTypeDef,
     InputContextOutputTypeDef,
     KendraConfigurationOutputTypeDef,
     OutputContextOutputTypeDef,
     SampleUtteranceOutputTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
-    CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
-    CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
     MultipleValuesSettingOutputTypeDef,
     ObfuscationSettingOutputTypeDef,
-    CreateUploadUrlResponseTypeDef,
     CustomPayloadOutputTypeDef,
     CustomPayloadTypeDef,
     CustomVocabularyExportSpecificationOutputTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
     CustomVocabularyImportSpecificationOutputTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
     DateRangeFilterOutputTypeDef,
     DateRangeFilterTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
-    DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
-    DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
-    DeleteBotResponseTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
-    DeleteBotVersionResponseTypeDef,
     DeleteCustomVocabularyRequestRequestTypeDef,
-    DeleteCustomVocabularyResponseTypeDef,
     DeleteExportRequestRequestTypeDef,
-    DeleteExportResponseTypeDef,
     DeleteImportRequestRequestTypeDef,
-    DeleteImportResponseTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteResourcePolicyStatementRequestRequestTypeDef,
-    DeleteResourcePolicyStatementResponseTypeDef,
     DeleteSlotRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
     EncryptionSettingOutputTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
-    DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
     SlotPriorityOutputTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
-    DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
     TestSetStorageLocationOutputTypeDef,
     DescribeTestSetRequestRequestTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
     ElicitationCodeHookInvocationSettingOutputTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionSettingTypeDef,
     ExportFilterTypeDef,
     TestSetExportSpecificationOutputTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
-    GetTestExecutionArtifactsUrlResponseTypeDef,
     GrammarSlotTypeSourceOutputTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
@@ -648,15 +631,14 @@
     SessionDataSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
     UtteranceDataSortByTypeDef,
     PlainTextMessageOutputTypeDef,
     SSMLMessageOutputTypeDef,
     PlainTextMessageTypeDef,
@@ -664,66 +646,83 @@
     OverallTestResultItemTypeDef,
     PathFormatOutputTypeDef,
     PathFormatTypeDef,
     TextInputSpecificationOutputTypeDef,
     TextInputSpecificationTypeDef,
     RelativeAggregationDurationOutputTypeDef,
     RelativeAggregationDurationTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
     SampleValueOutputTypeDef,
     SampleValueTypeDef,
     SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
     SlotPriorityTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
     SlotValueOutputTypeDef,
     SlotValueTypeDef,
     SlotValueRegexFilterOutputTypeDef,
     SlotValueRegexFilterTypeDef,
     TestSetStorageLocationTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
-    StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
     TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
     TestSetImportInputLocationOutputTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
-    UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
     AnalyticsIntentResultTypeDef,
     ListIntentMetricsRequestRequestTypeDef,
-    ListIntentPathsResponseTypeDef,
     AnalyticsIntentStageResultTypeDef,
     ListIntentStageMetricsRequestRequestTypeDef,
     ListIntentPathsRequestRequestTypeDef,
     AnalyticsSessionResultTypeDef,
     ListSessionMetricsRequestRequestTypeDef,
     AnalyticsUtteranceResultTypeDef,
     ListUtteranceMetricsRequestRequestTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
-    SearchAssociatedTranscriptsResponseTypeDef,
     AudioAndDTMFInputSpecificationOutputTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
     AudioLogDestinationOutputTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
-    ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
+    BuildBotLocaleResponseTypeDef,
+    CreateResourcePolicyResponseTypeDef,
+    CreateResourcePolicyStatementResponseTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    DeleteBotAliasResponseTypeDef,
+    DeleteBotLocaleResponseTypeDef,
+    DeleteBotResponseTypeDef,
+    DeleteBotVersionResponseTypeDef,
+    DeleteCustomVocabularyResponseTypeDef,
+    DeleteExportResponseTypeDef,
+    DeleteImportResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteResourcePolicyStatementResponseTypeDef,
+    DescribeCustomVocabularyMetadataResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetTestExecutionArtifactsUrlResponseTypeDef,
+    ListCustomVocabularyItemsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SearchAssociatedTranscriptsResponseTypeDef,
+    StopBotRecommendationResponseTypeDef,
+    UpdateResourcePolicyResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
     BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
     TestExecutionTargetOutputTypeDef,
     TestExecutionTargetTypeDef,
     BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
```

### Comparing `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-models-1.28.8/mypy_boto3_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.5/setup.py` & `mypy-boto3-lexv2-models-1.28.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-models",
-    version="1.28.5",
+    version="1.28.8",
     packages=["mypy_boto3_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.LexModelsV2 1.28.8 service generated with mypy-boto3-builder"
         " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

