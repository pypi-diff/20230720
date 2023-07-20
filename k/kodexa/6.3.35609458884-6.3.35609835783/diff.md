# Comparing `tmp/kodexa-6.3.35609458884.tar.gz` & `tmp/kodexa-6.3.35609835783.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35609458884.tar", max compression
+gzip compressed data, was "kodexa-6.3.35609835783.tar", max compression
```

## Comparing `kodexa-6.3.35609458884.tar` & `kodexa-6.3.35609835783.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-07-20 09:48:32.657626 kodexa-6.3.35609458884/LICENSE
--rw-r--r--   0        0        0     2804 2023-07-20 09:48:32.657626 kodexa-6.3.35609458884/README.md
--rw-r--r--   0        0        0      847 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-07-20 09:48:32.665627 kodexa-6.3.35609458884/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/model/model.py
--rw-r--r--   0        0        0   118200 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/model/objects.py
--rw-r--r--   0        0        0    38744 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111394 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/platform/client.py
--rw-r--r--   0        0        0    28288 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-07-20 09:48:32.669627 kodexa-6.3.35609458884/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-07-20 09:48:32.673627 kodexa-6.3.35609458884/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-07-20 09:48:32.673627 kodexa-6.3.35609458884/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 09:48:32.673627 kodexa-6.3.35609458884/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-07-20 09:49:00.078935 kodexa-6.3.35609458884/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35609458884/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 10:26:27.520209 kodexa-6.3.35609835783/LICENSE
+-rw-r--r--   0        0        0     2804 2023-07-20 10:26:27.520209 kodexa-6.3.35609835783/README.md
+-rw-r--r--   0        0        0      847 2023-07-20 10:26:27.524209 kodexa-6.3.35609835783/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-20 10:26:27.524209 kodexa-6.3.35609835783/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/model/model.py
+-rw-r--r--   0        0        0   118200 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38744 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111395 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28288 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:26:27.528209 kodexa-6.3.35609835783/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-07-20 10:27:01.956382 kodexa-6.3.35609835783/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35609835783/PKG-INFO
```

### Comparing `kodexa-6.3.35609458884/LICENSE` & `kodexa-6.3.35609835783/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/README.md` & `kodexa-6.3.35609835783/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/__init__.py` & `kodexa-6.3.35609835783/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/assistant/assistant.py` & `kodexa-6.3.35609835783/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/connectors/connectors.py` & `kodexa-6.3.35609835783/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/model/__init__.py` & `kodexa-6.3.35609835783/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/model/base.py` & `kodexa-6.3.35609835783/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/model/model.py` & `kodexa-6.3.35609835783/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/model/objects.py` & `kodexa-6.3.35609835783/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/model/persistence.py` & `kodexa-6.3.35609835783/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35609835783/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/platform/client.py` & `kodexa-6.3.35609835783/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 class ClientEndpoint(BaseModel):
     """
     Represents a client endpoint
     """
     client: Optional[Any] = Field(None, exclude=True)
-    ref: Optional[str] = Field(None, exclude=True)
+    ref: Optional[str] = Field(None, exclude=False)
 
     class Config:
         arbitrary_types_allowed = True
 
     def set_client(self, client):
         """
         Set the client that this endpoint is associated with
```

### Comparing `kodexa-6.3.35609458884/kodexa/platform/kodexa.py` & `kodexa-6.3.35609835783/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/ast.py` & `kodexa-6.3.35609835783/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/core.py` & `kodexa-6.3.35609835783/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/lexrules.py` & `kodexa-6.3.35609835783/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/lextab.py` & `kodexa-6.3.35609835783/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/parserules.py` & `kodexa-6.3.35609835783/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/selectors/parsetab.py` & `kodexa-6.3.35609835783/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/spatial/azure_models.py` & `kodexa-6.3.35609835783/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35609835783/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35609835783/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/steps/common.py` & `kodexa-6.3.35609835783/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/testing/test_components.py` & `kodexa-6.3.35609835783/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/kodexa/testing/test_utils.py` & `kodexa-6.3.35609835783/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35609458884/pyproject.toml` & `kodexa-6.3.35609835783/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35609458884"
+version = "6.3.35609835783"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35609458884/PKG-INFO` & `kodexa-6.3.35609835783/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35609458884
+Version: 6.3.35609835783
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

