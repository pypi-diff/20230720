# Comparing `tmp/openssm_dev-0.1.6.6.tar.gz` & `tmp/openssm_dev-0.1.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm_dev-0.1.6.6.tar", max compression
+gzip compressed data, was "openssm_dev-0.1.6.dev0.tar", max compression
```

## Comparing `openssm_dev-0.1.6.6.tar` & `openssm_dev-0.1.6.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     7181 2023-07-20 00:43:00.830273 openssm_dev-0.1.6.6/README.md
--rw-r--r--   0        0        0       79 2023-07-11 05:54:22.327687 openssm_dev-0.1.6.6/openssm/Makefile
--rw-r--r--   0        0        0     2553 2023-07-11 05:54:22.327950 openssm_dev-0.1.6.6/openssm/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.482785 openssm_dev-0.1.6.6/openssm/__init__.py
--rw-r--r--   0        0        0      899 2023-07-18 02:22:03.792028 openssm_dev-0.1.6.6/openssm/config.py
--rw-r--r--   0        0        0      754 2023-07-18 02:22:03.792311 openssm_dev-0.1.6.6/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
--rw-r--r--   0        0        0      789 2023-07-18 02:22:03.792644 openssm_dev-0.1.6.6/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
--rw-r--r--   0        0        0     1010 2023-07-18 02:22:03.792852 openssm_dev-0.1.6.6/openssm/contrib/ssms/mri_operator_ssm/__init__.py
--rw-r--r--   0        0        0     1610 2023-07-18 02:22:03.793056 openssm_dev-0.1.6.6/openssm/contrib/ssms/semiconductor_ssm/__init__.py
--rw-r--r--   0        0        0       30 2023-07-20 07:31:42.149227 openssm_dev-0.1.6.6/openssm/core/__init__.py
--rw-r--r--   0        0        0       20 2023-07-20 07:31:42.149881 openssm_dev-0.1.6.6/openssm/core/adapter/__init__.py
--rw-r--r--   0        0        0     2340 2023-07-20 07:31:42.150525 openssm_dev-0.1.6.6/openssm/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0     3647 2023-07-20 07:31:42.151118 openssm_dev-0.1.6.6/openssm/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     4994 2023-07-20 17:33:52.835440 openssm_dev-0.1.6.6/openssm/core/adapter/llama_index_adapter.py
--rw-r--r--   0        0        0       20 2023-07-20 07:31:42.152588 openssm_dev-0.1.6.6/openssm/core/backend/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-20 07:31:42.153087 openssm_dev-0.1.6.6/openssm/core/backend/abstract_backend.py
--rw-r--r--   0        0        0     1806 2023-07-20 07:31:42.153690 openssm_dev-0.1.6.6/openssm/core/backend/base_backend.py
--rw-r--r--   0        0        0     3298 2023-07-20 17:33:52.835843 openssm_dev-0.1.6.6/openssm/core/backend/document_backend.py
--rw-r--r--   0        0        0     1068 2023-07-20 07:31:42.154375 openssm_dev-0.1.6.6/openssm/core/backend/text_backend.py
--rw-r--r--   0        0        0       23 2023-07-20 07:31:42.154973 openssm_dev-0.1.6.6/openssm/core/inferencer/__init__.py
--rw-r--r--   0        0        0      838 2023-07-20 05:02:58.109206 openssm_dev-0.1.6.6/openssm/core/inferencer/abstract_inferencer.py
--rw-r--r--   0        0        0      641 2023-07-20 07:31:42.155747 openssm_dev-0.1.6.6/openssm/core/inferencer/base_inferencer.py
--rw-r--r--   0        0        0       36 2023-07-20 07:31:42.156277 openssm_dev-0.1.6.6/openssm/core/slm/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-20 07:31:42.156807 openssm_dev-0.1.6.6/openssm/core/slm/abstract_slm.py
--rw-r--r--   0        0        0     5458 2023-07-20 17:33:52.836229 openssm_dev-0.1.6.6/openssm/core/slm/base_slm.py
--rw-r--r--   0        0        0     6792 2023-07-20 05:02:58.111898 openssm_dev-0.1.6.6/openssm/core/slm/huggingface_slm.py
--rw-r--r--   0        0        0       21 2023-07-20 07:31:42.157922 openssm_dev-0.1.6.6/openssm/core/slm/memory/__init__.py
--rw-r--r--   0        0        0      658 2023-07-20 07:31:42.158427 openssm_dev-0.1.6.6/openssm/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     1897 2023-07-20 07:31:42.159054 openssm_dev-0.1.6.6/openssm/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     2258 2023-07-20 07:31:42.159681 openssm_dev-0.1.6.6/openssm/core/slm/openai_slm.py
--rw-r--r--   0        0        0       38 2023-07-20 07:31:42.160386 openssm_dev-0.1.6.6/openssm/core/ssm/__init__.py
--rw-r--r--   0        0        0     2440 2023-07-20 07:31:42.160849 openssm_dev-0.1.6.6/openssm/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     3352 2023-07-20 07:31:42.161570 openssm_dev-0.1.6.6/openssm/core/ssm/base_ssm.py
--rw-r--r--   0        0        0      812 2023-07-20 19:21:00.770309 openssm_dev-0.1.6.6/openssm/core/ssm/gpt3_llama_index_ssm.py
--rw-r--r--   0        0        0     1360 2023-07-20 07:31:42.162899 openssm_dev-0.1.6.6/openssm/core/ssm/huggingface_ssm.py
--rw-r--r--   0        0        0     1376 2023-07-20 07:31:42.163688 openssm_dev-0.1.6.6/openssm/core/ssm/openai_ssm.py
--rw-r--r--   0        0        0       58 2023-07-05 16:04:01.488477 openssm_dev-0.1.6.6/openssm/industrial/interpretability/README.md
--rw-r--r--   0        0        0       60 2023-07-05 16:04:01.488662 openssm_dev-0.1.6.6/openssm/industrial/monitoring/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488770 openssm_dev-0.1.6.6/openssm/industrial/security/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488908 openssm_dev-0.1.6.6/openssm/industrial/security/audit/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.489033 openssm_dev-0.1.6.6/openssm/industrial/security/best_practices/README.md
--rw-r--r--   0        0        0       63 2023-07-05 16:04:01.489309 openssm_dev-0.1.6.6/openssm/integration/README.md
--rw-r--r--   0        0        0     3574 2023-07-05 16:04:01.489472 openssm_dev-0.1.6.6/openssm/integration/llamaindex/README.md
--rw-r--r--   0        0        0       34 2023-07-05 16:04:01.489708 openssm_dev-0.1.6.6/openssm/integration/testing_tools/README.md
--rw-r--r--   0        0        0     1572 2023-07-20 19:22:02.389457 openssm_dev-0.1.6.6/pyproject.toml
--rw-r--r--   0        0        0     7869 1970-01-01 00:00:00.000000 openssm_dev-0.1.6.6/PKG-INFO
+-rw-r--r--   0        0        0     7181 2023-07-19 02:34:22.673459 openssm_dev-0.1.6.dev0/README.md
+-rw-r--r--   0        0        0       79 2023-07-11 05:54:22.327687 openssm_dev-0.1.6.dev0/openssm/Makefile
+-rw-r--r--   0        0        0     2553 2023-07-11 05:54:22.327950 openssm_dev-0.1.6.dev0/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.482785 openssm_dev-0.1.6.dev0/openssm/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-18 02:22:03.792028 openssm_dev-0.1.6.dev0/openssm/config.py
+-rw-r--r--   0        0        0      754 2023-07-18 02:22:03.792311 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-18 02:22:03.792644 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-18 02:22:03.792852 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/mri_operator_ssm/__init__.py
+-rw-r--r--   0        0        0     1610 2023-07-18 02:22:03.793056 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/semiconductor_ssm/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-05 16:04:01.482973 openssm_dev-0.1.6.dev0/openssm/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.768495 openssm_dev-0.1.6.dev0/openssm/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2199 2023-07-19 02:43:24.231241 openssm_dev-0.1.6.dev0/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0     3401 2023-07-19 02:43:24.231585 openssm_dev-0.1.6.dev0/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     4001 2023-07-19 03:54:14.438862 openssm_dev-0.1.6.dev0/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.769364 openssm_dev-0.1.6.dev0/openssm/core/backend/__init__.py
+-rw-r--r--   0        0        0     1194 2023-07-19 02:43:24.231970 openssm_dev-0.1.6.dev0/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0     1635 2023-07-19 02:43:24.232293 openssm_dev-0.1.6.dev0/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0      897 2023-07-19 02:43:24.232711 openssm_dev-0.1.6.dev0/openssm/core/backend/text_backend.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770313 openssm_dev-0.1.6.dev0/openssm/core/inferencer/__init__.py
+-rw-r--r--   0        0        0      720 2023-07-11 05:54:22.329332 openssm_dev-0.1.6.dev0/openssm/core/inferencer/abstract_inferencer.py
+-rw-r--r--   0        0        0      458 2023-07-18 02:22:03.796108 openssm_dev-0.1.6.dev0/openssm/core/inferencer/base_inferencer.py
+-rw-r--r--   0        0        0      442 2023-07-11 20:37:04.252092 openssm_dev-0.1.6.dev0/openssm/core/inferencer/text_formula_inferencer.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770377 openssm_dev-0.1.6.dev0/openssm/core/slm/__init__.py
+-rw-r--r--   0        0        0      885 2023-07-18 02:22:03.796723 openssm_dev-0.1.6.dev0/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0     5007 2023-07-19 02:34:22.688509 openssm_dev-0.1.6.dev0/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     6355 2023-07-19 02:34:22.689111 openssm_dev-0.1.6.dev0/openssm/core/slm/huggingface_slm.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770841 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-19 02:34:22.689574 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     1620 2023-07-18 02:22:03.797836 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     1685 2023-07-19 02:34:22.689924 openssm_dev-0.1.6.dev0/openssm/core/slm/openai_slm.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.771113 openssm_dev-0.1.6.dev0/openssm/core/ssm/__init__.py
+-rw-r--r--   0        0        0     2307 2023-07-18 02:22:03.798567 openssm_dev-0.1.6.dev0/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     3037 2023-07-18 02:22:03.798847 openssm_dev-0.1.6.dev0/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0      471 2023-07-19 03:54:14.439712 openssm_dev-0.1.6.dev0/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0      747 2023-07-18 02:22:03.799477 openssm_dev-0.1.6.dev0/openssm/core/ssm/huggingface_ssm.py
+-rw-r--r--   0        0        0      770 2023-07-18 06:13:04.771412 openssm_dev-0.1.6.dev0/openssm/core/ssm/openai_ssm.py
+-rw-r--r--   0        0        0       58 2023-07-05 16:04:01.488477 openssm_dev-0.1.6.dev0/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-07-05 16:04:01.488662 openssm_dev-0.1.6.dev0/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488770 openssm_dev-0.1.6.dev0/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488908 openssm_dev-0.1.6.dev0/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.489033 openssm_dev-0.1.6.dev0/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-07-05 16:04:01.489309 openssm_dev-0.1.6.dev0/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-07-05 16:04:01.489472 openssm_dev-0.1.6.dev0/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-07-05 16:04:01.489708 openssm_dev-0.1.6.dev0/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0      837 2023-07-19 06:30:05.159596 openssm_dev-0.1.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 openssm_dev-0.1.6.dev0/PKG-INFO
```

### Comparing `openssm_dev-0.1.6.6/README.md` & `openssm_dev-0.1.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/README.md` & `openssm_dev-0.1.6.dev0/openssm/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/config.py` & `openssm_dev-0.1.6.dev0/openssm/config.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/contrib/ssms/mri_operator_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/mri_operator_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/contrib/ssms/semiconductor_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/semiconductor_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/openssm/core/adapter/abstract_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/abstract_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-"""Abstract adapter."""
-
-
 from abc import ABC, abstractmethod
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class AbstractAdapter(ABC):
     """
     The AbstractAdapter serves as the base for all concrete Adapter classes.
     It provides an interface for interaction between the Small Language Model
     (SLM) and the Backend.
     """
 
     @abstractmethod
-    def __repr__(self) -> str:
-        """Return Adapter instance's string representation."""
-
-    @abstractmethod
     def query(self, conversation_id: str, user_input: str) -> list[dict]:
         """
         Queries the backends for a response to the user's input.
         :param user_query: The user's input.
         :return: The backend's response.
         """
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/adapter/base_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/base_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-"""Base adapter."""
-
-
-from typing import Optional
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 from openssm.core.backend.text_backend import TextBackend
 from openssm.core.inferencer.abstract_inferencer import AbstractInferencer
 
 
 class BaseAdapter(AbstractAdapter):
     """Base adapter class for SSMs."""
 
-    def __init__(self, backends: Optional[list[AbstractBackend]] = None):
-        """Initialize adapter with collection of backends."""
+    def __init__(self, backends: list[AbstractBackend] = None):
         self.backends = backends or []
 
-    def __repr__(self) -> str:
-        """Return Adapter instance's string representation."""
-        return 'BaseAdapter'
-
     def query(self, conversation_id: str, user_input: str) -> list[dict]:
         """
         Queries the backends for a response to the user's input.
         :param user_query: The user's input.
         :return: The backend's response.
         """
         responses = [
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/adapter/llama_index_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/llama_index_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-"""Llama Index adapter."""
-
-
-from dataclasses import dataclass
-from itertools import chain
-from typing import Any, Optional
+from typing import Any
 from llama_index.indices.base import BaseIndex
 from llama_index.indices.query.base import BaseQueryEngine
-from llama_index.indices.vector_store.base import VectorStoreIndex
-from llama_index.readers.schema import Document
 from openssm.core.adapter.base_adapter import BaseAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
-from openssm.core.backend.document_backend import DocumentBackend
 
 
 class LlamaIndexAdapter(BaseAdapter):
     """
     The LlamaIndexAdapter is a concrete implementation of the AbstractAdapter
     that uses LlamaIndex.
     """
 
-    def __init__(self, backends: Optional[list[AbstractBackend]] = None):
+    def __init__(self, backends: list[AbstractBackend] = None):
         """Initializes the LlamaIndexAdapter with a specific LlamaIndex."""
         super().__init__(backends)
         self.llama_tuples = []
 
-        # TODO: refactor
-        _llama_documents: list[Document] = list(chain.from_iterable(backend._llama_load_documents()
-                                                for backend in backends
-                                                if isinstance(backend, DocumentBackend)))
-        self.vector_store_index = VectorStoreIndex.from_documents(documents=_llama_documents,
-                                                                  show_progress=True)
-        self.chat_engine = self.vector_store_index.as_chat_engine()
-
-    def __repr__(self) -> str:
-        """Return Adapter instance's string representation."""
-        return 'LlamaIndexAdapter'
-
-    @dataclass
     class _LlamaTuple:
-        index: Optional[BaseIndex] = None
-        query_engine: Optional[BaseQueryEngine] = None
+        index: BaseIndex = None
+        query_engine: BaseQueryEngine = None
 
     def _get_llama_tuples(self) -> list[_LlamaTuple]:
         if self.llama_tuples is None:
             self.llama_tuples = []
         return self.llama_tuples
 
     def _get_indexes(self) -> list[BaseIndex]:
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/backend/abstract_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/abstract_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-"""Abstract backend."""
-
-
 from abc import ABC, abstractmethod
 from openssm.core.inferencer.abstract_inferencer import AbstractInferencer
 
 
 # pylint: disable=duplicate-code
 class AbstractBackend(ABC):
-    """Abstract backend."""
-
-    @abstractmethod
-    def __repr__(self) -> str:
-        """Return Backend instance's string representation."""
-
     @abstractmethod
     def query(self, conversation_id: str, user_input: str) -> list[dict]:
         pass
 
     @abstractmethod
     def load_all(self):
         """
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/backend/base_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/base_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-"""Base backend."""
-
-
 from openssm.core.inferencer.abstract_inferencer import AbstractInferencer
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class BaseBackend(AbstractBackend):
-    """Base backend."""
-
     def __init__(self):
         self.facts = set()
         self.inferencers = set()
         self.heuristics = set()
 
-    def __repr__(self) -> str:
-        """Return Backend instance's string representation."""
-        return 'BaseBackend'
-
     # pylint: disable=unused-argument
     def query(self, conversation_id: str, user_input: str) -> list[dict]:
         return []
 
     def load_all(self):
         """
         The base backend does not load anything.
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/backend/text_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/text_backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-"""Text backend."""
-
-
 from openssm.core.inferencer.abstract_inferencer import AbstractInferencer
 from openssm.core.backend.base_backend import BaseBackend
 
 
 class TextBackend(BaseBackend):
-    """Text backend."""
-
     def __init__(self):
         super().__init__()
         self.texts = set()
 
-    def __repr__(self) -> str:
-        """Return Backend instance's string representation."""
-        return 'TextBackend'
-
     # pylint: disable=unused-argument
     def query(self, conversation_id: str, user_input: str) -> list[dict]:
         responses = [{"item": text} for text in self.texts]
         return responses
 
     def all_texts(self):
         return self.texts
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/inferencer/abstract_inferencer.py` & `openssm_dev-0.1.6.dev0/openssm/core/inferencer/abstract_inferencer.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,14 @@
     The AbstractInferencer serves as the base for all concrete Inferencer
     classes.  The most common inferencer is simply an ML model, but it
     could also be a rule-based system, a fuzzy logic system, or any other
     system that can infer a response from a given input.
     """
 
     @abstractmethod
-    def __repr__(self) -> str:
-        """Return Inferencer instance's string representation."""
-
-    @abstractmethod
     def predict(self, input_data: dict) -> dict:
         """
         Returns a prediction based on the given input.
         """
 
     @abstractmethod
     def load(self, path: str):
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/slm/abstract_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/abstract_slm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-"""Abstract SLM."""
-
-
 from abc import ABC, abstractmethod
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 
 
 class AbstractSLM(ABC):
     """
     The AbstractSLM serves as the base for all concrete Small Language Models
     (SLMs). It provides an interface for natural language communication and
     structured API interactions.
     """
 
     @abstractmethod
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-
-    @abstractmethod
     def get_adapter(self) -> AbstractAdapter:
         """Returns our adapter"""
 
     @abstractmethod
     def set_adapter(self, adapter: AbstractAdapter):
         """Sets our adapter"""
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/slm/base_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/base_slm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-"""Base SLM."""
-
-
 import json
-from typing import Optional
 from openssm.core.slm.abstract_slm import AbstractSLM
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 
 
 class BaseSLM(AbstractSLM):
-    """Base SLM."""
-
-    def __init__(self, adapter: Optional[AbstractAdapter] = None):
+    def __init__(self, adapter: AbstractAdapter = None):
         """
         self.conversations is initialized as a dictionary of conversations,
         where each conversation is a list of user inputs and model replies.
         """
         self.adapter = adapter
         self.conversations = {}
-        self.pass_to_adapter: bool = False
-
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'BaseSLM'
 
     def get_adapter(self) -> AbstractAdapter:
         return self.adapter
 
     def set_adapter(self, adapter: AbstractAdapter):
         self.adapter = adapter
 
@@ -36,20 +25,15 @@
         Send user input to OpenAI's API and return the replies
         """
 
         # If conversation is new, start a new one, else continue from previous
         conversation = self.conversations.get(conversation_id, [])
         conversation.extend(user_input)
 
-        # TODO: refactor
-        if self.pass_to_adapter:
-            response = self.adapter.chat_engine.chat(user_input[0]['content']).response
-            replies = [{'role': 'assistant', 'content': response}]
-        else:
-            replies = self.call_lm_api(conversation)
+        replies = self.call_lm_api(conversation)
 
         # Save response to the conversation
         conversation.extend(replies)
         self.conversations[conversation_id] = conversation
 
         # Return the model's replies
         return replies
@@ -68,22 +52,22 @@
 
     #
     # Helper functions for GPT-like completion models
     #
     def _make_completion_prompt(self, conversation: list[dict]) -> str:
         # print(f"conversation: {conversation}")
         prompt = self._convert_conversation_to_string(conversation)
-        prompt = ("Complete this conversation with the response, "
-                  "up to 2000 words (plus this prompt): "
-                  "{'role': 'assistant', 'content': 'xxx'} format. "
-                  "where 'xxx' is the response. "
-                  "Make sure the entire response is valid JSON, xxx is "
-                  "only a string, and no code of any kind, even if the "
-                  "prompt has code. "
-                  "Escape quotes with \\:\n"
+        prompt = ("Complete this conversation with the response, " +
+                  "up to 2000 words (plus this prompt): " +
+                  "{'role': 'assistant', 'content': 'xxx'} format. " +
+                  "where 'xxx' is the response. " +
+                  "Make sure the entire response is valid JSON, xxx is " +
+                  "only a string, and no code of any kind, even if the " +
+                  "prompt has code. " +
+                  "Escape quotes with \\:\n" +
                   f"{prompt}")
         return prompt
 
     def _convert_conversation_to_string(self, conversation: list[dict]) -> str:
         list_conversation = []
         for item in conversation:
             # print(f"item: {item}")
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/slm/huggingface_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/huggingface_slm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 This module contains the HuggingFaceBaseSLM class, and its subclasses,
 which are SLMs based on models from HugoingFace. The models may be
 served from HuggingFace's model hub, or a private internal server,
 or they may be served locally.
 """
 import json
-from typing import Optional
 import torch
 
 from requests import request
 from transformers import AutoTokenizer, pipeline, AutoModelForCausalLM
 
 from openssm.core.slm.base_slm import BaseSLM
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
@@ -36,15 +35,15 @@
     _not_supported = False
     _local_mode = False
 
     def __init__(self,
                  model_name=None,
                  model_url=None,
                  model_server_token=None,
-                 adapter: Optional[AbstractAdapter] = None):
+                 adapter: AbstractAdapter = None):
 
         super().__init__(adapter)
         if model_name is None:
             raise ValueError("model_name must be specified")
 
         self._local_mode = model_url == "LOCAL"
         self._not_supported = model_url is None or model_url == "NONE"
@@ -74,18 +73,14 @@
             if model_url is None:
                 raise ValueError("model_url must be specified")
             if model_server_token is None:
                 raise ValueError("model_server_token must be specified")
             self.model_url = model_url
             self.model_server_token = model_server_token
 
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'HuggingFaceBaseSLM'
-
     def call_lm_api(self, conversation: list[dict]) -> list[dict]:
         """
         This method calls the API of the underlying language model,
         and returns the response as a list of dicts.
         """
         if self._not_supported:
             reply_dict = {
@@ -118,20 +113,20 @@
                                url=self.model_url,
                                headers=headers,
                                data=data,
                                timeout=10)
 
             if response.status_code == 200:
                 # pylint: disable=invalid-name
-                response_text = response.text.strip()
-                response_dict = json.loads(response_text)
-                if isinstance(response_dict, list):
-                    response_dict = response_dict[0]
+                responseText = response.text.strip()
+                responseDict = json.loads(responseText)
+                if isinstance(responseDict, list):
+                    responseDict = responseDict[0]
 
-                result = self._parse_llm_response(response_text)
+                result = self._parse_llm_response(responseText)
             else:
                 message = 'Model unavailable, try again'
                 result = [{'system': message}]
 
         # print(f"result: {result}")
         return result
 
@@ -148,38 +143,30 @@
     - If hosted locally, set to "LOCAL"
     - If not supported, set to "NONE" (or not set at all)
     """
 
     def __init__(self,
                  model_url=None,
                  model_server_token=None,
-                 adapter: Optional[AbstractAdapter] = None):
+                 adapter: AbstractAdapter = None):
 
         model_name = "tiiuae/falcon-7b"
         model_url = model_url or Config.FALCON7B_MODEL_URL or "NONE"
         model_server_token = model_server_token or Config.FALCON7B_SERVER_TOKEN
 
         super().__init__(model_name=model_name,
                          model_url=model_url,
                          model_server_token=model_server_token,
                          adapter=adapter)
 
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'Falcon7bSLM'
-
 
 class Falcon7bSLMLocal(Falcon7bSLM):
     """
     Provided for convenience, this class is a wrapper for the Falcon7b
     model hosted locally.
     """
 
     def __init__(self,
-                 adapter: Optional[AbstractAdapter] = None):
+                 adapter: AbstractAdapter = None):
         super().__init__(model_url="LOCAL",
                          model_server_token=None,
                          adapter=adapter)
-
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'Falcon7bSLMLocal'
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/slm/openai_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/openai_slm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,37 @@
-"""OpenAI-based SLM."""
-
-
-from typing import Optional
 import openai
 from openssm.core.slm.base_slm import BaseSLM
 from openssm.config import Config
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 
 
 class GPT3BaseSLM(BaseSLM):
-    """Base GPT3-based SLM."""
-
-    def __init__(self, adapter: Optional[AbstractAdapter] = None):
+    def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
         if Config.OPENAI_API_KEY is None:
             raise ValueError("Config.OPENAI_API_KEY is not set")
         openai.api_key = Config.OPENAI_API_KEY
 
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'GPT3BaseSLM'
-
 
 class GPT3ChatCompletionSLM(GPT3BaseSLM):
-    """GPT3-based Chat Completion SLM."""
-
-    def __init__(self, adapter: Optional[AbstractAdapter] = None):
+    def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
 
     def call_lm_api(self, conversation: list[dict]) -> list[dict]:
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=conversation,
             # max_tokens=150,
             temperature=0.7
         )
         return [response.choices[0].message]
 
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'GPT3ChatCompletionSLM'
-
 
 class GPT3CompletionSLM(GPT3BaseSLM):
-    """GPT3-based Completion SLM."""
-
-    def __init__(self, adapter: Optional[AbstractAdapter] = None):
+    def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
 
     def call_lm_api(self, conversation: list[dict]) -> list[dict]:
         prompt = self._make_completion_prompt(conversation)
 
         response = openai.Completion.create(
             engine="text-davinci-002",
@@ -65,11 +47,7 @@
 
         if len(replies) == 0 or len(replies[0]) == 0:
             replies = [{'role': 'assistant', 'content': 'I got nothing.'}]
 
         # print(f"replies: {replies}")
 
         return replies
-
-    def __repr__(self) -> str:
-        """Return SLM instance's string representation."""
-        return 'GPT3CompletionSLM'
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/ssm/abstract_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/abstract_ssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-"""Abstract SSM."""
-
-
 from abc import ABC, abstractmethod
 from openssm.core.slm.abstract_slm import AbstractSLM
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class AbstractSSM(ABC):
     """
     The AbstractSSM serves as the base for all concrete Small Specialist
     Models (SSMs).
     """
 
     @abstractmethod
-    def __repr__(self) -> str:
-        """Return SSM instance's string representation."""
-
-    @abstractmethod
     def get_slm(self) -> AbstractSLM:
         """Returns our small language model (SLM)"""
 
     @abstractmethod
     def get_adapter(self) -> AbstractAdapter:
         """Returns our adapter"""
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/ssm/base_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/base_ssm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-"""Base SSM."""
-
-
-from typing import Optional
 from openssm.core.ssm.abstract_ssm import AbstractSSM
 from openssm.core.slm.abstract_slm import AbstractSLM
 from openssm.core.adapter.abstract_adapter import AbstractAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 from openssm.core.slm.base_slm import BaseSLM
 from openssm.core.adapter.base_adapter import BaseAdapter
 from openssm.core.backend.base_backend import BaseBackend
 
 
 class BaseSSM(AbstractSSM):
-    """Base SSM."""
-
     def __init__(self,
-                 slm: Optional[AbstractSLM] = None,
-                 adapter: Optional[AbstractAdapter] = None,
-                 backends: Optional[list[AbstractBackend]] = None):
+                 slm: AbstractSLM = None,
+                 adapter: AbstractAdapter = None,
+                 backends: list[AbstractBackend] = None):
         self.slm = slm or BaseSLM()
         self.slm.set_adapter(adapter or BaseAdapter())
         self.get_adapter().set_backends(backends or [BaseBackend()])
 
-    def __repr__(self) -> str:
-        """Return SSM instance's string representation."""
-        return (f'SSM[slm: {self.slm} | adapter: {self.get_adapter()} | '
-                f'backends: {self.get_backends()}]')
-
     def get_slm(self) -> AbstractSLM:
         """
         Return the previous assigned SLM,
         or a default SLM if none was assigned.
         """
         if self.slm is None:
             self.slm = BaseSLM()
```

### Comparing `openssm_dev-0.1.6.6/openssm/core/ssm/gpt3_llama_index_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/openai_ssm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-"""SSM with GPT3-based SLM and LlamaIndex-based adapter."""
-
-
 from openssm.core.ssm.base_ssm import BaseSSM
+from openssm.core.slm.openai_slm import GPT3CompletionSLM
 from openssm.core.slm.openai_slm import GPT3ChatCompletionSLM
-from openssm.core.adapter.llama_index_adapter import LlamaIndexAdapter
+from openssm.core.adapter.abstract_adapter import AbstractAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
-class GPT3LlamaIndexSSM(BaseSSM):
-    """SSM with GPT3-based SLM and LlamaIndex-based adapter."""
-
-    def __init__(self, backends: list[AbstractBackend]):
-        adapter = LlamaIndexAdapter(backends)
-
-        slm = GPT3ChatCompletionSLM(adapter=adapter)
-        slm.pass_to_adapter: bool = True
+class GPT3CompletionSSM(BaseSSM):
+    def __init__(self,
+                 adapter: AbstractAdapter = None,
+                 backends: list[AbstractBackend] = None):
+        super().__init__(GPT3CompletionSLM(), adapter, backends)
 
-        super().__init__(slm, adapter, backends)
 
-    def __repr__(self) -> str:
-        """Return SSM instance's string representation."""
-        return f'LlamaIndexSSM[backends: {self.get_backends()}]'
+class GPT3ChatCompletionSSM(BaseSSM):
+    def __init__(self,
+                 adapter: AbstractAdapter = None,
+                 backends: list[AbstractBackend] = None):
+        super().__init__(GPT3ChatCompletionSLM(), adapter, backends)
```

### Comparing `openssm_dev-0.1.6.6/openssm/integration/llamaindex/README.md` & `openssm_dev-0.1.6.dev0/openssm/integration/llamaindex/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.6.6/PKG-INFO` & `openssm_dev-0.1.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openssm-dev
-Version: 0.1.6.6
+Version: 0.1.6.dev0
 Summary: OpenSSM - 'Small Specialist Models' for Industrial AI
 Author: Aitomatic Engineering
 Author-email: engineering@aitomatic.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: accelerate (>=0.20.3)
+Requires-Dist: accelerate (>=0.21.0)
 Requires-Dist: einops (>=0.6.1)
-Requires-Dist: llama-hub (>=0.0.4)
-Requires-Dist: llama-index (>=0.6.33)
-Requires-Dist: pypdf (>=3.11.0)
-Requires-Dist: pytest (>=7.0.0)
+Requires-Dist: llama-hub (>=0.0.12)
+Requires-Dist: llama-index (>=0.7.10)
+Requires-Dist: pypdf (>=3.12.2)
+Requires-Dist: pytest (>=7.4.0)
 Requires-Dist: torch (>=1.13.1)
-Requires-Dist: transformers (>=4.30.2)
+Requires-Dist: transformers (>=4.31.0)
 Description-Content-Type: text/markdown
 
 # OpenSSM – “Small Specialist Models” for Industrial AI
 
 > &nbsp;
 > See full documentation at [aitomatic.github.io/openssm/](https://aitomatic.github.io/openssm/).
 > &nbsp;
```

