# Comparing `tmp/mypy-boto3-s3-1.28.3.post2.tar.gz` & `tmp/mypy-boto3-s3-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:35 2023, max compression
+gzip compressed data, was "mypy-boto3-s3-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-s3-1.28.3.post2.tar` & `mypy-boto3-s3-1.28.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.242399 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83859 2023-07-15 06:37:38.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83740 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   117865 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   117649 2023-07-15 06:37:38.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   204619 2023-07-15 06:37:47.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   204307 2023-07-15 06:37:44.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-15 06:37:40.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 06:38:35.000000 mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:35.250400 mypy-boto3-s3-1.28.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-15 06:37:37.000000 mypy-boto3-s3-1.28.3.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-s3-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37024 2023-07-20 19:47:56.000775 mypy-boto3-s3-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-s3-1.28.8/mypy_boto3_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83859 2023-07-20 19:47:08.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83740 2023-07-20 19:47:08.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16627 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   117865 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117649 2023-07-20 19:47:08.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   204473 2023-07-20 19:47:15.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204161 2023-07-20 19:47:13.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-20 19:47:10.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37024 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 19:47:55.000000 mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-s3-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-20 19:47:07.000000 mypy-boto3-s3-1.28.8/setup.py
```

### Comparing `mypy-boto3-s3-1.28.3.post2/LICENSE` & `mypy-boto3-s3-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/PKG-INFO` & `mypy-boto3-s3-1.28.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.3.post2
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.8
+Summary: Type annotations for boto3.S3 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -553,15 +553,15 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
@@ -583,25 +583,22 @@
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -622,94 +619,80 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
@@ -725,24 +708,20 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
@@ -750,57 +729,73 @@
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
@@ -851,14 +846,19 @@
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.3.post2/README.md` & `mypy-boto3-s3-1.28.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -521,15 +521,15 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
@@ -551,25 +551,22 @@
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -590,94 +587,80 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
@@ -693,24 +676,20 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
@@ -718,57 +697,73 @@
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
@@ -819,14 +814,19 @@
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__init__.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/__main__.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
-        " 7.15.0\nDocs:           "
+        "Type annotations for boto3.S3 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3.post2")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/client.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,14 +484,15 @@
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

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/literals.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,15 @@
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

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 
@@ -101,15 +101,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 
@@ -125,15 +125,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 
@@ -151,15 +151,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 
@@ -176,13 +176,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/paginator.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         *,
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 class ListObjectVersionsPaginator(Paginator):
@@ -96,15 +96,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 class ListObjectsPaginator(Paginator):
@@ -119,15 +119,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 class ListObjectsV2Paginator(Paginator):
@@ -144,15 +144,15 @@
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 class ListPartsPaginator(Paginator):
@@ -168,13 +168,13 @@
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/service_resource.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
     "TagOutputTypeDef",
@@ -109,25 +109,22 @@
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
@@ -148,94 +145,80 @@
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "OwnerOutputTypeDef",
     "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
     "DeletedObjectTypeDef",
     "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "ErrorDocumentOutputTypeDef",
-    "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentOutputTypeDef",
     "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "IndexDocumentResponseMetadataTypeDef",
     "IndexDocumentTypeDef",
-    "InitiatorResponseMetadataTypeDef",
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringOutputTypeDef",
     "TieringTypeDef",
     "InventoryFilterOutputTypeDef",
     "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
@@ -251,24 +234,20 @@
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
-    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
-    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
-    "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
-    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
-    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedOutputTypeDef",
     "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
@@ -276,57 +255,73 @@
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "ObjectLockRetentionTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "ProgressTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
     "RecordsEventTypeDef",
-    "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectAllRequestsToTypeDef",
     "RedirectOutputTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
-    "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
-    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ErrorDocumentResponseMetadataTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
+    "GetObjectOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
+    "HeadObjectOutputTypeDef",
+    "IndexDocumentResponseMetadataTypeDef",
+    "InitiatorResponseMetadataTypeDef",
+    "OwnerResponseMetadataTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseMetadataTypeDef",
+    "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "AnalyticsAndOperatorOutputTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorOutputTypeDef",
     "MetricsAndOperatorOutputTypeDef",
@@ -377,14 +372,19 @@
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
+    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    "ListObjectsRequestListObjectsPaginateTypeDef",
+    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsOutputTypeDef",
     "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
@@ -541,19 +541,22 @@
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     {
         "RequestPayer": Literal["requester"],
@@ -1013,35 +1016,14 @@
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
-    {
-        "Location": str,
-        "Bucket": str,
-        "Key": str,
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CompletedPartTypeDef = TypedDict(
     "CompletedPartTypeDef",
     {
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
@@ -1213,42 +1195,14 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
-    {
-        "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef = TypedDict(
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
@@ -1732,24 +1686,14 @@
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
     total=False,
 )
 
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "VersionId": str,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteObjectRequestObjectDeleteTypeDef = TypedDict(
     "DeleteObjectRequestObjectDeleteTypeDef",
     {
         "MFA": str,
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "BypassGovernanceRetention": bool,
@@ -1803,22 +1747,14 @@
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
 
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -1911,21 +1847,14 @@
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionType": ServerSideEncryptionType,
     },
 )
 _OptionalEncryptionTypeDef = TypedDict(
@@ -1945,22 +1874,14 @@
 ErrorDocumentOutputTypeDef = TypedDict(
     "ErrorDocumentOutputTypeDef",
     {
         "Key": str,
     },
 )
 
-ErrorDocumentResponseMetadataTypeDef = TypedDict(
-    "ErrorDocumentResponseMetadataTypeDef",
-    {
-        "Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
 
@@ -1991,23 +1912,14 @@
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
-    {
-        "Status": BucketAccelerateStatusType,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
@@ -2185,22 +2097,14 @@
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
-    {
-        "LocationConstraint": BucketLocationConstraintType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLocationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -2302,22 +2206,14 @@
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2382,22 +2278,14 @@
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
-    {
-        "Payer": PayerType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2433,23 +2321,14 @@
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketVersioningRequestRequestTypeDef = TypedDict(
@@ -2621,57 +2500,14 @@
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentRange": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "TagCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectRequestObjectGetTypeDef = TypedDict(
     "GetObjectRequestObjectGetTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -2838,23 +2674,14 @@
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetObjectTorrentRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTorrentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2972,55 +2799,14 @@
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
 
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "ArchiveStatus": ArchiveStatusType,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ETag": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HeadObjectRequestObjectVersionHeadTypeDef = TypedDict(
     "HeadObjectRequestObjectVersionHeadTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -3066,38 +2852,21 @@
 
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
 
-IndexDocumentResponseMetadataTypeDef = TypedDict(
-    "IndexDocumentResponseMetadataTypeDef",
-    {
-        "Suffix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InitiatorTypeDef = TypedDict(
     "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
 )
@@ -3337,41 +3106,24 @@
 class ListBucketMetricsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultipartUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListMultipartUploadsRequestRequestTypeDef = TypedDict(
@@ -3393,42 +3145,14 @@
 class ListMultipartUploadsRequestRequestTypeDef(
     _RequiredListMultipartUploadsRequestRequestTypeDef,
     _OptionalListMultipartUploadsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
-    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectVersionsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectVersionsRequestRequestTypeDef = TypedDict(
@@ -3451,42 +3175,14 @@
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
     _OptionalListObjectVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectsRequestListObjectsPaginateTypeDef(
-    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
-    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsRequestRequestTypeDef = TypedDict(
@@ -3507,44 +3203,14 @@
 
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "FetchOwner": bool,
-        "StartAfter": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
-    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
-    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsV2RequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsV2RequestRequestTypeDef = TypedDict(
@@ -3581,43 +3247,14 @@
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
 
-_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsRequestListPartsPaginateTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-    },
-)
-_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsRequestListPartsPaginateTypeDef",
-    {
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKey": str,
-        "SSECustomerKeyMD5": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPartsRequestListPartsPaginateTypeDef(
-    _RequiredListPartsRequestListPartsPaginateTypeDef,
-    _OptionalListPartsRequestListPartsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPartsRequestRequestTypeDef = TypedDict(
     "_RequiredListPartsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "UploadId": str,
     },
@@ -3822,47 +3459,28 @@
 
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
 
-OwnerResponseMetadataTypeDef = TypedDict(
-    "OwnerResponseMetadataTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OwnershipControlsRuleOutputTypeDef = TypedDict(
     "OwnershipControlsRuleOutputTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ProgressTypeDef = TypedDict(
     "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
@@ -3959,59 +3577,14 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalPutObjectRequestBucketPutObjectTypeDef = TypedDict(
@@ -4199,46 +3772,21 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecordsEventTypeDef = TypedDict(
     "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
 )
 
-RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
-    "RedirectAllRequestsToResponseMetadataTypeDef",
-    {
-        "HostName": str,
-        "Protocol": ProtocolType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRedirectAllRequestsToTypeDef = TypedDict(
     "_RequiredRedirectAllRequestsToTypeDef",
     {
         "HostName": str,
     },
 )
 _OptionalRedirectAllRequestsToTypeDef = TypedDict(
@@ -4297,43 +3845,14 @@
     "RequestProgressTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
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
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "RestoreOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestoreStatusResponseMetadataTypeDef = TypedDict(
-    "RestoreStatusResponseMetadataTypeDef",
-    {
-        "IsRestoreInProgress": bool,
-        "RestoreExpiryDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": int,
         "End": int,
     },
     total=False,
@@ -4387,32 +3906,14 @@
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
-    {
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UploadPartRequestMultipartUploadPartUploadTypeDef = TypedDict(
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "ContentLength": int,
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -4521,14 +4022,371 @@
 class WriteGetObjectResponseRequestRequestTypeDef(
     _RequiredWriteGetObjectResponseRequestRequestTypeDef,
     _OptionalWriteGetObjectResponseRequestRequestTypeDef,
 ):
     pass
 
 
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
+    {
+        "Location": str,
+        "Bucket": str,
+        "Key": str,
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
+    {
+        "Location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
+    {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "VersionId": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
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
+ErrorDocumentResponseMetadataTypeDef = TypedDict(
+    "ErrorDocumentResponseMetadataTypeDef",
+    {
+        "Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    {
+        "Status": BucketAccelerateStatusType,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
+    {
+        "LocationConstraint": BucketLocationConstraintType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
+    {
+        "Payer": PayerType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentRange": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "TagCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "ArchiveStatus": ArchiveStatusType,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ETag": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentResponseMetadataTypeDef = TypedDict(
+    "IndexDocumentResponseMetadataTypeDef",
+    {
+        "Suffix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
+    {
+        "ID": str,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OwnerResponseMetadataTypeDef = TypedDict(
+    "OwnerResponseMetadataTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    {
+        "HostName": str,
+        "Protocol": ProtocolType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "RestoreOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusResponseMetadataTypeDef = TypedDict(
+    "RestoreStatusResponseMetadataTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
+    {
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "AccelerateConfiguration": AccelerateConfigurationTypeDef,
     },
 )
@@ -4557,24 +4415,24 @@
     },
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectTaggingOutputTypeDef = TypedDict(
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
     "IntelligentTieringAndOperatorOutputTypeDef",
     {
         "Prefix": str,
@@ -4893,15 +4751,15 @@
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
@@ -4919,30 +4777,30 @@
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadPartCopyOutputTypeDef = TypedDict(
     "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
         "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -5044,25 +4902,25 @@
 )
 
 ListBucketsOutputTypeDef = TypedDict(
     "ListBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "Owner": OwnerOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteObjectsOutputTypeDef = TypedDict(
     "DeleteObjectsOutputTypeDef",
     {
         "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
         "Errors": List[ErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
@@ -5096,15 +4954,15 @@
     total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesPartsTypeDef = TypedDict(
     "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
@@ -5116,31 +4974,31 @@
     },
 )
 
 GetObjectLegalHoldOutputTypeDef = TypedDict(
     "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GrantOutputTypeDef = TypedDict(
     "GrantOutputTypeDef",
     {
         "Grantee": GranteeOutputTypeDef,
@@ -5377,14 +5235,156 @@
 )
 
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
+_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
+    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectsRequestListObjectsPaginateTypeDef(
+    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
+    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "FetchOwner": bool,
+        "StartAfter": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
+    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsRequestListPartsPaginateTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+    },
+)
+_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsRequestListPartsPaginateTypeDef",
+    {
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKey": str,
+        "SSECustomerKeyMD5": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPartsRequestListPartsPaginateTypeDef(
+    _RequiredListPartsRequestListPartsPaginateTypeDef,
+    _OptionalListPartsRequestListPartsPaginateTypeDef,
+):
+    pass
+
+
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
@@ -5395,15 +5395,15 @@
         "IsTruncated": bool,
         "Parts": List[PartTypeDef],
         "Initiator": InitiatorTypeDef,
         "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsOutputTypeDef = TypedDict(
     "MetricsOutputTypeDef",
     {
         "Status": MetricsStatusType,
@@ -5448,15 +5448,15 @@
 
 NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
@@ -6141,34 +6141,34 @@
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
         "Checksum": ChecksumTypeDef,
         "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketAclOutputTypeDef = TypedDict(
     "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAclOutputTypeDef = TypedDict(
     "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingEnabledOutputTypeDef = TypedDict(
     "LoggingEnabledOutputTypeDef",
     {
         "TargetBucket": str,
@@ -6179,15 +6179,15 @@
 
 LoggingEnabledResponseMetadataTypeDef = TypedDict(
     "LoggingEnabledResponseMetadataTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantOutputTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessControlPolicyTypeDef = TypedDict(
     "AccessControlPolicyTypeDef",
     {
         "Grants": Sequence[GrantTypeDef],
@@ -6253,15 +6253,15 @@
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryS3BucketDestinationOutputTypeDef = TypedDict(
     "InventoryS3BucketDestinationOutputTypeDef",
     {
         "AccountId": str,
@@ -6338,15 +6338,15 @@
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
@@ -6424,15 +6424,15 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
@@ -6444,15 +6444,15 @@
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
@@ -6465,23 +6465,23 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6508,15 +6508,15 @@
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
         "IndexDocument": IndexDocumentOutputTypeDef,
         "ErrorDocument": ErrorDocumentOutputTypeDef,
         "RoutingRules": List[RoutingRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
         "ErrorDocument": ErrorDocumentTypeDef,
@@ -6670,15 +6670,15 @@
     total=False,
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6804,15 +6804,15 @@
     pass
 
 
 GetBucketLoggingOutputTypeDef = TypedDict(
     "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -7058,15 +7058,15 @@
     pass
 
 
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7091,61 +7091,61 @@
     pass
 
 
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7219,15 +7219,15 @@
 NotificationConfigurationResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
         "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "TopicConfigurations": Sequence[TopicConfigurationTypeDef],
@@ -7387,26 +7387,26 @@
     pass
 
 
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7527,26 +7527,26 @@
     pass
 
 
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7570,15 +7570,15 @@
     pass
 
 
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/type_defs.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
     "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
     "TagOutputTypeDef",
@@ -108,25 +108,22 @@
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
     "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
     "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
     "CompletedPartTypeDef",
     "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "CopyObjectResultTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
     "CopyPartResultTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
     "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
@@ -147,94 +144,80 @@
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
     "OwnerOutputTypeDef",
     "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
     "DeletedObjectTypeDef",
     "ErrorTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
     "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "ErrorDocumentOutputTypeDef",
-    "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
     "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
     "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
     "IndexDocumentOutputTypeDef",
     "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
     "ObjectPartTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
     "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
     "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
     "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
-    "IndexDocumentResponseMetadataTypeDef",
     "IndexDocumentTypeDef",
-    "InitiatorResponseMetadataTypeDef",
     "InitiatorTypeDef",
     "JSONInputTypeDef",
     "TieringOutputTypeDef",
     "TieringTypeDef",
     "InventoryFilterOutputTypeDef",
     "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
@@ -250,24 +233,20 @@
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
-    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMultipartUploadsRequestRequestTypeDef",
-    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
-    "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
-    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
     "PartTypeDef",
-    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
     "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "QueueConfigurationDeprecatedOutputTypeDef",
     "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
@@ -275,57 +254,73 @@
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
     "ObjectLockLegalHoldTypeDef",
     "ObjectLockRetentionTypeDef",
     "RestoreStatusTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
-    "OwnerResponseMetadataTypeDef",
     "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "ProgressTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
     "RecordsEventTypeDef",
-    "RedirectAllRequestsToResponseMetadataTypeDef",
     "RedirectAllRequestsToTypeDef",
     "RedirectOutputTypeDef",
     "RedirectTypeDef",
     "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
-    "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
     "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
     "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StatsTypeDef",
-    "UploadPartOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
+    "AbortMultipartUploadOutputTypeDef",
+    "CompleteMultipartUploadOutputTypeDef",
+    "CreateBucketOutputTypeDef",
+    "CreateMultipartUploadOutputTypeDef",
+    "DeleteObjectOutputTypeDef",
+    "DeleteObjectTaggingOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ErrorDocumentResponseMetadataTypeDef",
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketLocationOutputTypeDef",
+    "GetBucketPolicyOutputTypeDef",
+    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketVersioningOutputTypeDef",
+    "GetObjectOutputTypeDef",
+    "GetObjectTorrentOutputTypeDef",
+    "HeadObjectOutputTypeDef",
+    "IndexDocumentResponseMetadataTypeDef",
+    "InitiatorResponseMetadataTypeDef",
+    "OwnerResponseMetadataTypeDef",
+    "PutObjectAclOutputTypeDef",
+    "PutObjectLegalHoldOutputTypeDef",
+    "PutObjectLockConfigurationOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "PutObjectRetentionOutputTypeDef",
+    "PutObjectTaggingOutputTypeDef",
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RestoreObjectOutputTypeDef",
+    "RestoreStatusResponseMetadataTypeDef",
+    "UploadPartOutputTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
     "AnalyticsAndOperatorOutputTypeDef",
     "GetBucketTaggingOutputTypeDef",
     "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorOutputTypeDef",
     "LifecycleRuleAndOperatorOutputTypeDef",
     "MetricsAndOperatorOutputTypeDef",
@@ -376,14 +371,19 @@
     "MultipartUploadTypeDef",
     "InputSerializationTypeDef",
     "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
+    "ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    "ListObjectsRequestListObjectsPaginateTypeDef",
+    "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsOutputTypeDef",
     "MetricsOutputTypeDef",
     "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
@@ -540,19 +540,22 @@
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     {
         "RequestPayer": Literal["requester"],
@@ -986,35 +989,14 @@
 CommonPrefixTypeDef = TypedDict(
     "CommonPrefixTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
-    {
-        "Location": str,
-        "Bucket": str,
-        "Key": str,
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CompletedPartTypeDef = TypedDict(
     "CompletedPartTypeDef",
     {
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
@@ -1182,42 +1164,14 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
-    {
-        "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
-    {
-        "AbortDate": datetime,
-        "AbortRuleId": str,
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef = TypedDict(
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     {
         "ACL": ObjectCannedACLType,
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
@@ -1675,24 +1629,14 @@
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
     total=False,
 )
 
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "VersionId": str,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteObjectRequestObjectDeleteTypeDef = TypedDict(
     "DeleteObjectRequestObjectDeleteTypeDef",
     {
         "MFA": str,
         "VersionId": str,
         "RequestPayer": Literal["requester"],
         "BypassGovernanceRetention": bool,
@@ -1744,22 +1688,14 @@
 )
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteObjectTaggingRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -1846,21 +1782,14 @@
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionType": ServerSideEncryptionType,
     },
 )
 _OptionalEncryptionTypeDef = TypedDict(
@@ -1878,22 +1807,14 @@
 ErrorDocumentOutputTypeDef = TypedDict(
     "ErrorDocumentOutputTypeDef",
     {
         "Key": str,
     },
 )
 
-ErrorDocumentResponseMetadataTypeDef = TypedDict(
-    "ErrorDocumentResponseMetadataTypeDef",
-    {
-        "Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
 
@@ -1924,23 +1845,14 @@
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
-    {
-        "Status": BucketAccelerateStatusType,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
@@ -2102,22 +2014,14 @@
 
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
-    {
-        "LocationConstraint": BucketLocationConstraintType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketLocationRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -2209,22 +2113,14 @@
 
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2283,22 +2179,14 @@
 
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
-    {
-        "Payer": PayerType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketRequestPaymentRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2330,23 +2218,14 @@
 )
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetBucketVersioningRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketVersioningRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalGetBucketVersioningRequestRequestTypeDef = TypedDict(
@@ -2506,57 +2385,14 @@
 
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentRange": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "TagCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectRequestObjectGetTypeDef = TypedDict(
     "GetObjectRequestObjectGetTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -2717,23 +2553,14 @@
 )
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
-    {
-        "Body": StreamingBody,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetObjectTorrentRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectTorrentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -2843,55 +2670,14 @@
 )
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
-    {
-        "DeleteMarker": bool,
-        "AcceptRanges": str,
-        "Expiration": str,
-        "Restore": str,
-        "ArchiveStatus": ArchiveStatusType,
-        "LastModified": datetime,
-        "ContentLength": int,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ETag": str,
-        "MissingMeta": int,
-        "VersionId": str,
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "ContentType": str,
-        "Expires": datetime,
-        "WebsiteRedirectLocation": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "Metadata": Dict[str, str],
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "StorageClass": StorageClassType,
-        "RequestCharged": Literal["requester"],
-        "ReplicationStatus": ReplicationStatusType,
-        "PartsCount": int,
-        "ObjectLockMode": ObjectLockModeType,
-        "ObjectLockRetainUntilDate": datetime,
-        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HeadObjectRequestObjectVersionHeadTypeDef = TypedDict(
     "HeadObjectRequestObjectVersionHeadTypeDef",
     {
         "IfMatch": str,
         "IfModifiedSince": Union[datetime, str],
         "IfNoneMatch": str,
         "IfUnmodifiedSince": Union[datetime, str],
@@ -2935,38 +2721,21 @@
 )
 
 class HeadObjectRequestRequestTypeDef(
     _RequiredHeadObjectRequestRequestTypeDef, _OptionalHeadObjectRequestRequestTypeDef
 ):
     pass
 
-IndexDocumentResponseMetadataTypeDef = TypedDict(
-    "IndexDocumentResponseMetadataTypeDef",
-    {
-        "Suffix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IndexDocumentTypeDef = TypedDict(
     "IndexDocumentTypeDef",
     {
         "Suffix": str,
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
-    {
-        "ID": str,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InitiatorTypeDef = TypedDict(
     "InitiatorTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
 )
@@ -3198,39 +2967,24 @@
 
 class ListBucketMetricsConfigurationsRequestRequestTypeDef(
     _RequiredListBucketMetricsConfigurationsRequestRequestTypeDef,
     _OptionalListBucketMetricsConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultipartUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListMultipartUploadsRequestRequestTypeDef = TypedDict(
@@ -3250,40 +3004,14 @@
 
 class ListMultipartUploadsRequestRequestTypeDef(
     _RequiredListMultipartUploadsRequestRequestTypeDef,
     _OptionalListMultipartUploadsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "ExpectedBucketOwner": str,
-        "RequestPayer": Literal["requester"],
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
-    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectVersionsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectVersionsRequestRequestTypeDef = TypedDict(
@@ -3304,40 +3032,14 @@
 
 class ListObjectVersionsRequestRequestTypeDef(
     _RequiredListObjectVersionsRequestRequestTypeDef,
     _OptionalListObjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectsRequestListObjectsPaginateTypeDef(
-    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
-    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsRequestRequestTypeDef = TypedDict(
@@ -3356,42 +3058,14 @@
 )
 
 class ListObjectsRequestRequestTypeDef(
     _RequiredListObjectsRequestRequestTypeDef, _OptionalListObjectsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
-    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
-    {
-        "Delimiter": str,
-        "EncodingType": Literal["url"],
-        "Prefix": str,
-        "FetchOwner": bool,
-        "StartAfter": str,
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
-    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
-    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
-):
-    pass
-
 _RequiredListObjectsV2RequestRequestTypeDef = TypedDict(
     "_RequiredListObjectsV2RequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalListObjectsV2RequestRequestTypeDef = TypedDict(
@@ -3426,41 +3100,14 @@
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
 
-_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsRequestListPartsPaginateTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-        "UploadId": str,
-    },
-)
-_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsRequestListPartsPaginateTypeDef",
-    {
-        "RequestPayer": Literal["requester"],
-        "ExpectedBucketOwner": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKey": str,
-        "SSECustomerKeyMD5": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPartsRequestListPartsPaginateTypeDef(
-    _RequiredListPartsRequestListPartsPaginateTypeDef,
-    _OptionalListPartsRequestListPartsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPartsRequestRequestTypeDef = TypedDict(
     "_RequiredListPartsRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "UploadId": str,
     },
@@ -3655,47 +3302,28 @@
 )
 
 class ObjectUploadFileobjRequestTypeDef(
     _RequiredObjectUploadFileobjRequestTypeDef, _OptionalObjectUploadFileobjRequestTypeDef
 ):
     pass
 
-OwnerResponseMetadataTypeDef = TypedDict(
-    "OwnerResponseMetadataTypeDef",
-    {
-        "DisplayName": str,
-        "ID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OwnershipControlsRuleOutputTypeDef = TypedDict(
     "OwnershipControlsRuleOutputTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ProgressTypeDef = TypedDict(
     "ProgressTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
@@ -3788,59 +3416,14 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "Expiration": str,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "VersionId": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "SSEKMSEncryptionContext": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectRequestBucketPutObjectTypeDef = TypedDict(
     "_RequiredPutObjectRequestBucketPutObjectTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalPutObjectRequestBucketPutObjectTypeDef = TypedDict(
@@ -4024,46 +3607,21 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
-    {
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecordsEventTypeDef = TypedDict(
     "RecordsEventTypeDef",
     {
         "Payload": bytes,
     },
 )
 
-RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
-    "RedirectAllRequestsToResponseMetadataTypeDef",
-    {
-        "HostName": str,
-        "Protocol": ProtocolType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRedirectAllRequestsToTypeDef = TypedDict(
     "_RequiredRedirectAllRequestsToTypeDef",
     {
         "HostName": str,
     },
 )
 _OptionalRedirectAllRequestsToTypeDef = TypedDict(
@@ -4120,43 +3678,14 @@
     "RequestProgressTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
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
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
-    {
-        "RequestCharged": Literal["requester"],
-        "RestoreOutputPath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestoreStatusResponseMetadataTypeDef = TypedDict(
-    "RestoreStatusResponseMetadataTypeDef",
-    {
-        "IsRestoreInProgress": bool,
-        "RestoreExpiryDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanRangeTypeDef = TypedDict(
     "ScanRangeTypeDef",
     {
         "Start": int,
         "End": int,
     },
     total=False,
@@ -4208,32 +3737,14 @@
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
-    {
-        "ServerSideEncryption": ServerSideEncryptionType,
-        "ETag": str,
-        "ChecksumCRC32": str,
-        "ChecksumCRC32C": str,
-        "ChecksumSHA1": str,
-        "ChecksumSHA256": str,
-        "SSECustomerAlgorithm": str,
-        "SSECustomerKeyMD5": str,
-        "SSEKMSKeyId": str,
-        "BucketKeyEnabled": bool,
-        "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UploadPartRequestMultipartUploadPartUploadTypeDef = TypedDict(
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "ContentLength": int,
         "ContentMD5": str,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -4338,14 +3849,371 @@
 
 class WriteGetObjectResponseRequestRequestTypeDef(
     _RequiredWriteGetObjectResponseRequestRequestTypeDef,
     _OptionalWriteGetObjectResponseRequestRequestTypeDef,
 ):
     pass
 
+AbortMultipartUploadOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartUploadOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputTypeDef",
+    {
+        "Location": str,
+        "Bucket": str,
+        "Key": str,
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBucketOutputTypeDef = TypedDict(
+    "CreateBucketOutputTypeDef",
+    {
+        "Location": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartUploadOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputTypeDef",
+    {
+        "AbortDate": datetime,
+        "AbortRuleId": str,
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectOutputTypeDef = TypedDict(
+    "DeleteObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "VersionId": str,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteObjectTaggingOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
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
+ErrorDocumentResponseMetadataTypeDef = TypedDict(
+    "ErrorDocumentResponseMetadataTypeDef",
+    {
+        "Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputTypeDef",
+    {
+        "Status": BucketAccelerateStatusType,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketLocationOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputTypeDef",
+    {
+        "LocationConstraint": BucketLocationConstraintType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketRequestPaymentOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputTypeDef",
+    {
+        "Payer": PayerType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketVersioningOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectOutputTypeDef = TypedDict(
+    "GetObjectOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentRange": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "TagCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectTorrentOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputTypeDef",
+    {
+        "Body": StreamingBody,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+HeadObjectOutputTypeDef = TypedDict(
+    "HeadObjectOutputTypeDef",
+    {
+        "DeleteMarker": bool,
+        "AcceptRanges": str,
+        "Expiration": str,
+        "Restore": str,
+        "ArchiveStatus": ArchiveStatusType,
+        "LastModified": datetime,
+        "ContentLength": int,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ETag": str,
+        "MissingMeta": int,
+        "VersionId": str,
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "ContentType": str,
+        "Expires": datetime,
+        "WebsiteRedirectLocation": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "Metadata": Dict[str, str],
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "StorageClass": StorageClassType,
+        "RequestCharged": Literal["requester"],
+        "ReplicationStatus": ReplicationStatusType,
+        "PartsCount": int,
+        "ObjectLockMode": ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "ObjectLockLegalHoldStatus": ObjectLockLegalHoldStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IndexDocumentResponseMetadataTypeDef = TypedDict(
+    "IndexDocumentResponseMetadataTypeDef",
+    {
+        "Suffix": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
+    {
+        "ID": str,
+        "DisplayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OwnerResponseMetadataTypeDef = TypedDict(
+    "OwnerResponseMetadataTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectAclOutputTypeDef = TypedDict(
+    "PutObjectAclOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLegalHoldOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectLockConfigurationOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "Expiration": str,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "VersionId": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "SSEKMSEncryptionContext": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectRetentionOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectTaggingOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputTypeDef",
+    {
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
+    "RedirectAllRequestsToResponseMetadataTypeDef",
+    {
+        "HostName": str,
+        "Protocol": ProtocolType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreObjectOutputTypeDef = TypedDict(
+    "RestoreObjectOutputTypeDef",
+    {
+        "RequestCharged": Literal["requester"],
+        "RestoreOutputPath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreStatusResponseMetadataTypeDef = TypedDict(
+    "RestoreStatusResponseMetadataTypeDef",
+    {
+        "IsRestoreInProgress": bool,
+        "RestoreExpiryDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadPartOutputTypeDef = TypedDict(
+    "UploadPartOutputTypeDef",
+    {
+        "ServerSideEncryption": ServerSideEncryptionType,
+        "ETag": str,
+        "ChecksumCRC32": str,
+        "ChecksumCRC32C": str,
+        "ChecksumSHA1": str,
+        "ChecksumSHA256": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKeyMD5": str,
+        "SSEKMSKeyId": str,
+        "BucketKeyEnabled": bool,
+        "RequestCharged": Literal["requester"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "AccelerateConfiguration": AccelerateConfigurationTypeDef,
     },
 )
@@ -4372,24 +4240,24 @@
     },
 )
 
 GetBucketTaggingOutputTypeDef = TypedDict(
     "GetBucketTaggingOutputTypeDef",
     {
         "TagSet": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectTaggingOutputTypeDef = TypedDict(
     "GetObjectTaggingOutputTypeDef",
     {
         "VersionId": str,
         "TagSet": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
     "IntelligentTieringAndOperatorOutputTypeDef",
     {
         "Prefix": str,
@@ -4696,15 +4564,15 @@
     },
 )
 
 GetBucketCorsOutputTypeDef = TypedDict(
     "GetBucketCorsOutputTypeDef",
     {
         "CORSRules": List[CORSRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
@@ -4722,30 +4590,30 @@
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadPartCopyOutputTypeDef = TypedDict(
     "UploadPartCopyOutputTypeDef",
     {
         "CopySourceVersionId": str,
         "CopyPartResult": CopyPartResultTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketRequestBucketCreateTypeDef = TypedDict(
     "CreateBucketRequestBucketCreateTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -4843,25 +4711,25 @@
 )
 
 ListBucketsOutputTypeDef = TypedDict(
     "ListBucketsOutputTypeDef",
     {
         "Buckets": List[BucketTypeDef],
         "Owner": OwnerOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteObjectsOutputTypeDef = TypedDict(
     "DeleteObjectsOutputTypeDef",
     {
         "Deleted": List[DeletedObjectTypeDef],
         "RequestCharged": Literal["requester"],
         "Errors": List[ErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
         "Objects": Sequence[ObjectIdentifierTypeDef],
@@ -4893,15 +4761,15 @@
     total=False,
 )
 
 GetBucketPolicyStatusOutputTypeDef = TypedDict(
     "GetBucketPolicyStatusOutputTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesPartsTypeDef = TypedDict(
     "GetObjectAttributesPartsTypeDef",
     {
         "TotalPartsCount": int,
@@ -4913,31 +4781,31 @@
     },
 )
 
 GetObjectLegalHoldOutputTypeDef = TypedDict(
     "GetObjectLegalHoldOutputTypeDef",
     {
         "LegalHold": ObjectLockLegalHoldOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectRetentionOutputTypeDef = TypedDict(
     "GetObjectRetentionOutputTypeDef",
     {
         "Retention": ObjectLockRetentionOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GrantOutputTypeDef = TypedDict(
     "GrantOutputTypeDef",
     {
         "Grantee": GranteeOutputTypeDef,
@@ -5164,14 +5032,146 @@
     },
     total=False,
 )
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
+_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "ExpectedBucketOwner": str,
+        "RequestPayer": Literal["requester"],
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectVersionsRequestListObjectVersionsPaginateTypeDef(
+    _RequiredListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    _OptionalListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsRequestListObjectsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectsRequestListObjectsPaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectsRequestListObjectsPaginateTypeDef(
+    _RequiredListObjectsRequestListObjectsPaginateTypeDef,
+    _OptionalListObjectsRequestListObjectsPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef = TypedDict(
+    "_OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef",
+    {
+        "Delimiter": str,
+        "EncodingType": Literal["url"],
+        "Prefix": str,
+        "FetchOwner": bool,
+        "StartAfter": str,
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "OptionalObjectAttributes": Sequence[Literal["RestoreStatus"]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectsV2RequestListObjectsV2PaginateTypeDef(
+    _RequiredListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    _OptionalListObjectsV2RequestListObjectsV2PaginateTypeDef,
+):
+    pass
+
+_RequiredListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsRequestListPartsPaginateTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "UploadId": str,
+    },
+)
+_OptionalListPartsRequestListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsRequestListPartsPaginateTypeDef",
+    {
+        "RequestPayer": Literal["requester"],
+        "ExpectedBucketOwner": str,
+        "SSECustomerAlgorithm": str,
+        "SSECustomerKey": str,
+        "SSECustomerKeyMD5": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPartsRequestListPartsPaginateTypeDef(
+    _RequiredListPartsRequestListPartsPaginateTypeDef,
+    _OptionalListPartsRequestListPartsPaginateTypeDef,
+):
+    pass
+
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
@@ -5182,15 +5182,15 @@
         "IsTruncated": bool,
         "Parts": List[PartTypeDef],
         "Initiator": InitiatorTypeDef,
         "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsOutputTypeDef = TypedDict(
     "MetricsOutputTypeDef",
     {
         "Status": MetricsStatusType,
@@ -5233,15 +5233,15 @@
 
 NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
@@ -5894,34 +5894,34 @@
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
         "Checksum": ChecksumTypeDef,
         "ObjectParts": GetObjectAttributesPartsTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketAclOutputTypeDef = TypedDict(
     "GetBucketAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAclOutputTypeDef = TypedDict(
     "GetObjectAclOutputTypeDef",
     {
         "Owner": OwnerOutputTypeDef,
         "Grants": List[GrantOutputTypeDef],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingEnabledOutputTypeDef = TypedDict(
     "LoggingEnabledOutputTypeDef",
     {
         "TargetBucket": str,
@@ -5932,15 +5932,15 @@
 
 LoggingEnabledResponseMetadataTypeDef = TypedDict(
     "LoggingEnabledResponseMetadataTypeDef",
     {
         "TargetBucket": str,
         "TargetGrants": List[TargetGrantOutputTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessControlPolicyTypeDef = TypedDict(
     "AccessControlPolicyTypeDef",
     {
         "Grants": Sequence[GrantTypeDef],
@@ -6002,15 +6002,15 @@
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
         "Uploads": List[MultipartUploadTypeDef],
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryS3BucketDestinationOutputTypeDef = TypedDict(
     "InventoryS3BucketDestinationOutputTypeDef",
     {
         "AccountId": str,
@@ -6083,15 +6083,15 @@
     },
 )
 
 GetBucketLifecycleOutputTypeDef = TypedDict(
     "GetBucketLifecycleOutputTypeDef",
     {
         "Rules": List[RuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
@@ -6165,15 +6165,15 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectsV2OutputTypeDef = TypedDict(
     "ListObjectsV2OutputTypeDef",
     {
         "IsTruncated": bool,
@@ -6185,15 +6185,15 @@
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListObjectVersionsOutputTypeDef = TypedDict(
     "ListObjectVersionsOutputTypeDef",
     {
         "IsTruncated": bool,
@@ -6206,23 +6206,23 @@
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
         "CommonPrefixes": List[CommonPrefixTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketOwnershipControlsOutputTypeDef = TypedDict(
     "GetBucketOwnershipControlsOutputTypeDef",
     {
         "OwnershipControls": OwnershipControlsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6247,15 +6247,15 @@
 GetBucketWebsiteOutputTypeDef = TypedDict(
     "GetBucketWebsiteOutputTypeDef",
     {
         "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
         "IndexDocument": IndexDocumentOutputTypeDef,
         "ErrorDocument": ErrorDocumentOutputTypeDef,
         "RoutingRules": List[RoutingRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
         "ErrorDocument": ErrorDocumentTypeDef,
@@ -6403,15 +6403,15 @@
     total=False,
 )
 
 GetObjectLockConfigurationOutputTypeDef = TypedDict(
     "GetObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6529,15 +6529,15 @@
 ):
     pass
 
 GetBucketLoggingOutputTypeDef = TypedDict(
     "GetBucketLoggingOutputTypeDef",
     {
         "LoggingEnabled": LoggingEnabledOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
@@ -6771,15 +6771,15 @@
 ):
     pass
 
 GetBucketEncryptionOutputTypeDef = TypedDict(
     "GetBucketEncryptionOutputTypeDef",
     {
         "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6802,61 +6802,61 @@
 ):
     pass
 
 SelectObjectContentOutputTypeDef = TypedDict(
     "SelectObjectContentOutputTypeDef",
     {
         "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
     "GetBucketIntelligentTieringConfigurationOutputTypeDef",
     {
         "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
     "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationOutputTypeDef",
     {
         "Rules": List[LifecycleRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
     "GetBucketMetricsConfigurationOutputTypeDef",
     {
         "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketMetricsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6926,15 +6926,15 @@
 NotificationConfigurationResponseMetadataTypeDef = TypedDict(
     "NotificationConfigurationResponseMetadataTypeDef",
     {
         "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
         "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
         "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "TopicConfigurations": Sequence[TopicConfigurationTypeDef],
@@ -7086,26 +7086,26 @@
 ):
     pass
 
 GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
     "GetBucketAnalyticsConfigurationOutputTypeDef",
     {
         "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
     "ListBucketAnalyticsConfigurationsOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7218,26 +7218,26 @@
 ):
     pass
 
 GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
     "GetBucketInventoryConfigurationOutputTypeDef",
     {
         "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
     "ListBucketInventoryConfigurationsOutputTypeDef",
     {
         "ContinuationToken": str,
         "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketInventoryConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -7259,15 +7259,15 @@
 ):
     pass
 
 GetBucketReplicationOutputTypeDef = TypedDict(
     "GetBucketReplicationOutputTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
         "Bucket": str,
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.py` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3/waiter.pyi` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.3.post2
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.8
+Summary: Type annotations for boto3.S3 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3?color=blue)](https://pypistats.org/packages/mypy-boto3-s3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
+[boto3.S3 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -553,15 +553,15 @@
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
     AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    ResponseMetadataTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
     AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
     TagOutputTypeDef,
@@ -583,25 +583,22 @@
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
     CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
     CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
     CompletedPartTypeDef,
     ConditionOutputTypeDef,
     ConditionTypeDef,
     CopyObjectResultTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
     CopyPartResultTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
     DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
@@ -622,94 +619,80 @@
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
     OwnerOutputTypeDef,
     DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
     DeletedObjectTypeDef,
     ErrorTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
     EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     ErrorDocumentOutputTypeDef,
-    ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
     ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
     FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
     IndexDocumentOutputTypeDef,
     RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
     ObjectPartTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
     ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
     ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
     PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
     GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
-    IndexDocumentResponseMetadataTypeDef,
     IndexDocumentTypeDef,
-    InitiatorResponseMetadataTypeDef,
     InitiatorTypeDef,
     JSONInputTypeDef,
     TieringOutputTypeDef,
     TieringTypeDef,
     InventoryFilterOutputTypeDef,
     InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
@@ -725,24 +708,20 @@
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
-    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMultipartUploadsRequestRequestTypeDef,
-    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
-    ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
-    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
     PartTypeDef,
-    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
     ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     QueueConfigurationDeprecatedOutputTypeDef,
     TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
@@ -750,57 +729,73 @@
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     RestoreStatusTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
-    OwnerResponseMetadataTypeDef,
     OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
-    PaginatorConfigTypeDef,
     ProgressTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
     RecordsEventTypeDef,
-    RedirectAllRequestsToResponseMetadataTypeDef,
     RedirectAllRequestsToTypeDef,
     RedirectOutputTypeDef,
     RedirectTypeDef,
     ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
-    RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
     ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
     SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StatsTypeDef,
-    UploadPartOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
+    AbortMultipartUploadOutputTypeDef,
+    CompleteMultipartUploadOutputTypeDef,
+    CreateBucketOutputTypeDef,
+    CreateMultipartUploadOutputTypeDef,
+    DeleteObjectOutputTypeDef,
+    DeleteObjectTaggingOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ErrorDocumentResponseMetadataTypeDef,
+    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketLocationOutputTypeDef,
+    GetBucketPolicyOutputTypeDef,
+    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketVersioningOutputTypeDef,
+    GetObjectOutputTypeDef,
+    GetObjectTorrentOutputTypeDef,
+    HeadObjectOutputTypeDef,
+    IndexDocumentResponseMetadataTypeDef,
+    InitiatorResponseMetadataTypeDef,
+    OwnerResponseMetadataTypeDef,
+    PutObjectAclOutputTypeDef,
+    PutObjectLegalHoldOutputTypeDef,
+    PutObjectLockConfigurationOutputTypeDef,
+    PutObjectOutputTypeDef,
+    PutObjectRetentionOutputTypeDef,
+    PutObjectTaggingOutputTypeDef,
+    RedirectAllRequestsToResponseMetadataTypeDef,
+    RestoreObjectOutputTypeDef,
+    RestoreStatusResponseMetadataTypeDef,
+    UploadPartOutputTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
     AnalyticsAndOperatorOutputTypeDef,
     GetBucketTaggingOutputTypeDef,
     GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorOutputTypeDef,
     LifecycleRuleAndOperatorOutputTypeDef,
     MetricsAndOperatorOutputTypeDef,
@@ -851,14 +846,19 @@
     MultipartUploadTypeDef,
     InputSerializationTypeDef,
     InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
+    ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef,
+    ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
+    ListObjectsRequestListObjectsPaginateTypeDef,
+    ListObjectsV2RequestListObjectsV2PaginateTypeDef,
+    ListPartsRequestListPartsPaginateTypeDef,
     ListPartsOutputTypeDef,
     MetricsOutputTypeDef,
     ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     NotificationConfigurationDeprecatedResponseMetadataTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
```

### Comparing `mypy-boto3-s3-1.28.3.post2/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy-boto3-s3-1.28.8/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3.post2/setup.py` & `mypy-boto3-s3-1.28.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.28.3.post2",
+    version="1.28.8",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.15.0"
+        "Type annotations for boto3.S3 1.28.8 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

