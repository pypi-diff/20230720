# Comparing `tmp/mypy-boto3-connectcases-1.28.0.tar.gz` & `tmp/mypy-boto3-connectcases-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.28.0.tar", last modified: Thu Jul  6 20:59:19 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.28.0.tar` & `mypy-boto3-connectcases-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.586267 mypy-boto3-connectcases-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-07-06 20:59:19.578267 mypy-boto3-connectcases-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.578267 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29502 2023-07-06 20:37:10.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-07-06 20:37:10.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:09.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.578267 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:19.000000 mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:19.586267 mypy-boto3-connectcases-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:37:08.000000 mypy-boto3-connectcases-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/setup.py
```

### Comparing `mypy-boto3-connectcases-1.28.0/LICENSE` & `mypy-boto3-connectcases-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.0/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectCases 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,103 +333,120 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
+    FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
+    FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
 def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-connectcases-1.28.0/README.md` & `mypy-boto3-connectcases-1.28.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,103 +301,120 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
+    FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
+    FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
 def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
 
     def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
-        Deletes a domain.
+        Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
         """
 
     def generate_presigned_url(
         self,
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
     def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
-        Deletes a domain.
+        Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,15 @@
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

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -258,14 +258,15 @@
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

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 
@@ -78,13 +78,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchcasespaginator)
         """
 
 class SearchRelatedItemsPaginator(Paginator):
@@ -74,13 +74,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,157 +34,163 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
-    "CreateCaseRequestRequestTypeDef",
-    "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
     "UpdateCaseRequestRequestTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
+    "CaseFilterTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
+        "tags": Dict[str, str],
         "type": FieldTypeType,
     },
 )
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "description": str,
-        "tags": Dict[str, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
-
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -195,22 +201,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -236,40 +257,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -285,41 +287,14 @@
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -327,23 +302,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -352,51 +318,78 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "includeContent": bool,
     },
 )
 
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
     },
 )
 
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "emptyValue": Dict[str, Any],
+        "stringValue": str,
+    },
+)
+
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
         "stringValue": str,
     },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
@@ -408,27 +401,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -437,14 +417,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -554,22 +548,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
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
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -605,25 +591,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -674,15 +649,15 @@
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -706,60 +681,140 @@
 
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
-    "BatchPutFieldOptionsRequestRequestTypeDef",
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
     {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
         "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
         "fieldId": str,
-        "options": Sequence[FieldOptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
     {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
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
+BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
+    "BatchPutFieldOptionsRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "fieldId": str,
+        "options": Sequence[FieldOptionTypeDef],
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -797,29 +852,14 @@
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -843,15 +883,23 @@
 
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemOutputTypeDef],
+        "name": str,
     },
 )
 
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
@@ -866,46 +914,78 @@
 )
 
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionOutputTypeDef,
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -940,15 +1020,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -962,38 +1042,33 @@
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "associationTime": datetime,
-        "content": RelatedItemContentTypeDef,
-        "relatedItemId": str,
-        "type": RelatedItemTypeType,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
 )
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
+
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
+        "associationTime": datetime,
+        "content": RelatedItemContentTypeDef,
+        "relatedItemId": str,
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1022,15 +1097,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1045,22 +1120,50 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
+    {
+        "fieldGroup": FieldGroupOutputTypeDef,
+    },
+)
+
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
 
+GetCaseResponseTypeDef = TypedDict(
+    "GetCaseResponseTypeDef",
+    {
+        "fields": List[FieldValueOutputTypeDef],
+        "nextToken": str,
+        "tags": Dict[str, str],
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
+    {
+        "caseId": str,
+        "fields": List[FieldValueOutputTypeDef],
+        "tags": Dict[str, str],
+        "templateId": str,
+    },
+)
+
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
@@ -1089,48 +1192,14 @@
         "greaterThanOrEqualTo": FieldValueTypeDef,
         "lessThan": FieldValueTypeDef,
         "lessThanOrEqualTo": FieldValueTypeDef,
     },
     total=False,
 )
 
-GetCaseResponseTypeDef = TypedDict(
-    "GetCaseResponseTypeDef",
-    {
-        "fields": List[FieldValueTypeDef],
-        "nextToken": str,
-        "tags": Dict[str, str],
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
-    {
-        "caseId": str,
-        "fields": List[FieldValueTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
-
 UpdateCaseRequestRequestTypeDef = TypedDict(
     "UpdateCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
@@ -1153,101 +1222,132 @@
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": List[SectionOutputTypeDef],
     },
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
 
+SearchCasesResponseTypeDef = TypedDict(
+    "SearchCasesResponseTypeDef",
+    {
+        "cases": List[SearchCasesResponseItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-SearchCasesResponseTypeDef = TypedDict(
-    "SearchCasesResponseTypeDef",
+PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
+    "PutCaseEventConfigurationRequestRequestTypeDef",
     {
-        "cases": List[SearchCasesResponseItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domainId": str,
+        "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
-    "PutCaseEventConfigurationRequestRequestTypeDef",
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
     {
-        "domainId": str,
-        "eventBridge": EventBridgeConfigurationTypeDef,
+        "moreInfo": LayoutSectionsOutputTypeDef,
+        "topPanel": LayoutSectionsOutputTypeDef,
     },
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
+    {
+        "basic": BasicLayoutOutputTypeDef,
+    },
+)
+
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
     total=False,
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+GetLayoutResponseTypeDef = TypedDict(
+    "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
+        "content": LayoutContentOutputTypeDef,
+        "layoutArn": str,
+        "layoutId": str,
         "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetLayoutResponseTypeDef = TypedDict(
-    "GetLayoutResponseTypeDef",
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
     {
         "content": LayoutContentTypeDef,
-        "layoutArn": str,
-        "layoutId": str,
+        "domainId": str,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -33,153 +33,163 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
+    "FieldValueUnionOutputTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
+    "FieldValueOutputTypeDef",
     "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
-    "CreateCaseRequestRequestTypeDef",
-    "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
     "UpdateCaseRequestRequestTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
+    "CaseFilterTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
+        "tags": Dict[str, str],
         "type": FieldTypeType,
     },
 )
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "description": str,
-        "tags": Dict[str, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -190,22 +200,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -231,40 +256,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -278,41 +284,14 @@
 )
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -320,23 +299,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -345,51 +315,78 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "includeContent": bool,
     },
 )
 
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
         "type": FieldTypeType,
     },
 )
 
+FieldValueUnionOutputTypeDef = TypedDict(
+    "FieldValueUnionOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "emptyValue": Dict[str, Any],
+        "stringValue": str,
+    },
+)
+
 FieldValueUnionTypeDef = TypedDict(
     "FieldValueUnionTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
         "stringValue": str,
     },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
@@ -401,27 +398,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -430,14 +414,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -539,22 +537,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
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
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -588,25 +578,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -655,15 +634,15 @@
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -685,60 +664,140 @@
     pass
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
-    "BatchPutFieldOptionsRequestRequestTypeDef",
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
     {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
         "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
         "fieldId": str,
-        "options": Sequence[FieldOptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
     {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
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
+BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
+    "BatchPutFieldOptionsRequestRequestTypeDef",
+    {
+        "domainId": str,
+        "fieldId": str,
+        "options": Sequence[FieldOptionTypeDef],
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -774,29 +833,14 @@
 )
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -818,15 +862,23 @@
     pass
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemOutputTypeDef],
+        "name": str,
     },
 )
 
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
@@ -839,46 +891,78 @@
     },
     total=False,
 )
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FieldValueOutputTypeDef = TypedDict(
+    "FieldValueOutputTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionOutputTypeDef,
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
         "value": FieldValueUnionTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -911,15 +995,15 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
@@ -931,36 +1015,33 @@
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "associationTime": datetime,
-        "content": RelatedItemContentTypeDef,
-        "relatedItemId": str,
-        "type": RelatedItemTypeType,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
 )
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
+
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
+        "associationTime": datetime,
+        "content": RelatedItemContentTypeDef,
+        "relatedItemId": str,
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -987,15 +1068,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1008,22 +1089,50 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
+    {
+        "fieldGroup": FieldGroupOutputTypeDef,
+    },
+)
+
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
 
+GetCaseResponseTypeDef = TypedDict(
+    "GetCaseResponseTypeDef",
+    {
+        "fields": List[FieldValueOutputTypeDef],
+        "nextToken": str,
+        "tags": Dict[str, str],
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
+    {
+        "caseId": str,
+        "fields": List[FieldValueOutputTypeDef],
+        "tags": Dict[str, str],
+        "templateId": str,
+    },
+)
+
 _RequiredCreateCaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCaseRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
         "templateId": str,
     },
@@ -1050,46 +1159,14 @@
         "greaterThanOrEqualTo": FieldValueTypeDef,
         "lessThan": FieldValueTypeDef,
         "lessThanOrEqualTo": FieldValueTypeDef,
     },
     total=False,
 )
 
-GetCaseResponseTypeDef = TypedDict(
-    "GetCaseResponseTypeDef",
-    {
-        "fields": List[FieldValueTypeDef],
-        "nextToken": str,
-        "tags": Dict[str, str],
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
-    {
-        "caseId": str,
-        "fields": List[FieldValueTypeDef],
-        "templateId": str,
-    },
-)
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
-    {
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
-):
-    pass
-
 UpdateCaseRequestRequestTypeDef = TypedDict(
     "UpdateCaseRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
@@ -1110,101 +1187,132 @@
 )
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": List[SectionOutputTypeDef],
     },
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
 
+SearchCasesResponseTypeDef = TypedDict(
+    "SearchCasesResponseTypeDef",
+    {
+        "cases": List[SearchCasesResponseItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CaseFilterTypeDef = TypedDict(
     "CaseFilterTypeDef",
     {
         "andAll": Sequence[Dict[str, Any]],
         "field": FieldFilterTypeDef,
         "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-SearchCasesResponseTypeDef = TypedDict(
-    "SearchCasesResponseTypeDef",
+PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
+    "PutCaseEventConfigurationRequestRequestTypeDef",
     {
-        "cases": List[SearchCasesResponseItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domainId": str,
+        "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
-    "PutCaseEventConfigurationRequestRequestTypeDef",
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
     {
-        "domainId": str,
-        "eventBridge": EventBridgeConfigurationTypeDef,
+        "moreInfo": LayoutSectionsOutputTypeDef,
+        "topPanel": LayoutSectionsOutputTypeDef,
     },
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
+    {
+        "basic": BasicLayoutOutputTypeDef,
+    },
+)
+
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
     total=False,
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+GetLayoutResponseTypeDef = TypedDict(
+    "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
+        "content": LayoutContentOutputTypeDef,
+        "layoutArn": str,
+        "layoutId": str,
         "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetLayoutResponseTypeDef = TypedDict(
-    "GetLayoutResponseTypeDef",
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
     {
         "content": LayoutContentTypeDef,
-        "layoutArn": str,
-        "layoutId": str,
+        "domainId": str,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectCases 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,103 +333,120 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
+    FieldValueUnionOutputTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
+    FieldValueOutputTypeDef,
     FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
-    CreateCaseRequestRequestTypeDef,
-    FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
     UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
 def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-connectcases-1.28.0/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.0/setup.py` & `mypy-boto3-connectcases-1.28.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

