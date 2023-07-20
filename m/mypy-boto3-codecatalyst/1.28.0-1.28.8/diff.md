# Comparing `tmp/mypy-boto3-codecatalyst-1.28.0.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.28.0.tar` & `mypy-boto3-codecatalyst-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.678251 mypy-boto3-codecatalyst-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-06 20:59:12.666251 mypy-boto3-codecatalyst-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.666251 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24109 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-06 20:35:50.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-06 20:35:50.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-06 20:35:50.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-07-06 20:35:51.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-07-06 20:35:50.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.666251 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:12.000000 mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.678251 mypy-boto3-codecatalyst-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:35:49.000000 mypy-boto3-codecatalyst-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37203 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/LICENSE` & `mypy-boto3-codecatalyst-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.0/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeCatalyst 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,86 +358,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryRequestRequestTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectRequestRequestTypeDef,
+    DeleteSourceRepositoryRequestRequestTypeDef,
+    DeleteSpaceRequestRequestTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    IdeConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    UpdateProjectRequestRequestTypeDef,
+    UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/README.md` & `mypy-boto3-codecatalyst-1.28.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,86 +326,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryRequestRequestTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectRequestRequestTypeDef,
+    DeleteSourceRepositoryRequestRequestTypeDef,
+    DeleteSpaceRequestRequestTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    IdeConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    UpdateProjectRequestRequestTypeDef,
+    UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
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

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,20 +31,25 @@
     ListSpacesPaginator,
 )
 from .type_defs import (
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     FilterTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
@@ -57,14 +62,16 @@
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -162,14 +169,24 @@
         """
         Creates a project in a specified space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_project)
         """
 
+    def create_source_repository(
+        self, *, spaceName: str, projectName: str, name: str, description: str = ...
+    ) -> CreateSourceRepositoryResponseTypeDef:
+        """
+        Creates an empty Git-based source repository in a specified project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_source_repository)
+        """
+
     def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
@@ -196,14 +213,40 @@
         """
         Deletes a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_dev_environment)
         """
 
+    def delete_project(self, *, spaceName: str, name: str) -> DeleteProjectResponseTypeDef:
+        """
+        Deletes a project in a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_project)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_project)
+        """
+
+    def delete_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> DeleteSourceRepositoryResponseTypeDef:
+        """
+        Deletes a source repository in Amazon CodeCatalyst.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_source_repository)
+        """
+
+    def delete_space(self, *, name: str) -> DeleteSpaceResponseTypeDef:
+        """
+        Deletes a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_space)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_space)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -229,14 +272,24 @@
         """
         Returns information about a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_project)
         """
 
+    def get_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> GetSourceRepositoryResponseTypeDef:
+        """
+        Returns information about a source repository.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_source_repository)
+        """
+
     def get_source_repository_clone_urls(
         self, *, spaceName: str, projectName: str, sourceRepositoryName: str
     ) -> GetSourceRepositoryCloneUrlsResponseTypeDef:
         """
         Returns information about the URLs that can be used with a Git client to clone a
         source repository.
 
@@ -448,14 +501,32 @@
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_dev_environment)
         """
 
+    def update_project(
+        self, *, spaceName: str, name: str, description: str = ...
+    ) -> UpdateProjectResponseTypeDef:
+        """
+        Changes one or more values for a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_project)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_project)
+        """
+
+    def update_space(self, *, name: str, description: str = ...) -> UpdateSpaceResponseTypeDef:
+        """
+        Changes one or more values for a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_space)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_space)
+        """
+
     def verify_session(self) -> VerifySessionResponseTypeDef:
         """
         Verifies whether the calling user has a valid Amazon CodeCatalyst login and
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.verify_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#verify_session)
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -31,20 +31,25 @@
     ListSpacesPaginator,
 )
 from .type_defs import (
     CreateAccessTokenResponseTypeDef,
     CreateDevEnvironmentResponseTypeDef,
     CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
     DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     FilterTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
     GetSpaceResponseTypeDef,
     GetSubscriptionResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     IdeConfigurationTypeDef,
     ListAccessTokensResponseTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     ListDevEnvironmentsResponseTypeDef,
@@ -57,14 +62,16 @@
     ProjectListFilterTypeDef,
     RepositoryInputTypeDef,
     StartDevEnvironmentResponseTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -152,14 +159,23 @@
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a project in a specified space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_project)
         """
+    def create_source_repository(
+        self, *, spaceName: str, projectName: str, name: str, description: str = ...
+    ) -> CreateSourceRepositoryResponseTypeDef:
+        """
+        Creates an empty Git-based source repository in a specified project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.create_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#create_source_repository)
+        """
     def create_source_repository_branch(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
         name: str,
@@ -183,14 +199,37 @@
     ) -> DeleteDevEnvironmentResponseTypeDef:
         """
         Deletes a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_dev_environment)
         """
+    def delete_project(self, *, spaceName: str, name: str) -> DeleteProjectResponseTypeDef:
+        """
+        Deletes a project in a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_project)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_project)
+        """
+    def delete_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> DeleteSourceRepositoryResponseTypeDef:
+        """
+        Deletes a source repository in Amazon CodeCatalyst.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_source_repository)
+        """
+    def delete_space(self, *, name: str) -> DeleteSpaceResponseTypeDef:
+        """
+        Deletes a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.delete_space)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#delete_space)
+        """
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -213,14 +252,23 @@
     def get_project(self, *, spaceName: str, name: str) -> GetProjectResponseTypeDef:
         """
         Returns information about a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_project)
         """
+    def get_source_repository(
+        self, *, spaceName: str, projectName: str, name: str
+    ) -> GetSourceRepositoryResponseTypeDef:
+        """
+        Returns information about a source repository.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.get_source_repository)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#get_source_repository)
+        """
     def get_source_repository_clone_urls(
         self, *, spaceName: str, projectName: str, sourceRepositoryName: str
     ) -> GetSourceRepositoryCloneUrlsResponseTypeDef:
         """
         Returns information about the URLs that can be used with a Git client to clone a
         source repository.
 
@@ -415,14 +463,30 @@
     ) -> UpdateDevEnvironmentResponseTypeDef:
         """
         Changes one or more values for a Dev Environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_dev_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_dev_environment)
         """
+    def update_project(
+        self, *, spaceName: str, name: str, description: str = ...
+    ) -> UpdateProjectResponseTypeDef:
+        """
+        Changes one or more values for a project.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_project)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_project)
+        """
+    def update_space(self, *, name: str, description: str = ...) -> UpdateSpaceResponseTypeDef:
+        """
+        Changes one or more values for a space.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.update_space)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#update_space)
+        """
     def verify_session(self) -> VerifySessionResponseTypeDef:
         """
         Verifies whether the calling user has a valid Amazon CodeCatalyst login and
         session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Client.verify_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/client/#verify_session)
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
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

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -273,14 +273,15 @@
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

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 
@@ -97,15 +97,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 
@@ -117,15 +117,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 
@@ -138,15 +138,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 
@@ -157,30 +157,30 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
 
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 
@@ -192,28 +192,28 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 class ListDevEnvironmentSessionsPaginator(Paginator):
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 class ListDevEnvironmentsPaginator(Paginator):
@@ -112,15 +112,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 class ListEventLogsPaginator(Paginator):
@@ -132,15 +132,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
@@ -150,29 +150,29 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 class ListSourceRepositoryBranchesPaginator(Paginator):
@@ -183,27 +183,27 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,119 +33,121 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryRequestRequestTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectRequestRequestTypeDef",
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    "DeleteSpaceRequestRequestTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "IdeConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "UpdateProjectRequestRequestTypeDef",
+    "UpdateSpaceRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
+    "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -159,22 +161,22 @@
 
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -205,24 +207,14 @@
 )
 
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -237,25 +229,14 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -273,24 +254,37 @@
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
+_RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
     {
-        "ref": str,
+        "spaceName": str,
+        "projectName": str,
         "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class CreateSourceRepositoryRequestRequestTypeDef(
+    _RequiredCreateSourceRepositoryRequestRequestTypeDef,
+    _OptionalCreateSourceRepositoryRequestRequestTypeDef,
+):
+    pass
+
 
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -300,53 +294,54 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
+DeleteProjectRequestRequestTypeDef = TypedDict(
+    "DeleteProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+
+DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "DeleteSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+    },
+)
+
+DeleteSpaceRequestRequestTypeDef = TypedDict(
+    "DeleteSpaceRequestRequestTypeDef",
+    {
+        "name": str,
     },
 )
 
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -378,15 +373,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -394,56 +388,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -473,126 +453,82 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+GetSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "GetSourceRepositoryRequestRequestTypeDef",
     {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
     },
 )
 
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runtime": str,
+        "name": str,
     },
-    total=False,
 )
 
-ListAccessTokensRequestRequestTypeDef = TypedDict(
-    "ListAccessTokensRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+ListAccessTokensRequestRequestTypeDef = TypedDict(
+    "ListAccessTokensRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -610,39 +546,14 @@
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -682,80 +593,33 @@
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
-
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -781,41 +645,16 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -833,138 +672,307 @@
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
+        "displayName": str,
+        "description": str,
     },
 )
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
+
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+    },
+)
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "displayName": str,
         "description": str,
     },
     total=False,
 )
 
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySessionResponseTypeDef = TypedDict(
-    "VerifySessionResponseTypeDef",
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
     {
-        "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
+UpdateSpaceResponseTypeDef = TypedDict(
+    "UpdateSpaceResponseTypeDef",
     {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySessionResponseTypeDef = TypedDict(
+    "VerifySessionResponseTypeDef",
+    {
+        "identity": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1014,29 +1022,14 @@
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1066,15 +1059,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1097,49 +1090,36 @@
 
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
-
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1149,122 +1129,238 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
+)
+
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
     total=False,
 )
 
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
     pass
 
 
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
 ):
     pass
 
 
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
@@ -1297,42 +1393,42 @@
 
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1343,19 +1439,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -32,117 +32,121 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryRequestRequestTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectRequestRequestTypeDef",
+    "DeleteSourceRepositoryRequestRequestTypeDef",
+    "DeleteSpaceRequestRequestTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryRequestRequestTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "IdeConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
+    "UpdateProjectRequestRequestTypeDef",
+    "UpdateSpaceRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
+    "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
-    "UpdateDevEnvironmentResponseTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
+    "UpdateDevEnvironmentResponseTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -154,22 +158,22 @@
 )
 
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -198,24 +202,14 @@
     },
     total=False,
 )
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -228,25 +222,14 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -262,24 +245,35 @@
 
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
+_RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
     {
-        "ref": str,
+        "spaceName": str,
+        "projectName": str,
         "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSourceRepositoryRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class CreateSourceRepositoryRequestRequestTypeDef(
+    _RequiredCreateSourceRepositoryRequestRequestTypeDef,
+    _OptionalCreateSourceRepositoryRequestRequestTypeDef,
+):
+    pass
 
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -289,51 +283,54 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
+DeleteProjectRequestRequestTypeDef = TypedDict(
+    "DeleteProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+
+DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "DeleteSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+    },
+)
+
+DeleteSpaceRequestRequestTypeDef = TypedDict(
+    "DeleteSpaceRequestRequestTypeDef",
+    {
+        "name": str,
     },
 )
 
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -363,15 +360,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -379,54 +375,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -454,124 +438,82 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+GetSourceRepositoryRequestRequestTypeDef = TypedDict(
+    "GetSourceRepositoryRequestRequestTypeDef",
     {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
     },
 )
 
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+IdeConfigurationOutputTypeDef = TypedDict(
+    "IdeConfigurationOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runtime": str,
+        "name": str,
     },
-    total=False,
 )
 
-ListAccessTokensRequestRequestTypeDef = TypedDict(
-    "ListAccessTokensRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+ListAccessTokensRequestRequestTypeDef = TypedDict(
+    "ListAccessTokensRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -587,37 +529,14 @@
 
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -653,74 +572,33 @@
 )
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -744,39 +622,16 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -792,136 +647,303 @@
 
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
+        "displayName": str,
+        "description": str,
+    },
+)
+
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
     },
 )
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "displayName": str,
         "description": str,
     },
     total=False,
 )
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    {
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    {
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
+    {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDevEnvironmentSessionResponseTypeDef = TypedDict(
     "StopDevEnvironmentSessionResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
         "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySessionResponseTypeDef = TypedDict(
-    "VerifySessionResponseTypeDef",
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
     {
-        "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
+UpdateSpaceResponseTypeDef = TypedDict(
+    "UpdateSpaceResponseTypeDef",
     {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySessionResponseTypeDef = TypedDict(
+    "VerifySessionResponseTypeDef",
+    {
+        "identity": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -967,29 +989,14 @@
 
 class UpdateDevEnvironmentRequestRequestTypeDef(
     _RequiredUpdateDevEnvironmentRequestRequestTypeDef,
     _OptionalUpdateDevEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
-    {
-        "id": str,
-        "spaceName": str,
-        "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "instanceType": InstanceTypeType,
         "persistentStorage": PersistentStorageConfigurationTypeDef,
@@ -1017,15 +1024,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1046,47 +1053,36 @@
     pass
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1096,116 +1092,226 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
+)
+
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
     pass
 
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
 ):
     pass
 
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
@@ -1234,42 +1340,42 @@
     pass
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1280,19 +1386,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeCatalyst 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
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
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,86 +358,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryRequestRequestTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectRequestRequestTypeDef,
+    DeleteSourceRepositoryRequestRequestTypeDef,
+    DeleteSpaceRequestRequestTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryRequestRequestTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    IdeConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
+    UpdateProjectRequestRequestTypeDef,
+    UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
+    UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
-    UpdateDevEnvironmentResponseTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
+    UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.0/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.0/setup.py` & `mypy-boto3-codecatalyst-1.28.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

