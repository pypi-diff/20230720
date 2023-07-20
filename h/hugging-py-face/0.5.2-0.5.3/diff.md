# Comparing `tmp/hugging_py_face-0.5.2.tar.gz` & `tmp/hugging_py_face-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.5.2.tar", last modified: Thu Jul 20 17:30:19 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.5.3.tar", last modified: Thu Jul 20 18:07:49 2023, max compression
```

## Comparing `hugging_py_face-0.5.2.tar` & `hugging_py_face-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/
--rw-rw-rw-   0        0        0     6177 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face/
--rw-rw-rw-   0        0        0      466 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      676 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3927 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0     1058 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/base_api.py
--rw-rw-rw-   0        0        0     2852 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face/config/
--rw-rw-rw-   0        0        0      875 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/config/config.yaml
--rw-rw-rw-   0        0        0      265 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/config/logging.yaml
--rw-rw-rw-   0        0        0      320 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0      171 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/exceptions.py
--rw-rw-rw-   0        0        0     2483 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    27325 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 17:30:19.000000 hugging_py_face-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-20 17:30:02.000000 hugging_py_face-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/
+-rw-rw-rw-   0        0        0     6177 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      676 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3927 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0     1058 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/base_api.py
+-rw-rw-rw-   0        0        0     2852 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      875 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      265 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/config/logging.yaml
+-rw-rw-rw-   0        0        0      320 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0      236 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/exceptions.py
+-rw-rw-rw-   0        0        0     2483 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    27972 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-07-20 18:07:48.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-20 18:07:48.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:07:48.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-20 18:07:48.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-20 18:07:48.000000 hugging_py_face-0.5.3/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:07:49.000000 hugging_py_face-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-20 18:07:21.000000 hugging_py_face-0.5.3/setup.py
```

### Comparing `hugging_py_face-0.5.2/PKG-INFO` & `hugging_py_face-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging_py_face
-Version: 0.5.2
+Version: 0.5.3
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.5.2/README.md` & `hugging_py_face-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/__init__.py` & `hugging_py_face-0.5.3/hugging_py_face/__init__.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/audio_processing.py` & `hugging_py_face-0.5.3/hugging_py_face/audio_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/base_api.py` & `hugging_py_face-0.5.3/hugging_py_face/base_api.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/computer_vision.py` & `hugging_py_face-0.5.3/hugging_py_face/computer_vision.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/config/config.yaml` & `hugging_py_face-0.5.3/hugging_py_face/config/config.yaml`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/multimedia_processing.py` & `hugging_py_face-0.5.3/hugging_py_face/multimedia_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/hugging_py_face/nlp.py` & `hugging_py_face-0.5.3/hugging_py_face/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import requests
 import pandas as pd
 from pandas import DataFrame
 from typing import Text, List, Dict, Optional, Union
 
 from .base_api import BaseAPI
-from .exceptions import HTTPServiceUnavailableException, APICallException
+from .exceptions import HTTPServiceUnavailableException, APICallException, InsufficientParametersException
 
 
 class NLP(BaseAPI):
     def __init__(self, api_token: Text, api_url: Optional[Text] = None):
         super().__init__(api_token, api_url)
 
     def _query(self, inputs: Union[Text, List, Dict], parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
@@ -365,44 +365,48 @@
         :param text: a string or a list of strings to get the features from.
         :param options: a dict of options. For more information, see the `detailed parameters for the feature extraction task <https://huggingface.co/docs/api-inference/detailed_parameters#feature-extraction-task>`_.
         :param model: the model to use for the feature extraction task. If not provided, the recommended model from Hugging Face will be used.
         :return: a list of dicts or a list of lists (of dicts) containing the representation of the features of the input(s).
         """
         return self._query(text, options=options, model=model, task='feature-extraction')
 
-    def translation(self, text: Union[Text, List], lang_input: Text, lang_output: Text, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
+    def translation(self, text: Union[Text, List], lang_input: Text = None, lang_output: Text = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Translates text from one language to another.
 
         :param text: a string or a list of strings to translate.
-        :param lang_input: the short code of the language of the input text.
-        :param lang_output: the short code of the language to translate the input text to.
+        :param lang_input: the short code of the language of the input text. This parameter is mandatory if the model is not provided.
+        :param lang_output: the short code of the language to translate the input text to. This parameter is mandatory if the model is not provided.
         :param options: a dict of options. For more information, see the `detailed parameters for the translation task <https://huggingface.co/docs/api-inference/detailed_parameters#translation-task>`_.
         :param model: the model to use for the translation task. If not provided, the recommended model from Hugging Face will be used.
         :return: a dict or a list of dicts containing the translated text.
         """
         if model is None:
+            if lang_input is None or lang_output is None:
+                InsufficientParametersException("lang_input and lang_output are required if model is not provided.")
             model = f"{self.config['TASK_MODEL_MAP']['translation']}{lang_input}-{lang_output}"
             return self._query(text, options=options, model=model, task='translation')
         else:
             return self._query(text, options=options, model=model, task='translation')
 
-    def translation_in_df(self, df: DataFrame, column: Text, lang_input: Text, lang_output: Text, options: Optional[Dict] = None, model: Optional[Text] = None) -> DataFrame:
+    def translation_in_df(self, df: DataFrame, column: Text, lang_input: Text = None, lang_output: Text = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> DataFrame:
         """
         Translates text from one language to another.
 
         :param df: a pandas DataFrame containing the strings to be translated.
         :param column: the column containing the strings to be translated.
-        :param lang_input: the short code of the language of the input text.
-        :param lang_output: the short code of the language to translate the input text to.
+        :param lang_input: the short code of the language of the input text. This parameter is mandatory if the model is not provided.
+        :param lang_output: the short code of the language to translate the input text to. This parameter is mandatory if the model is not provided.
         :param options: a dict of options. For more information, see the `detailed parameters for the translation task <https://huggingface.co/docs/api-inference/detailed_parameters#translation-task>`_.
         :param model: the model to use for the translation task. If not provided, the recommended model from Hugging Face will be used.
         :return: a pandas DataFrame with the translations. The translations will be added as a new column called 'predictions' to the original DataFrame.
         """
         if model is None:
+            if lang_input is None or lang_output is None:
+                InsufficientParametersException("lang_input and lang_output are required if model is not provided.")
             model = f"{self.config['TASK_MODEL_MAP']['translation']}{lang_input}-{lang_output}"
             predictions = self._query_in_df(df, column, options=options, model=model, task='translation')
         else:
             predictions = self._query_in_df(df, column, options=options, model=model, task='translation')
 
         df['predictions'] = [prediction['translation_text'] for prediction in predictions]
         return df
```

### Comparing `hugging_py_face-0.5.2/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.5.3/hugging_py_face.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging-py-face
-Version: 0.5.2
+Version: 0.5.3
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.5.2/hugging_py_face.egg-info/SOURCES.txt` & `hugging_py_face-0.5.3/hugging_py_face.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.5.2/setup.py` & `hugging_py_face-0.5.3/setup.py`

 * *Files identical despite different names*

