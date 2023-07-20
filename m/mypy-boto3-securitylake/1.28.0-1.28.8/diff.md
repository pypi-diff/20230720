# Comparing `tmp/mypy-boto3-securitylake-1.28.0.tar.gz` & `tmp/mypy-boto3-securitylake-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securitylake-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
+gzip compressed data, was "mypy-boto3-securitylake-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-securitylake-1.28.0.tar` & `mypy-boto3-securitylake-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.850427 mypy-boto3-securitylake-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-07-06 21:00:35.846428 mypy-boto3-securitylake-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.846428 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23969 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-06 20:55:29.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-06 20:55:29.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-07-06 20:55:29.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-07-06 20:55:29.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.846428 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:35.000000 mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.850427 mypy-boto3-securitylake-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:55:28.000000 mypy-boto3-securitylake-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27940 2023-07-20 19:47:43.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-07-20 19:47:43.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/setup.py
```

### Comparing `mypy-boto3-securitylake-1.28.0/LICENSE` & `mypy-boto3-securitylake-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.0/PKG-INFO` & `mypy-boto3-securitylake-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.28.0
-Summary: Type annotations for boto3.SecurityLake 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,91 +340,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
+    TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.0/README.md` & `mypy-boto3-securitylake-1.28.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,91 +308,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
+    TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__init__.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__init__.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/__main__.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityLake 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SecurityLake 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/client.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,18 @@
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogSourceResourceTypeDef,
     NotificationConfigurationTypeDef,
+    TagTypeDef,
     UpdateDataLakeResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -138,15 +140,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_custom_log_source)
         """
 
     def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
-        metaStoreManagerRoleArn: str
+        metaStoreManagerRoleArn: str,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake)
@@ -181,15 +184,16 @@
     def create_subscriber(
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
-        subscriberDescription: str = ...
+        subscriberDescription: str = ...,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber)
@@ -247,17 +251,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_exception_subscription)
         """
 
     def delete_data_lake_organization_configuration(
         self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Removes automatic the enablement of configuration settings for new member
-        accounts (but retains the settings for the delegated administrator) from Amazon
-        Security Lake.
+        Turns off automatic enablement of Amazon Security Lake for member accounts that
+        are added to an organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_organization_configuration)
         """
 
     def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
@@ -353,15 +356,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lake_exceptions)
         """
 
     def list_data_lakes(self, *, regions: Sequence[str] = ...) -> ListDataLakesResponseTypeDef:
         """
         Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Web Services Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lakes)
         """
 
     def list_log_sources(
         self,
@@ -385,23 +388,53 @@
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_subscribers)
         """
 
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Retrieves the tags (keys and values) that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_tags_for_resource)
+        """
+
     def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
         Designates the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#register_data_lake_delegated_administrator)
         """
 
+    def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+        """
+        Adds or updates one or more tags that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#tag_resource)
+        """
+
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes one or more tags (keys and values) from an Amazon Security Lake
+        resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#untag_resource)
+        """
+
     def update_data_lake(
         self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
     ) -> UpdateDataLakeResponseTypeDef:
         """
         Specifies where to store your security data and for how long.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/client.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,18 @@
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     ListDataLakesResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     ListSubscribersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     LogSourceResourceTypeDef,
     NotificationConfigurationTypeDef,
+    TagTypeDef,
     UpdateDataLakeResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -129,15 +131,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_custom_log_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_custom_log_source)
         """
     def create_data_lake(
         self,
         *,
         configurations: Sequence[DataLakeConfigurationTypeDef],
-        metaStoreManagerRoleArn: str
+        metaStoreManagerRoleArn: str,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataLakeResponseTypeDef:
         """
         Initializes an Amazon Security Lake instance with the provided (or default)
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_data_lake)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_data_lake)
@@ -169,15 +172,16 @@
     def create_subscriber(
         self,
         *,
         sources: Sequence[LogSourceResourceTypeDef],
         subscriberIdentity: AwsIdentityTypeDef,
         subscriberName: str,
         accessTypes: Sequence[AccessTypeType] = ...,
-        subscriberDescription: str = ...
+        subscriberDescription: str = ...,
+        tags: Sequence[TagTypeDef] = ...
     ) -> CreateSubscriberResponseTypeDef:
         """
         Creates a subscription permission for accounts that are already enabled in
         Amazon Security Lake.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.create_subscriber)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#create_subscriber)
@@ -229,17 +233,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_exception_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_exception_subscription)
         """
     def delete_data_lake_organization_configuration(
         self, *, autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef]
     ) -> Dict[str, Any]:
         """
-        Removes automatic the enablement of configuration settings for new member
-        accounts (but retains the settings for the delegated administrator) from Amazon
-        Security Lake.
+        Turns off automatic enablement of Amazon Security Lake for member accounts that
+        are added to an organization in Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.delete_data_lake_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#delete_data_lake_organization_configuration)
         """
     def delete_subscriber(self, *, subscriberId: str) -> Dict[str, Any]:
         """
         Deletes the subscription permission and all notification settings for accounts
@@ -325,15 +328,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lake_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lake_exceptions)
         """
     def list_data_lakes(self, *, regions: Sequence[str] = ...) -> ListDataLakesResponseTypeDef:
         """
         Retrieves the Amazon Security Lake configuration object for the specified Amazon
-        Web Services account ID.
+        Web Services Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_data_lakes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_data_lakes)
         """
     def list_log_sources(
         self,
         *,
@@ -354,22 +357,49 @@
     ) -> ListSubscribersResponseTypeDef:
         """
         List all subscribers for the specific Amazon Security Lake account ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_subscribers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_subscribers)
         """
+    def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
+        """
+        Retrieves the tags (keys and values) that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.list_tags_for_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#list_tags_for_resource)
+        """
     def register_data_lake_delegated_administrator(self, *, accountId: str) -> Dict[str, Any]:
         """
         Designates the Amazon Security Lake delegated administrator account for the
         organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.register_data_lake_delegated_administrator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#register_data_lake_delegated_administrator)
         """
+    def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
+        """
+        Adds or updates one or more tags that are associated with an Amazon Security
+        Lake resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.tag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#tag_resource)
+        """
+    def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
+        """
+        Removes one or more tags (keys and values) from an Amazon Security Lake
+        resource: a subscriber, or the data lake configuration for your Amazon Web
+        Services account in a particular Amazon Web Services Region.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.untag_resource)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/client/#untag_resource)
+        """
     def update_data_lake(
         self, *, configurations: Sequence[DataLakeConfigurationTypeDef]
     ) -> UpdateDataLakeResponseTypeDef:
         """
         Specifies where to store your security data and for how long.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client.update_data_lake)
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/literals.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
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

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/literals.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
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

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/paginator.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,30 +59,30 @@
 class GetDataLakeSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDataLakeSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
 
 class ListDataLakeExceptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, regions: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 
@@ -94,28 +94,28 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
         """
 
 
 class ListSubscribersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/paginator.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,29 +56,29 @@
 class GetDataLakeSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
     """
 
     def paginate(
-        self, *, accounts: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accounts: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDataLakeSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.GetDataLakeSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#getdatalakesourcespaginator)
         """
 
 class ListDataLakeExceptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
     """
 
     def paginate(
-        self, *, regions: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, regions: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataLakeExceptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListDataLakeExceptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listdatalakeexceptionspaginator)
         """
 
 class ListLogSourcesPaginator(Paginator):
@@ -89,27 +89,27 @@
 
     def paginate(
         self,
         *,
         accounts: Sequence[str] = ...,
         regions: Sequence[str] = ...,
         sources: Sequence[LogSourceResourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLogSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListLogSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listlogsourcespaginator)
         """
 
 class ListSubscribersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscribersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Paginator.ListSubscribers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/paginators/#listsubscriberspaginator)
         """
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/type_defs.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityOutputTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -27,89 +27,115 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AwsIdentityOutputTypeDef",
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceOutputTypeDef",
     "AwsLogSourceResourceTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "CreateSubscriberNotificationResponseTypeDef",
+    "TagTypeDef",
+    "CustomLogSourceAttributesOutputTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderOutputTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeEncryptionConfigurationOutputTypeDef",
     "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    "DataLakeLifecycleTransitionOutputTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriberNotificationResponseTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceOutputTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
+    "LogSourceResourceOutputTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "LogSourceTypeDef",
+    "SubscriberResourceTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
-    "LogSourceTypeDef",
-    "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
     "UpdateDataLakeRequestRequestTypeDef",
     "CreateDataLakeResponseTypeDef",
     "ListDataLakesResponseTypeDef",
     "UpdateDataLakeResponseTypeDef",
     "ListLogSourcesResponseTypeDef",
     "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
 )
 
+AwsIdentityOutputTypeDef = TypedDict(
+    "AwsIdentityOutputTypeDef",
+    {
+        "externalId": str,
+        "principal": str,
+    },
+)
+
 AwsIdentityTypeDef = TypedDict(
     "AwsIdentityTypeDef",
     {
         "externalId": str,
         "principal": str,
     },
 )
@@ -133,28 +159,39 @@
 
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
 
+AwsLogSourceResourceOutputTypeDef = TypedDict(
+    "AwsLogSourceResourceOutputTypeDef",
+    {
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
+    },
+)
+
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -173,19 +210,28 @@
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSubscriberNotificationResponseTypeDef = TypedDict(
-    "CreateSubscriberNotificationResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "key": str,
+        "value": str,
+    },
+)
+
+CustomLogSourceAttributesOutputTypeDef = TypedDict(
+    "CustomLogSourceAttributesOutputTypeDef",
+    {
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
     },
 )
 
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
@@ -198,14 +244,22 @@
 CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
     "CustomLogSourceCrawlerConfigurationTypeDef",
     {
         "roleArn": str,
     },
 )
 
+CustomLogSourceProviderOutputTypeDef = TypedDict(
+    "CustomLogSourceProviderOutputTypeDef",
+    {
+        "location": str,
+        "roleArn": str,
+    },
+)
+
 CustomLogSourceProviderTypeDef = TypedDict(
     "CustomLogSourceProviderTypeDef",
     {
         "location": str,
         "roleArn": str,
     },
     total=False,
@@ -224,23 +278,44 @@
     {
         "regions": Sequence[str],
         "roleArn": str,
     },
     total=False,
 )
 
+DataLakeEncryptionConfigurationOutputTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+)
+
 DataLakeExceptionTypeDef = TypedDict(
     "DataLakeExceptionTypeDef",
     {
         "exception": str,
         "region": str,
         "remediation": str,
         "timestamp": datetime,
     },
-    total=False,
+)
+
+DataLakeLifecycleExpirationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    {
+        "days": int,
+    },
+)
+
+DataLakeLifecycleTransitionOutputTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionOutputTypeDef",
+    {
+        "days": int,
+        "storageClass": str,
+    },
 )
 
 DataLakeLifecycleExpirationTypeDef = TypedDict(
     "DataLakeLifecycleExpirationTypeDef",
     {
         "days": int,
     },
@@ -252,38 +327,36 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
+DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationOutputTypeDef",
+    {
+        "regions": List[str],
+        "roleArn": str,
+    },
+)
+
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
-    total=False,
 )
 
 DataLakeUpdateExceptionTypeDef = TypedDict(
     "DataLakeUpdateExceptionTypeDef",
     {
         "code": str,
         "reason": str,
     },
-    total=False,
-)
-
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
-    {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
@@ -321,29 +394,20 @@
 DeleteSubscriberRequestRequestTypeDef = TypedDict(
     "DeleteSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 
-GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    {
-        "exceptionTimeToLive": int,
-        "notificationEndpoint": str,
-        "subscriptionProtocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "accounts": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
     "GetDataLakeSourcesRequestRequestTypeDef",
     {
@@ -381,23 +445,14 @@
 
 class HttpsNotificationConfigurationTypeDef(
     _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
 ):
     pass
 
 
-ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
-    {
-        "regions": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
     "ListDataLakeExceptionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "regions": Sequence[str],
     },
@@ -408,56 +463,50 @@
     "ListDataLakesRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
     total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceArn": str,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
     },
-    total=False,
 )
 
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -476,52 +525,112 @@
 class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSubscriberNotificationResponseTypeDef = TypedDict(
-    "UpdateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
     "CreateAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
+    {
+        "region": str,
+        "sources": List[AwsLogSourceResourceOutputTypeDef],
+    },
+)
+
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
 
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    {
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
 
+CustomLogSourceResourceOutputTypeDef = TypedDict(
+    "CustomLogSourceResourceOutputTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesOutputTypeDef,
+        "provider": CustomLogSourceProviderOutputTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
+    },
+)
+
 CustomLogSourceResourceTypeDef = TypedDict(
     "CustomLogSourceResourceTypeDef",
     {
         "attributes": CustomLogSourceAttributesTypeDef,
         "provider": CustomLogSourceProviderTypeDef,
         "sourceName": str,
         "sourceVersion": str,
@@ -530,15 +639,23 @@
 )
 
 ListDataLakeExceptionsResponseTypeDef = TypedDict(
     "ListDataLakeExceptionsResponseTypeDef",
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationOutputTypeDef",
+    {
+        "expiration": DataLakeLifecycleExpirationOutputTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionOutputTypeDef],
     },
 )
 
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
@@ -551,58 +668,90 @@
     "DataLakeSourceTypeDef",
     {
         "account": str,
         "eventClasses": List[str],
         "sourceName": str,
         "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
-    total=False,
 )
 
 DataLakeUpdateStatusTypeDef = TypedDict(
     "DataLakeUpdateStatusTypeDef",
     {
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
+)
+
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    {
+        "accounts": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    {
+        "regions": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
 DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "GetDataLakeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -622,16 +771,24 @@
 ):
     pass
 
 
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
-        "source": CustomLogSourceResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "source": CustomLogSourceResourceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LogSourceResourceOutputTypeDef = TypedDict(
+    "LogSourceResourceOutputTypeDef",
+    {
+        "awsLogSource": AwsLogSourceResourceOutputTypeDef,
+        "customLogSource": CustomLogSourceResourceOutputTypeDef,
     },
 )
 
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
@@ -665,43 +822,32 @@
 
 GetDataLakeSourcesResponseTypeDef = TypedDict(
     "GetDataLakeSourcesResponseTypeDef",
     {
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataLakeResourceTypeDef = TypedDict(
-    "_RequiredDataLakeResourceTypeDef",
+DataLakeResourceTypeDef = TypedDict(
+    "DataLakeResourceTypeDef",
     {
+        "createStatus": DataLakeStatusType,
         "dataLakeArn": str,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationOutputTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
         "region": str,
-    },
-)
-_OptionalDataLakeResourceTypeDef = TypedDict(
-    "_OptionalDataLakeResourceTypeDef",
-    {
-        "createStatus": DataLakeStatusType,
-        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
-    total=False,
 )
 
-
-class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
-    pass
-
-
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -710,27 +856,58 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+    },
+)
+
+SubscriberResourceTypeDef = TypedDict(
+    "SubscriberResourceTypeDef",
+    {
+        "accessTypes": List[AccessTypeType],
+        "createdAt": datetime,
+        "resourceShareArn": str,
+        "resourceShareName": str,
+        "roleArn": str,
+        "s3BucketArn": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+        "subscriberArn": str,
+        "subscriberDescription": str,
+        "subscriberEndpoint": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityOutputTypeDef,
+        "subscriberName": str,
+        "subscriberStatus": SubscriberStatusType,
+        "updatedAt": datetime,
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
@@ -740,15 +917,15 @@
 
 ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLogSourcesRequestRequestTypeDef = TypedDict(
     "ListLogSourcesRequestRequestTypeDef",
     {
@@ -757,58 +934,14 @@
         "nextToken": str,
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
     },
     total=False,
 )
 
-LogSourceTypeDef = TypedDict(
-    "LogSourceTypeDef",
-    {
-        "account": str,
-        "region": str,
-        "sources": List[LogSourceResourceTypeDef],
-    },
-    total=False,
-)
-
-_RequiredSubscriberResourceTypeDef = TypedDict(
-    "_RequiredSubscriberResourceTypeDef",
-    {
-        "sources": List[LogSourceResourceTypeDef],
-        "subscriberArn": str,
-        "subscriberId": str,
-        "subscriberIdentity": AwsIdentityTypeDef,
-        "subscriberName": str,
-    },
-)
-_OptionalSubscriberResourceTypeDef = TypedDict(
-    "_OptionalSubscriberResourceTypeDef",
-    {
-        "accessTypes": List[AccessTypeType],
-        "createdAt": datetime,
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "subscriberDescription": str,
-        "subscriberEndpoint": str,
-        "subscriberStatus": SubscriberStatusType,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-
-class SubscriberResourceTypeDef(
-    _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
-):
-    pass
-
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
@@ -825,87 +958,101 @@
 
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
 
-CreateDataLakeRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeRequestRequestTypeDef",
+_RequiredCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
+_OptionalCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateDataLakeRequestRequestTypeDef(
+    _RequiredCreateDataLakeRequestRequestTypeDef, _OptionalCreateDataLakeRequestRequestTypeDef
+):
+    pass
+
 
 UpdateDataLakeRequestRequestTypeDef = TypedDict(
     "UpdateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
 )
 
 CreateDataLakeResponseTypeDef = TypedDict(
     "CreateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataLakesResponseTypeDef = TypedDict(
     "ListDataLakesResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataLakeResponseTypeDef = TypedDict(
     "UpdateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSourcesResponseTypeDef = TypedDict(
     "ListLogSourcesResponseTypeDef",
     {
         "nextToken": str,
         "sources": List[LogSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriberResponseTypeDef = TypedDict(
     "CreateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake/type_defs.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityOutputTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -26,89 +26,115 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AwsIdentityOutputTypeDef",
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceOutputTypeDef",
     "AwsLogSourceResourceTypeDef",
-    "CreateAwsLogSourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "CreateSubscriberNotificationResponseTypeDef",
+    "TagTypeDef",
+    "CustomLogSourceAttributesOutputTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderOutputTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeEncryptionConfigurationOutputTypeDef",
     "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    "DataLakeLifecycleTransitionOutputTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
+    "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
-    "DeleteAwsLogSourceResponseTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
     "DeleteSubscriberNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "ListSubscribersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
-    "UpdateSubscriberNotificationResponseTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
+    "CreateAwsLogSourceResponseTypeDef",
+    "CreateSubscriberNotificationResponseTypeDef",
+    "DeleteAwsLogSourceResponseTypeDef",
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    "UpdateSubscriberNotificationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceOutputTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
+    "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
-    "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
+    "LogSourceResourceOutputTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "LogSourceTypeDef",
+    "SubscriberResourceTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
-    "LogSourceTypeDef",
-    "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
     "UpdateDataLakeRequestRequestTypeDef",
     "CreateDataLakeResponseTypeDef",
     "ListDataLakesResponseTypeDef",
     "UpdateDataLakeResponseTypeDef",
     "ListLogSourcesResponseTypeDef",
     "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
 )
 
+AwsIdentityOutputTypeDef = TypedDict(
+    "AwsIdentityOutputTypeDef",
+    {
+        "externalId": str,
+        "principal": str,
+    },
+)
+
 AwsIdentityTypeDef = TypedDict(
     "AwsIdentityTypeDef",
     {
         "externalId": str,
         "principal": str,
     },
 )
@@ -130,28 +156,39 @@
 )
 
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
+AwsLogSourceResourceOutputTypeDef = TypedDict(
+    "AwsLogSourceResourceOutputTypeDef",
+    {
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
+    },
+)
+
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
 )
 
-CreateAwsLogSourceResponseTypeDef = TypedDict(
-    "CreateAwsLogSourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -168,19 +205,28 @@
 
 class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalCreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-CreateSubscriberNotificationResponseTypeDef = TypedDict(
-    "CreateSubscriberNotificationResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "key": str,
+        "value": str,
+    },
+)
+
+CustomLogSourceAttributesOutputTypeDef = TypedDict(
+    "CustomLogSourceAttributesOutputTypeDef",
+    {
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
     },
 )
 
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
@@ -193,14 +239,22 @@
 CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
     "CustomLogSourceCrawlerConfigurationTypeDef",
     {
         "roleArn": str,
     },
 )
 
+CustomLogSourceProviderOutputTypeDef = TypedDict(
+    "CustomLogSourceProviderOutputTypeDef",
+    {
+        "location": str,
+        "roleArn": str,
+    },
+)
+
 CustomLogSourceProviderTypeDef = TypedDict(
     "CustomLogSourceProviderTypeDef",
     {
         "location": str,
         "roleArn": str,
     },
     total=False,
@@ -219,23 +273,44 @@
     {
         "regions": Sequence[str],
         "roleArn": str,
     },
     total=False,
 )
 
+DataLakeEncryptionConfigurationOutputTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+)
+
 DataLakeExceptionTypeDef = TypedDict(
     "DataLakeExceptionTypeDef",
     {
         "exception": str,
         "region": str,
         "remediation": str,
         "timestamp": datetime,
     },
-    total=False,
+)
+
+DataLakeLifecycleExpirationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    {
+        "days": int,
+    },
+)
+
+DataLakeLifecycleTransitionOutputTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionOutputTypeDef",
+    {
+        "days": int,
+        "storageClass": str,
+    },
 )
 
 DataLakeLifecycleExpirationTypeDef = TypedDict(
     "DataLakeLifecycleExpirationTypeDef",
     {
         "days": int,
     },
@@ -247,38 +322,36 @@
     {
         "days": int,
         "storageClass": str,
     },
     total=False,
 )
 
+DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
+    "DataLakeReplicationConfigurationOutputTypeDef",
+    {
+        "regions": List[str],
+        "roleArn": str,
+    },
+)
+
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
-    total=False,
 )
 
 DataLakeUpdateExceptionTypeDef = TypedDict(
     "DataLakeUpdateExceptionTypeDef",
     {
         "code": str,
         "reason": str,
     },
-    total=False,
-)
-
-DeleteAwsLogSourceResponseTypeDef = TypedDict(
-    "DeleteAwsLogSourceResponseTypeDef",
-    {
-        "failed": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
@@ -314,29 +387,20 @@
 DeleteSubscriberRequestRequestTypeDef = TypedDict(
     "DeleteSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 
-GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
-    "GetDataLakeExceptionSubscriptionResponseTypeDef",
-    {
-        "exceptionTimeToLive": int,
-        "notificationEndpoint": str,
-        "subscriptionProtocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
-    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "accounts": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDataLakeSourcesRequestRequestTypeDef = TypedDict(
     "GetDataLakeSourcesRequestRequestTypeDef",
     {
@@ -372,23 +436,14 @@
 )
 
 class HttpsNotificationConfigurationTypeDef(
     _RequiredHttpsNotificationConfigurationTypeDef, _OptionalHttpsNotificationConfigurationTypeDef
 ):
     pass
 
-ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
-    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
-    {
-        "regions": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataLakeExceptionsRequestRequestTypeDef = TypedDict(
     "ListDataLakeExceptionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "regions": Sequence[str],
     },
@@ -399,56 +454,50 @@
     "ListDataLakesRequestRequestTypeDef",
     {
         "regions": Sequence[str],
     },
     total=False,
 )
 
-ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
-    "ListSubscribersRequestListSubscribersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribersRequestRequestTypeDef = TypedDict(
     "ListSubscribersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceArn": str,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
     },
-    total=False,
 )
 
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     {
         "notificationEndpoint": str,
@@ -465,52 +514,112 @@
 
 class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(
     _RequiredUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     _OptionalUpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-UpdateSubscriberNotificationResponseTypeDef = TypedDict(
-    "UpdateSubscriberNotificationResponseTypeDef",
-    {
-        "subscriberEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAwsLogSourceRequestRequestTypeDef = TypedDict(
     "CreateAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
 DeleteAwsLogSourceRequestRequestTypeDef = TypedDict(
     "DeleteAwsLogSourceRequestRequestTypeDef",
     {
         "sources": Sequence[AwsLogSourceConfigurationTypeDef],
     },
 )
 
+DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
+    "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
+    {
+        "region": str,
+        "sources": List[AwsLogSourceResourceOutputTypeDef],
+    },
+)
+
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
         "sources": Sequence[AwsLogSourceResourceTypeDef],
     },
 )
 
+CreateAwsLogSourceResponseTypeDef = TypedDict(
+    "CreateAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSubscriberNotificationResponseTypeDef = TypedDict(
+    "CreateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAwsLogSourceResponseTypeDef = TypedDict(
+    "DeleteAwsLogSourceResponseTypeDef",
+    {
+        "failed": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeExceptionSubscriptionResponseTypeDef = TypedDict(
+    "GetDataLakeExceptionSubscriptionResponseTypeDef",
+    {
+        "exceptionTimeToLive": int,
+        "notificationEndpoint": str,
+        "subscriptionProtocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriberNotificationResponseTypeDef = TypedDict(
+    "UpdateSubscriberNotificationResponseTypeDef",
+    {
+        "subscriberEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
 CustomLogSourceConfigurationTypeDef = TypedDict(
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
 
+CustomLogSourceResourceOutputTypeDef = TypedDict(
+    "CustomLogSourceResourceOutputTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesOutputTypeDef,
+        "provider": CustomLogSourceProviderOutputTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
+    },
+)
+
 CustomLogSourceResourceTypeDef = TypedDict(
     "CustomLogSourceResourceTypeDef",
     {
         "attributes": CustomLogSourceAttributesTypeDef,
         "provider": CustomLogSourceProviderTypeDef,
         "sourceName": str,
         "sourceVersion": str,
@@ -519,15 +628,23 @@
 )
 
 ListDataLakeExceptionsResponseTypeDef = TypedDict(
     "ListDataLakeExceptionsResponseTypeDef",
     {
         "exceptions": List[DataLakeExceptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleConfigurationOutputTypeDef",
+    {
+        "expiration": DataLakeLifecycleExpirationOutputTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionOutputTypeDef],
     },
 )
 
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
@@ -540,58 +657,90 @@
     "DataLakeSourceTypeDef",
     {
         "account": str,
         "eventClasses": List[str],
         "sourceName": str,
         "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
-    total=False,
 )
 
 DataLakeUpdateStatusTypeDef = TypedDict(
     "DataLakeUpdateStatusTypeDef",
     {
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
+)
+
+GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
+    "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
+    {
+        "accounts": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef = TypedDict(
+    "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
+    {
+        "regions": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribersRequestListSubscribersPaginateTypeDef = TypedDict(
+    "ListSubscribersRequestListSubscribersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "GetDataLakeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
 DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnableNewAccount": Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],
     },
 )
 
-GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "GetDataLakeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
 )
 _OptionalCreateCustomLogSourceRequestRequestTypeDef = TypedDict(
@@ -609,16 +758,24 @@
     _OptionalCreateCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
-        "source": CustomLogSourceResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "source": CustomLogSourceResourceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LogSourceResourceOutputTypeDef = TypedDict(
+    "LogSourceResourceOutputTypeDef",
+    {
+        "awsLogSource": AwsLogSourceResourceOutputTypeDef,
+        "customLogSource": CustomLogSourceResourceOutputTypeDef,
     },
 )
 
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
@@ -650,41 +807,32 @@
 
 GetDataLakeSourcesResponseTypeDef = TypedDict(
     "GetDataLakeSourcesResponseTypeDef",
     {
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataLakeResourceTypeDef = TypedDict(
-    "_RequiredDataLakeResourceTypeDef",
+DataLakeResourceTypeDef = TypedDict(
+    "DataLakeResourceTypeDef",
     {
+        "createStatus": DataLakeStatusType,
         "dataLakeArn": str,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationOutputTypeDef,
+        "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
         "region": str,
-    },
-)
-_OptionalDataLakeResourceTypeDef = TypedDict(
-    "_OptionalDataLakeResourceTypeDef",
-    {
-        "createStatus": DataLakeStatusType,
-        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
-        "lifecycleConfiguration": DataLakeLifecycleConfigurationTypeDef,
-        "replicationConfiguration": DataLakeReplicationConfigurationTypeDef,
+        "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
-    total=False,
 )
 
-class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
-    pass
-
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -693,27 +841,58 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+    },
+)
+
+SubscriberResourceTypeDef = TypedDict(
+    "SubscriberResourceTypeDef",
+    {
+        "accessTypes": List[AccessTypeType],
+        "createdAt": datetime,
+        "resourceShareArn": str,
+        "resourceShareName": str,
+        "roleArn": str,
+        "s3BucketArn": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+        "subscriberArn": str,
+        "subscriberDescription": str,
+        "subscriberEndpoint": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityOutputTypeDef,
+        "subscriberName": str,
+        "subscriberStatus": SubscriberStatusType,
+        "updatedAt": datetime,
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
 )
 _OptionalCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSubscriberRequestRequestTypeDef",
     {
         "accessTypes": Sequence[AccessTypeType],
         "subscriberDescription": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateSubscriberRequestRequestTypeDef(
     _RequiredCreateSubscriberRequestRequestTypeDef, _OptionalCreateSubscriberRequestRequestTypeDef
 ):
@@ -721,15 +900,15 @@
 
 ListLogSourcesRequestListLogSourcesPaginateTypeDef = TypedDict(
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLogSourcesRequestRequestTypeDef = TypedDict(
     "ListLogSourcesRequestRequestTypeDef",
     {
@@ -738,56 +917,14 @@
         "nextToken": str,
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
     },
     total=False,
 )
 
-LogSourceTypeDef = TypedDict(
-    "LogSourceTypeDef",
-    {
-        "account": str,
-        "region": str,
-        "sources": List[LogSourceResourceTypeDef],
-    },
-    total=False,
-)
-
-_RequiredSubscriberResourceTypeDef = TypedDict(
-    "_RequiredSubscriberResourceTypeDef",
-    {
-        "sources": List[LogSourceResourceTypeDef],
-        "subscriberArn": str,
-        "subscriberId": str,
-        "subscriberIdentity": AwsIdentityTypeDef,
-        "subscriberName": str,
-    },
-)
-_OptionalSubscriberResourceTypeDef = TypedDict(
-    "_OptionalSubscriberResourceTypeDef",
-    {
-        "accessTypes": List[AccessTypeType],
-        "createdAt": datetime,
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "subscriberDescription": str,
-        "subscriberEndpoint": str,
-        "subscriberStatus": SubscriberStatusType,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-class SubscriberResourceTypeDef(
-    _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
-):
-    pass
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
@@ -802,87 +939,99 @@
 )
 
 class UpdateSubscriberRequestRequestTypeDef(
     _RequiredUpdateSubscriberRequestRequestTypeDef, _OptionalUpdateSubscriberRequestRequestTypeDef
 ):
     pass
 
-CreateDataLakeRequestRequestTypeDef = TypedDict(
-    "CreateDataLakeRequestRequestTypeDef",
+_RequiredCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
         "metaStoreManagerRoleArn": str,
     },
 )
+_OptionalCreateDataLakeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataLakeRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDataLakeRequestRequestTypeDef(
+    _RequiredCreateDataLakeRequestRequestTypeDef, _OptionalCreateDataLakeRequestRequestTypeDef
+):
+    pass
 
 UpdateDataLakeRequestRequestTypeDef = TypedDict(
     "UpdateDataLakeRequestRequestTypeDef",
     {
         "configurations": Sequence[DataLakeConfigurationTypeDef],
     },
 )
 
 CreateDataLakeResponseTypeDef = TypedDict(
     "CreateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataLakesResponseTypeDef = TypedDict(
     "ListDataLakesResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataLakeResponseTypeDef = TypedDict(
     "UpdateDataLakeResponseTypeDef",
     {
         "dataLakes": List[DataLakeResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSourcesResponseTypeDef = TypedDict(
     "ListLogSourcesResponseTypeDef",
     {
         "nextToken": str,
         "sources": List[LogSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubscriberResponseTypeDef = TypedDict(
     "CreateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSubscriberResponseTypeDef = TypedDict(
     "GetSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribersResponseTypeDef = TypedDict(
     "ListSubscribersResponseTypeDef",
     {
         "nextToken": str,
         "subscribers": List[SubscriberResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubscriberResponseTypeDef = TypedDict(
     "UpdateSubscriberResponseTypeDef",
     {
         "subscriber": SubscriberResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/PKG-INFO` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.28.0
-Summary: Type annotations for boto3.SecurityLake 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,91 +340,109 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
-    CreateAwsLogSourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    CreateSubscriberNotificationResponseTypeDef,
+    TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
+    DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
-    DeleteAwsLogSourceResponseTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
     DeleteSubscriberNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    GetDataLakeExceptionSubscriptionResponseTypeDef,
-    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
-    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
-    ListSubscribersRequestListSubscribersPaginateTypeDef,
     ListSubscribersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
-    UpdateSubscriberNotificationResponseTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
+    DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
+    CreateAwsLogSourceResponseTypeDef,
+    CreateSubscriberNotificationResponseTypeDef,
+    DeleteAwsLogSourceResponseTypeDef,
+    GetDataLakeExceptionSubscriptionResponseTypeDef,
+    UpdateSubscriberNotificationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
+    DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
+    GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
+    ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
+    ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
-    GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.0/mypy_boto3_securitylake.egg-info/SOURCES.txt` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.0/setup.py` & `mypy-boto3-securitylake-1.28.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securitylake",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityLake 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

