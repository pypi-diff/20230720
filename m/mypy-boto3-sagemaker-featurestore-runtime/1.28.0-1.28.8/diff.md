# Comparing `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.0.tar", last modified: Thu Jul  6 21:00:32 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0.tar` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.370420 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-07-06 21:00:32.370420 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.370420 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.370420 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:32.370420 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-06 20:54:50.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:16.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-20 19:47:55.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.008775 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-20 19:47:15.000000 mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/LICENSE` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,22 +302,24 @@
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
+    BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
-    FeatureValueTypeDef,
+    ResponseMetadataTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetRecordRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/README.md` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,22 +270,24 @@
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
+    BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
-    FeatureValueTypeDef,
+    ResponseMetadataTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetRecordRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__init__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/__main__.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8\nVersion:        "
+        " 1.28.8\nBuilder version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime\nOther"
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/client.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,12 +143,13 @@
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
         TargetStores: Sequence[TargetStoreType] = ...,
         TtlDuration: TtlDurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Used for data ingestion into the `FeatureStore`.
+        The `PutRecord` API is used to ingest a list of `Records` into your feature
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#put_record)
         """
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/client.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -133,12 +133,13 @@
         *,
         FeatureGroupName: str,
         Record: Sequence[FeatureValueTypeDef],
         TargetStores: Sequence[TargetStoreType] = ...,
         TtlDuration: TtlDurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Used for data ingestion into the `FeatureStore`.
+        The `PutRecord` API is used to ingest a list of `Records` into your feature
+        group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client.put_record)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/client/#put_record)
         """
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/literals.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,15 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,15 @@
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

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchGetRecordErrorTypeDef",
+    "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
-    "FeatureValueTypeDef",
+    "ResponseMetadataTypeDef",
+    "FeatureValueOutputTypeDef",
     "DeleteRecordRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "FeatureValueTypeDef",
     "GetRecordRequestRequestTypeDef",
     "TtlDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetRecordRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
@@ -49,14 +51,23 @@
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
+    {
+        "FeatureGroupName": str,
+        "RecordIdentifiersValueAsString": List[str],
+        "FeatureNames": List[str],
+    },
+)
+
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -71,16 +82,27 @@
 
 class BatchGetRecordIdentifierTypeDef(
     _RequiredBatchGetRecordIdentifierTypeDef, _OptionalBatchGetRecordIdentifierTypeDef
 ):
     pass
 
 
-FeatureValueTypeDef = TypedDict(
-    "FeatureValueTypeDef",
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
+FeatureValueOutputTypeDef = TypedDict(
+    "FeatureValueOutputTypeDef",
     {
         "FeatureName": str,
         "ValueAsString": str,
     },
 )
 
 _RequiredDeleteRecordRequestRequestTypeDef = TypedDict(
@@ -103,18 +125,19 @@
 
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+FeatureValueTypeDef = TypedDict(
+    "FeatureValueTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FeatureName": str,
+        "ValueAsString": str,
     },
 )
 
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
@@ -141,25 +164,14 @@
     "TtlDurationTypeDef",
     {
         "Unit": TtlDurationUnitType,
         "Value": int,
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
 _RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRecordRequestRequestTypeDef",
     {
         "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
     },
 )
 _OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
@@ -173,43 +185,37 @@
 
 class BatchGetRecordRequestRequestTypeDef(
     _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "FeatureGroupName": str,
-        "RecordIdentifierValueAsString": str,
-        "Record": List[FeatureValueTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
+
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
+        "FeatureGroupName": str,
+        "RecordIdentifierValueAsString": str,
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
-        "Record": List[FeatureValueTypeDef],
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
@@ -233,11 +239,11 @@
 
 
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
-        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -24,22 +24,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchGetRecordErrorTypeDef",
+    "BatchGetRecordIdentifierOutputTypeDef",
     "BatchGetRecordIdentifierTypeDef",
-    "FeatureValueTypeDef",
+    "ResponseMetadataTypeDef",
+    "FeatureValueOutputTypeDef",
     "DeleteRecordRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "FeatureValueTypeDef",
     "GetRecordRequestRequestTypeDef",
     "TtlDurationTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetRecordRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "BatchGetRecordResultDetailTypeDef",
     "GetRecordResponseTypeDef",
     "PutRecordRequestRequestTypeDef",
     "BatchGetRecordResponseTypeDef",
 )
 
 BatchGetRecordErrorTypeDef = TypedDict(
@@ -48,14 +50,23 @@
         "FeatureGroupName": str,
         "RecordIdentifierValueAsString": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
 
+BatchGetRecordIdentifierOutputTypeDef = TypedDict(
+    "BatchGetRecordIdentifierOutputTypeDef",
+    {
+        "FeatureGroupName": str,
+        "RecordIdentifiersValueAsString": List[str],
+        "FeatureNames": List[str],
+    },
+)
+
 _RequiredBatchGetRecordIdentifierTypeDef = TypedDict(
     "_RequiredBatchGetRecordIdentifierTypeDef",
     {
         "FeatureGroupName": str,
         "RecordIdentifiersValueAsString": Sequence[str],
     },
 )
@@ -68,16 +79,27 @@
 )
 
 class BatchGetRecordIdentifierTypeDef(
     _RequiredBatchGetRecordIdentifierTypeDef, _OptionalBatchGetRecordIdentifierTypeDef
 ):
     pass
 
-FeatureValueTypeDef = TypedDict(
-    "FeatureValueTypeDef",
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
+FeatureValueOutputTypeDef = TypedDict(
+    "FeatureValueOutputTypeDef",
     {
         "FeatureName": str,
         "ValueAsString": str,
     },
 )
 
 _RequiredDeleteRecordRequestRequestTypeDef = TypedDict(
@@ -98,18 +120,19 @@
 )
 
 class DeleteRecordRequestRequestTypeDef(
     _RequiredDeleteRecordRequestRequestTypeDef, _OptionalDeleteRecordRequestRequestTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+FeatureValueTypeDef = TypedDict(
+    "FeatureValueTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FeatureName": str,
+        "ValueAsString": str,
     },
 )
 
 _RequiredGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
@@ -134,25 +157,14 @@
     "TtlDurationTypeDef",
     {
         "Unit": TtlDurationUnitType,
         "Value": int,
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
 _RequiredBatchGetRecordRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRecordRequestRequestTypeDef",
     {
         "Identifiers": Sequence[BatchGetRecordIdentifierTypeDef],
     },
 )
 _OptionalBatchGetRecordRequestRequestTypeDef = TypedDict(
@@ -164,41 +176,37 @@
 )
 
 class BatchGetRecordRequestRequestTypeDef(
     _RequiredBatchGetRecordRequestRequestTypeDef, _OptionalBatchGetRecordRequestRequestTypeDef
 ):
     pass
 
-_RequiredBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_RequiredBatchGetRecordResultDetailTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "FeatureGroupName": str,
-        "RecordIdentifierValueAsString": str,
-        "Record": List[FeatureValueTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchGetRecordResultDetailTypeDef = TypedDict(
-    "_OptionalBatchGetRecordResultDetailTypeDef",
+
+BatchGetRecordResultDetailTypeDef = TypedDict(
+    "BatchGetRecordResultDetailTypeDef",
     {
+        "FeatureGroupName": str,
+        "RecordIdentifierValueAsString": str,
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
     },
-    total=False,
 )
 
-class BatchGetRecordResultDetailTypeDef(
-    _RequiredBatchGetRecordResultDetailTypeDef, _OptionalBatchGetRecordResultDetailTypeDef
-):
-    pass
-
 GetRecordResponseTypeDef = TypedDict(
     "GetRecordResponseTypeDef",
     {
-        "Record": List[FeatureValueTypeDef],
+        "Record": List[FeatureValueOutputTypeDef],
         "ExpiresAt": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecordRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecordRequestRequestTypeDef",
     {
         "FeatureGroupName": str,
@@ -220,11 +228,11 @@
     pass
 
 BatchGetRecordResponseTypeDef = TypedDict(
     "BatchGetRecordResponseTypeDef",
     {
         "Records": List[BatchGetRecordResultDetailTypeDef],
         "Errors": List[BatchGetRecordErrorTypeDef],
-        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "UnprocessedIdentifiers": List[BatchGetRecordIdentifierOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-featurestore-runtime
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-featurestore-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-featurestore-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-featurestore-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-featurestore-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerFeatureStoreRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
+[boto3.SageMakerFeatureStoreRuntime 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
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
 [mypy-boto3-sagemaker-featurestore-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_featurestore_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,22 +302,24 @@
 `mypy_boto3_sagemaker_featurestore_runtime.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_sagemaker_featurestore_runtime.type_defs import (
     BatchGetRecordErrorTypeDef,
+    BatchGetRecordIdentifierOutputTypeDef,
     BatchGetRecordIdentifierTypeDef,
-    FeatureValueTypeDef,
+    ResponseMetadataTypeDef,
+    FeatureValueOutputTypeDef,
     DeleteRecordRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FeatureValueTypeDef,
     GetRecordRequestRequestTypeDef,
     TtlDurationTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetRecordRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     BatchGetRecordResultDetailTypeDef,
     GetRecordResponseTypeDef,
     PutRecordRequestRequestTypeDef,
     BatchGetRecordResponseTypeDef,
 )
```

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/mypy_boto3_sagemaker_featurestore_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-featurestore-runtime-1.28.0/setup.py` & `mypy-boto3-sagemaker-featurestore-runtime-1.28.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-featurestore-runtime",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_sagemaker_featurestore_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SageMakerFeatureStoreRuntime 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

