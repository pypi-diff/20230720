# Comparing `tmp/pandasai-0.6.9.tar.gz` & `tmp/pandasai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.9.tar", max compression
+gzip compressed data, was "pandasai-0.7.0.tar", max compression
```

## Comparing `pandasai-0.6.9.tar` & `pandasai-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1055 2023-07-12 00:57:07.624913 pandasai-0.6.9/LICENSE
--rw-r--r--   0        0        0     7705 2023-07-12 00:57:07.624913 pandasai-0.6.9/README.md
--rw-r--r--   0        0        0    25302 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3116 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3507 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4335 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11442 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3176 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1270 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1076 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1081 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1072 2023-07-12 00:57:07.628915 pandasai-0.6.9/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-07-12 00:57:07.632917 pandasai-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-20 13:09:33.567383 pandasai-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7705 2023-07-20 13:09:33.567383 pandasai-0.7.0/README.md
+-rw-r--r--   0        0        0    26182 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0     1438 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-20 13:09:33.571383 pandasai-0.7.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3507 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    12056 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1686 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1513 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1342 2023-07-20 13:09:33.575383 pandasai-0.7.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1900 2023-07-20 13:09:33.575383 pandasai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.0/PKG-INFO
```

### Comparing `pandasai-0.6.9/LICENSE` & `pandasai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/README.md` & `pandasai-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/__init__.py` & `pandasai-0.7.0/pandasai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 """
 
 import ast
 import io
 import logging
 import re
 import sys
+import traceback
 import uuid
 import time
 from contextlib import redirect_stdout
 from typing import List, Optional, Union, Dict, Type
 import importlib.metadata
 
 __version__ = importlib.metadata.version(__package__ or __name__)
@@ -65,14 +66,15 @@
 from .middlewares.charts import ChartsMiddleware
 from .prompts.base import Prompt
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
+from .callbacks.base import BaseCallback, DefaultCallback
 
 
 def get_version():
     """
     Get the version from the package metadata
     """
     from importlib.metadata import version
@@ -151,15 +153,15 @@
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
     _start_time: float = 0
     _enable_logging: bool = True
     _logger: logging.Logger = None
-    _logs: List[str] = []
+    _logs: List[dict[str, str]] = []
     last_code_generated: Optional[str] = None
     last_code_executed: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
@@ -170,14 +172,15 @@
         save_charts=False,
         save_charts_path=None,
         enable_cache=True,
         middlewares=None,
         custom_whitelisted_dependencies=None,
         enable_logging=True,
         non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
+        callback: BaseCallback = DefaultCallback,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -243,14 +246,16 @@
 
         if middlewares is not None:
             self.add_middlewares(*middlewares)
 
         if custom_whitelisted_dependencies is not None:
             self._custom_whitelisted_dependencies = custom_whitelisted_dependencies
 
+        self.callback = callback
+
     def _load_llm(self, llm):
         """
         Check if it is a PandasAI LLM or a Langchain LLM.
         If it is a Langchain LLM, wrap it in a PandasAI LLM.
 
         Args:
             llm (object): LLMs option to be used for API access
@@ -344,15 +349,15 @@
                     multiple_dataframes_instruction = self._non_default_prompts.get(
                         "multiple_dataframes", MultipleDataframesPrompt
                     )
                     code = self._llm.generate_code(
                         multiple_dataframes_instruction(dataframes=heads),
                         prompt,
                     )
-
+                    self.callback.on_code(code)
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
@@ -368,15 +373,15 @@
                         num_rows=data_frame.shape[0],
                         num_columns=data_frame.shape[1],
                     )
                     code = self._llm.generate_code(
                         generate_code_instruction,
                         prompt,
                     )
-
+                    self.callback.on_code(code)
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": df_head,
                         "num_rows": data_frame.shape[0],
                         "num_columns": data_frame.shape[1],
                     }
 
@@ -607,16 +612,17 @@
                 code=code,
                 error_returned=e,
                 question=self._original_instructions["question"],
                 df_head=self._original_instructions["df_head"],
                 num_rows=self._original_instructions["num_rows"],
                 num_columns=self._original_instructions["num_columns"],
             )
-
-        return self._llm.generate_code(error_correcting_instruction, "")
+        code = self._llm.generate_code(error_correcting_instruction, "")
+        self.callback.on_code(code)
+        return code
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
@@ -669,14 +675,19 @@
             while count < self._max_retries:
                 try:
                     # Execute the code
                     exec(code_to_run, environment)
                     code = code_to_run
                     break
                 except Exception as e:
+                    self.log(
+                        f"Error executing code (count: {count})", level=logging.WARNING
+                    )
+                    self.log(f"{traceback.format_exc()}", level=logging.DEBUG)
+
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
 
                     code_to_run = self._retry_run_code(code, e, multiple)
 
@@ -704,21 +715,28 @@
             if isinstance(result, tuple):
                 result = " ".join([str(element) for element in result])
 
             return result
         except Exception:
             return captured_output
 
-    def log(self, message: str):
-        """Log a message"""
-        self._logger.info(message)
-        self._logs.append(message)
+    def log(self, message: str, level: Optional[int] = logging.INFO):
+        """
+        Log the passed message with according log level.
+
+        Args:
+            message (str): a message string to be logged
+            level (Optional[int]): an integer, representing log level;
+                                   default to 20 (INFO)
+        """
+        self._logger.log(level=level, msg=message)
+        self._logs.append({"msg": message, "level": level})
 
     @property
-    def logs(self) -> List[str]:
+    def logs(self) -> List[dict[str, str]]:
         """Return the logs"""
         return self._logs
 
     def process_id(self) -> str:
         """Return the id of this PandasAI object."""
         return self._process_id
```

### Comparing `pandasai-0.6.9/pandasai/constants.py` & `pandasai-0.7.0/pandasai/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Constants used in the pandasai package.
+It includes Start & End Code tags, Whitelisted Python Packages and
+While List Builtin Methods.
+"""
+
+START_CODE_TAG = "<startCode>"
+END_CODE_TAG = "<endCode>"
+
 # List of Python builtin libraries that are added to the environment by default.
 WHITELISTED_BUILTINS = [
     "abs",
     "all",
     "any",
     "ascii",
     "bin",
```

### Comparing `pandasai-0.6.9/pandasai/exceptions.py` & `pandasai-0.7.0/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/_optional.py` & `pandasai-0.7.0/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/anonymizer.py` & `pandasai-0.7.0/pandasai/helpers/anonymizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 import random
 import re
 import string
 
 import pandas as pd
+import numpy as np
 
 
 def is_valid_email(email: str) -> bool:
     """Check if the given email is valid based on regex pattern.
 
     Args:
         email (str): email address to be checked.
@@ -138,22 +139,24 @@
         data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
         force_conversion (bool): Convert it with instruction. Default is True.
 
     Returns: Anonymized head of the DataFrame.
     """
 
     data_frame = copy_head(data_frame)
-    dtypes = data_frame.dtypes
     for col in data_frame.columns:
         col_idx = data_frame.columns.get_loc(col)
         # check category type column and temporarily convert to object type
         if force_conversion:
             if pd.api.types.is_categorical_dtype(data_frame[col]):
                 if data_frame[col].isna().any():
                     data_frame[col] = data_frame[col].astype(object)
+            else:
+                # converting all non-categorical columns to strings
+                data_frame[col] = data_frame[col].astype(str)
         for row_idx, val in enumerate(data_frame[col]):
             cell_value = str(val)
 
             if is_valid_email(cell_value):
                 data_frame.iloc[row_idx, col_idx] = generate_random_email()
                 continue
             if is_valid_phone_number(cell_value):
@@ -161,19 +164,38 @@
                     cell_value
                 )
                 continue
             if is_valid_credit_card(cell_value):
                 data_frame.iloc[row_idx, col_idx] = generate_random_credit_card()
                 continue
 
+            # "<NA>" is null value originaly which got converted to string
+            if cell_value == "<NA>":
+                # Reinitialising cell_value to NULL
+                cell_value = np.nan
             # anonymize data
-            random_row_index = random.choice(
-                [i for i in range(len(data_frame.index)) if i != row_idx]
-            )
-            random_value = data_frame.iloc[random_row_index, col_idx]
-            data_frame.iloc[row_idx, col_idx] = random_value
-            data_frame.iloc[random_row_index, col_idx] = (
-                pd.eval(cell_value) if cell_value in ["True", "False"] else cell_value
-            )
+            if len(data_frame.index) > 1:  # edge case , when only single row is present
+                random_row_index = random.choice(
+                    [i for i in range(len(data_frame.index)) if i != row_idx]
+                )
+                random_value = data_frame.iloc[random_row_index, col_idx]
+                data_frame.iloc[row_idx, col_idx] = random_value
+                data_frame.iloc[random_row_index, col_idx] = (
+                    pd.eval(cell_value)
+                    if cell_value in ["True", "False"]
+                    else cell_value
+                )
     # restore the original data types
-    data_frame = data_frame.astype(dtypes)
+    # Handling Int64 dtype explicitly
+    for i in range(len(data_frame.columns)):
+        dt = data_frame.dtypes[i]
+        col = data_frame.columns[i]
+        if dt == "Int64":
+            data_frame[col] = data_frame[col].astype(
+                "float64"
+            )  # float64 can handle Null values (np.nan)
+            data_frame[col] = data_frame[col].astype(
+                "Int64"
+            )  # Converting back to original Int64
+        else:
+            data_frame[col] = data_frame[col].astype(dt)
     return data_frame
```

### Comparing `pandasai-0.6.9/pandasai/helpers/cache.py` & `pandasai-0.7.0/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/from_excel.py` & `pandasai-0.7.0/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/notebook.py` & `pandasai-0.7.0/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/openai_info.py` & `pandasai-0.7.0/pandasai/helpers/openai_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     "text-davinci-003": 0.02,
     "text-davinci-002": 0.02,
     "code-davinci-002": 0.02,
 }
 
 
 def get_openai_token_cost_for_model(
-        model_name: str, num_tokens: int,
+    model_name: str,
+    num_tokens: int,
 ) -> float:
     """
     Get the cost in USD for a given model and number of tokens.
     Args:
         model_name: Name of the model
         num_tokens: Number of tokens.
     Returns:
@@ -62,18 +63,15 @@
     def __call__(self, response: OpenAIObject) -> None:
         """Collect token usage"""
         usage = response.usage
         if "total_tokens" not in usage:
             return None
         model_name = response.model
         if model_name in MODEL_COST_PER_1K_TOKENS:
-            total_cost = get_openai_token_cost_for_model(
-                model_name,
-                usage.total_tokens
-            )
+            total_cost = get_openai_token_cost_for_model(model_name, usage.total_tokens)
             self.total_cost += total_cost
 
         self.total_tokens += usage.total_tokens
         self.prompt_tokens += usage.prompt_tokens
         self.completion_tokens += usage.completion_tokens
 
     def __copy__(self) -> "OpenAICallbackHandler":
```

### Comparing `pandasai-0.6.9/pandasai/helpers/save_chart.py` & `pandasai-0.7.0/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/helpers/shortcuts.py` & `pandasai-0.7.0/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/llm/azure_openai.py` & `pandasai-0.7.0/pandasai/llm/azure_openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,15 @@
             raise UnsupportedOpenAIModelError("Model deployment name is required.")
 
         self.is_chat_model = is_chat_model
         self.engine = deployment_name
 
         self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
         if self.openai_proxy:
-            openai.proxy = {
-                "http": self.openai_proxy,
-                "https": self.openai_proxy
-            }
+            openai.proxy = {"http": self.openai_proxy, "https": self.openai_proxy}
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API
```

### Comparing `pandasai-0.6.9/pandasai/llm/base.py` & `pandasai-0.7.0/pandasai/llm/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
 import openai
 import requests
 
+from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 from ..helpers._optional import import_dependency
 from ..helpers.openai_info import openai_callback_var
@@ -103,14 +104,21 @@
         Raises:
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
         """
         code = response
+        match = re.search(
+            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
+            code,
+            re.DOTALL,
+        )
+        if match:
+            code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
@@ -309,14 +317,25 @@
             response = self.query({"inputs": payload})
             payload = response
             if response.count("<endCode>") >= 2:
                 break
 
         # replace instruction + value from the inputs to avoid showing it in the output
         output = response.replace(prompt + value + suffix, "")
+        ans = ""
+        for line in output.split("\n"):
+            if line.find("utput:") != -1:
+                break
+            if ans == "":
+                ans = ans + line
+            else:
+                ans = ans + "\n" + line
+        if len(ans.split("'''")) > 0:
+            ans = ans.split("'''")[0]
+        output = ans
         return output
 
 
 class BaseGoogle(LLM):
     """Base class to implement a new Google LLM
 
     LLM base class is extended to be used with Google Palm API.
```

### Comparing `pandasai-0.6.9/pandasai/llm/fake.py` & `pandasai-0.7.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/llm/falcon.py` & `pandasai-0.7.0/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/llm/google_palm.py` & `pandasai-0.7.0/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/llm/langchain.py` & `pandasai-0.7.0/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/llm/openai.py` & `pandasai-0.7.0/pandasai/llm/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,18 +63,15 @@
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
         self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
         if self.openai_proxy:
-            openai.proxy = {
-                "http": self.openai_proxy,
-                "https": self.openai_proxy
-            }
+            openai.proxy = {"http": self.openai_proxy, "https": self.openai_proxy}
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
```

### Comparing `pandasai-0.6.9/pandasai/llm/starcoder.py` & `pandasai-0.7.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/middlewares/base.py` & `pandasai-0.7.0/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/middlewares/charts.py` & `pandasai-0.7.0/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/middlewares/streamlit.py` & `pandasai-0.7.0/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/prompts/base.py` & `pandasai-0.7.0/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.9/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.7.0/pandasai/prompts/correct_error_prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above
-mentioned error. Do not generate the same code again.
+mentioned error. Do not generate the same code again. Make sure to prefix the requested python
+code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 ```
 """  # noqa: E501
 from datetime import date
 
+from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class CorrectErrorPrompt(Prompt):
     """Prompt to Correct Python code on Error"""
 
     text: str = """
@@ -38,11 +40,17 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
+Make sure to prefix the requested python code with <startCode> exactly and suffix the code with <endCode> exactly.
 """  # noqa: E501
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs, today_date=date.today())
+        super().__init__(
+            **kwargs,
+            START_CODE_TAG=START_CODE_TAG,
+            END_CODE_TAG=END_CODE_TAG,
+            today_date=date.today()
+        )
```

### Comparing `pandasai-0.6.9/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.7.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Prompt to correct error """
 
 import pandas as pd
 
+from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class CorrectMultipleDataframesErrorPrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
@@ -32,13 +33,14 @@
 You generated this python code:
 {code}
 
 It fails with the following error:
 {error_returned}
 
 Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
+Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
 """  # noqa: E501
 
         self.text += instruction
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.6.9/pandasai/prompts/generate_python_code.py` & `pandasai-0.7.0/pandasai/prompts/generate_python_code.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,39 @@
 ```
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the
-dataframe `df`. Using the provided dataframe, df, return the python code to get the answer to the following question:
+dataframe `df`. Using the provided dataframe, df, return the python code and make sure to prefix
+the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG}
+exactly to get the answer to the following question:
 ```
 """  # noqa: E501
 
 from datetime import date
 
+from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class GeneratePythonCodePrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
 Today is {today_date}.
 You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the metadata of the dataframe:
 {df_head}.
 
 When asked about the data, your response should include a python code that describes the dataframe `df`.
-Using the provided dataframe, df, return the python code to get the answer to the following question:
+Using the provided dataframe, df, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs, today_date=date.today())
+        super().__init__(
+            **kwargs,
+            START_CODE_TAG=START_CODE_TAG,
+            END_CODE_TAG=END_CODE_TAG,
+            today_date=date.today()
+        )
```

### Comparing `pandasai-0.6.9/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.7.0/pandasai/prompts/multiple_dataframes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """ Prompt to generate Python code for multiple dataframes """
 
 from datetime import date
 
 import pandas as pd
 
+from pandasai.constants import END_CODE_TAG, START_CODE_TAG
 from .base import Prompt
 
 
 class MultipleDataframesPrompt(Prompt):
     """Prompt to generate Python code"""
 
     text: str = """
 Today is {today_date}.
 You are provided with the following pandas dataframes:"""
     instruction: str = """
 When asked about the data, your response should include a python code that describes the dataframes provided.
-Using the provided dataframes and no other dataframes, return the python code to get the answer to the following question:
+Using the provided dataframes and no other dataframes, return the python code and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """  # noqa: E501
 
     def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             self.text += f"""
 Dataframe df{i}, with {row} rows and {col} columns.
 This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             today_date=date.today(),
+            START_CODE_TAG=START_CODE_TAG,
+            END_CODE_TAG=END_CODE_TAG,
         )
 
     def __str__(self):
         return self.text
```

### Comparing `pandasai-0.6.9/pyproject.toml` & `pandasai-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.9"
+version = "0.7.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.9/PKG-INFO` & `pandasai-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.9
+Version: 0.7.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

