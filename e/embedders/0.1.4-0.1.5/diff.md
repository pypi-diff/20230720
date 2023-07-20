# Comparing `tmp/embedders-0.1.4-py2.py3-none-any.whl.zip` & `tmp/embedders-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23364 bytes, number of entries: 18
+Zip file size: 23956 bytes, number of entries: 18
 -rw-r--r--  2.0 unx     6934 b- defN 22-Oct-30 14:35 embedders/__init__.py
 -rw-r--r--  2.0 unx      143 b- defN 22-Sep-07 08:19 embedders/enums.py
 -rw-r--r--  2.0 unx      399 b- defN 22-Jul-22 10:51 embedders/util.py
 -rw-r--r--  2.0 unx      178 b- defN 22-Sep-07 08:19 embedders/classification/__init__.py
--rw-r--r--  2.0 unx     3658 b- defN 23-May-14 20:53 embedders/classification/contextual.py
+-rw-r--r--  2.0 unx     6746 b- defN 23-Jul-20 21:17 embedders/classification/contextual.py
 -rw-r--r--  2.0 unx     3285 b- defN 22-Jul-22 10:51 embedders/classification/count_based.py
 -rw-r--r--  2.0 unx     2170 b- defN 22-Jul-22 10:51 embedders/classification/reduce.py
 -rw-r--r--  2.0 unx      670 b- defN 22-Sep-07 08:19 embedders/extraction/__init__.py
 -rw-r--r--  2.0 unx    14751 b- defN 22-Oct-22 16:42 embedders/extraction/contextual.py
 -rw-r--r--  2.0 unx     1784 b- defN 22-Jul-22 10:51 embedders/extraction/count_based.py
 -rw-r--r--  2.0 unx     2705 b- defN 22-Jul-22 10:51 embedders/extraction/reduce.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-22 10:51 embedders/samples/__init__.py
 -rw-r--r--  2.0 unx     6158 b- defN 22-Jul-22 10:51 embedders/samples/clickbait.py
--rw-r--r--  2.0 unx    11340 b- defN 23-May-14 20:54 embedders-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     7028 b- defN 23-May-14 20:54 embedders-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 20:54 embedders-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-14 20:54 embedders-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1526 b- defN 23-May-14 20:54 embedders-0.1.4.dist-info/RECORD
-18 files, 62849 bytes uncompressed, 20850 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx    11340 b- defN 23-Jul-20 21:18 embedders-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7028 b- defN 23-Jul-20 21:18 embedders-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-20 21:18 embedders-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-20 21:18 embedders-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1526 b- defN 23-Jul-20 21:18 embedders-0.1.5.dist-info/RECORD
+18 files, 65937 bytes uncompressed, 21442 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: embedders/samples/__init__.py
 Comment: 
 
 Filename: embedders/samples/clickbait.py
 Comment: 
 
-Filename: embedders-0.1.4.dist-info/LICENSE
+Filename: embedders-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: embedders-0.1.4.dist-info/METADATA
+Filename: embedders-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: embedders-0.1.4.dist-info/WHEEL
+Filename: embedders-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: embedders-0.1.4.dist-info/top_level.txt
+Filename: embedders-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: embedders-0.1.4.dist-info/RECORD
+Filename: embedders-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedders/classification/contextual.py

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Generator
+from typing import List, Optional, Union, Generator
 from sentence_transformers import SentenceTransformer
 from embedders import util
 from embedders.classification import SentenceEmbedder
 from spacy.tokens.doc import Doc
 import torch
 import openai
 from openai import error as openai_error
@@ -31,20 +31,83 @@
 
 class HuggingFaceSentenceEmbedder(TransformerSentenceEmbedder):
     def __init__(self, config_string: str, batch_size: int = 128):
         super().__init__(config_string, batch_size)
 
 
 class OpenAISentenceEmbedder(SentenceEmbedder):
-    def __init__(self, openai_api_key: str, model_name: str, batch_size: int = 128):
+    def __init__(
+        self,
+        openai_api_key: str,
+        model_name: str,
+        batch_size: int = 128,
+        api_base: Optional[str] = None,
+        api_type: Optional[str] = None,
+        api_version: Optional[str] = None,
+    ):
+        """
+        Embeds documents using large language models from https://openai.com or https://azure.microsoft.com
+
+        Args:
+            openai_api_key (str): API key from OpenAI or Azure
+            model_name (str): Name of the embedding model from OpenAI (e.g. text-embedding-ada-002) or the name of your Azure endpoint
+            batch_size (int, optional): Defines the number of conversions after which the embedder yields. Defaults to 128.
+            api_base (str, optional): If you use Azure, you need to provide the base URL of your Azure endpoint (e.g. 'https://azureopenkernai.openai.azure.com/'). Defaults to None.
+            api_type (str, optional): If you use Azure, you need to provide the type of your Azure endpoint (e.g. 'azure'). Defaults to None.
+            api_version (str, optional): If you use Azure, you need to provide the version of your Azure endpoint (e.g. '2023-05-15'). Defaults to None.
+
+        Raises:
+            Exception: If you use Azure, you need to provide api_type, api_version and api_base.
+
+        Examples:
+            >>> from embedders.classification.contextual import OpenAISentenceEmbedder
+            >>> embedder_openai = OpenAISentenceEmbedder(
+            ...     "my-key-from-openai",
+            ...     "text-embedding-ada-002",
+            ... )
+            >>> embeddings = embedder_openai.transform(["This is a test", "This is another test"])
+            >>> print(embeddings)
+            [[-0.0001, 0.0002, ...], [-0.0001, 0.0002, ...]]
+
+            >>> from embedders.classification.contextual import OpenAISentenceEmbedder
+            >>> embedder_azure = OpenAISentenceEmbedder(
+            ...     "my-key-from-azure",
+            ...     "my-endpoint-name",
+            ...     api_base="https://azureopenkernai.openai.azure.com/",
+            ...     api_type="azure",
+            ...     api_version="2023-05-15",
+            ... )
+            >>> embeddings = embedder_azure.transform(["This is a test", "This is another test"])
+            >>> print(embeddings)
+            [[-0.0001, 0.0002, ...], [-0.0001, 0.0002, ...]]
+
+        """
         super().__init__(batch_size)
         self.model_name = model_name
         self.openai_api_key = openai_api_key
         openai.api_key = self.openai_api_key
 
+        self.use_azure = any(
+            [
+                api_base is not None,
+                api_type is not None,
+                api_version is not None,
+            ]
+        )
+        if self.use_azure:
+            assert (
+                api_type is not None
+                and api_version is not None
+                and api_base is not None
+            ), "If you want to use Azure, you need to provide api_type, api_version and api_base."
+
+            openai.api_base = api_base
+            openai.api_type = api_type
+            openai.api_version = api_version
+
     def __getstate__(self):
         state = self.__dict__.copy()
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.model_name = state["model_name"]
@@ -53,17 +116,22 @@
 
     def _encode(
         self, documents: List[Union[str, Doc]], fit_model: bool
     ) -> Generator[List[List[float]], None, None]:
         for documents_batch in util.batch(documents, self.batch_size):
             documents_batch = [doc.replace("\n", " ") for doc in documents_batch]
             try:
-                response = openai.Embedding.create(
-                    input=documents_batch, model=self.model_name
-                )
+                if self.use_azure:
+                    response = openai.Embedding.create(
+                        input=documents_batch, engine=self.model_name
+                    )
+                else:
+                    response = openai.Embedding.create(
+                        input=documents_batch, model=self.model_name
+                    )
                 embeddings = [entry["embedding"] for entry in response["data"]]
                 yield embeddings
             except openai_error.AuthenticationError:
                 raise Exception(
                     "OpenAI API key is invalid. Please provide a valid API key in the constructor of OpenAISentenceEmbedder."
                 )
```

## Comparing `embedders-0.1.4.dist-info/LICENSE` & `embedders-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedders-0.1.4.dist-info/METADATA` & `embedders-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedders
-Version: 0.1.4
+Version: 0.1.5
 Summary: High-level API for creating sentence and token embeddings
 Home-page: https://github.com/code-kern-ai/embedders
 Author: Johannes Hötter
 Author-email: johannes.hoetter@kern.ai
 License: UNKNOWN
 Keywords: kern,machine learning,representation learning,python
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Requires-Dist: tqdm
 Requires-Dist: transformers (<5.0.0,>=4.6.0)
 Requires-Dist: openai
 Requires-Dist: cohere
 
 ![embedders](https://uploads-ssl.webflow.com/61e47fafb12bd56b40022a49/626ee1c35a3abf0ca872486d_embedder-banner.png)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![pypi 0.1.4](https://img.shields.io/badge/pypi-0.1.4-red.svg)](https://pypi.org/project/embedders/0.1.4/)
+[![pypi 0.1.5](https://img.shields.io/badge/pypi-0.1.5-red.svg)](https://pypi.org/project/embedders/0.1.5/)
 
 # ⚗️ embedders
 
 With `embedders`, you can easily convert your texts into sentence- or token-level embeddings within a few lines of code. Use cases for this include similarity search between texts, information extraction such as named entity recognition, or basic text classification.
 
 ## Prerequisites
```

## Comparing `embedders-0.1.4.dist-info/RECORD` & `embedders-0.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 embedders/__init__.py,sha256=k16jAhhQlZWXuJKGP2mIvhOWI7zxhk_B97i4cNlCYIc,6934
 embedders/enums.py,sha256=uGhAUUum4w6fNKZa8gqXBlnPTnKbZhFsbIEFdDdXzcc,143
 embedders/util.py,sha256=XnpCyf5U0z7EWmgOQJ46v1diI6JXsYGYFBI2c_-nycc,399
 embedders/classification/__init__.py,sha256=A0qKkBCI9ENcyY3D2H2at8IOLEpK112uwN2iJEOoG7c,178
-embedders/classification/contextual.py,sha256=BsvLPvn4RLpH387qoVcKICNo-wV8ziWU2auD6Xwud74,3658
+embedders/classification/contextual.py,sha256=s_9IFnrwYOc6WtBdgmNg9vuZgahsuJVaG-OfC2mUHyg,6746
 embedders/classification/count_based.py,sha256=uaGTdwljsA1cXlYWhtFQhuAGUtct12j3qnXh-mfIq9k,3285
 embedders/classification/reduce.py,sha256=hXXoK_vS-tzCmZmPFbfQ_pML2bGzqL2w-UrWhqn5gV4,2170
 embedders/extraction/__init__.py,sha256=D5YDQTnOTa7qO76CSXyqHCTtmIP559crWHXCBkTo5Co,670
 embedders/extraction/contextual.py,sha256=r0wviuKgssOqpx32iVzb5IRrTziR5TpDs-0a2TlyQWo,14751
 embedders/extraction/count_based.py,sha256=uwhg2r3D-My3faMv81OHCDkbQyjTWv3Uomft6BsxKik,1784
 embedders/extraction/reduce.py,sha256=iezo-xOkYfeuuio4O_JSUEeBfJHG6Iw1MqUmpS5enwk,2705
 embedders/samples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 embedders/samples/clickbait.py,sha256=IiivTTmb3zIUaurod3L0ADruCQuXtHGXsU4fW4IrFQc,6158
-embedders-0.1.4.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
-embedders-0.1.4.dist-info/METADATA,sha256=CEL0LOnk830TMBPQIbWFK5305MuC8ITMpIcf6fggMq8,7028
-embedders-0.1.4.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-embedders-0.1.4.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
-embedders-0.1.4.dist-info/RECORD,,
+embedders-0.1.5.dist-info/LICENSE,sha256=JYWPdm7R90tTEXK6muMxOgQBHToBQaLT9rPehcITO4I,11340
+embedders-0.1.5.dist-info/METADATA,sha256=LpUHQp1VWoKv8e3JSlFAymR8taymsEEuNCNHUzgNd_A,7028
+embedders-0.1.5.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+embedders-0.1.5.dist-info/top_level.txt,sha256=iRhfbBg_ZWmtclxcpD-WZe5rD-rvHFHKGkJwcWZM_f0,10
+embedders-0.1.5.dist-info/RECORD,,
```

