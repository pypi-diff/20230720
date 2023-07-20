# Comparing `tmp/scale_llm_engine-0.0.0b3.tar.gz` & `tmp/scale_llm_engine-0.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b3.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b4.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b3.tar` & `scale_llm_engine-0.0.0b4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1001 2023-07-17 21:09:48.759908 scale_llm_engine-0.0.0b3/README.md
--rw-r--r--   0        0        0     1576 2023-07-18 04:36:10.686982 scale_llm_engine-0.0.0b3/llmengine/__init__.py
--rw-r--r--   0        0        0     6190 2023-07-18 04:31:34.842871 scale_llm_engine-0.0.0b3/llmengine/api_engine.py
--rw-r--r--   0        0        0    12958 2023-07-18 04:31:39.203554 scale_llm_engine-0.0.0b3/llmengine/completion.py
--rw-r--r--   0        0        0    11851 2023-07-18 04:31:39.203919 scale_llm_engine-0.0.0b3/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-16 18:41:46.698514 scale_llm_engine-0.0.0b3/llmengine/errors.py
--rw-r--r--   0        0        0    11100 2023-07-18 04:31:39.204232 scale_llm_engine-0.0.0b3/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     7052 2023-07-18 03:09:52.904995 scale_llm_engine-0.0.0b3/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-18 04:32:04.597570 scale_llm_engine-0.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/README.md
+-rw-r--r--   0        0        0     1576 2023-07-20 17:29:36.022438 scale_llm_engine-0.0.0b4/llmengine/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/api_engine.py
+-rw-r--r--   0        0        0    13065 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/completion.py
+-rw-r--r--   0        0        0    13090 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/errors.py
+-rw-r--r--   0        0        0    13905 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    13738 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b4/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-20 17:29:35.126426 scale_llm_engine-0.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b4/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b3/README.md` & `scale_llm_engine-0.0.0b4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ```shell
 pip install scale-llm-engine
 ```
 
 ### Usage
 
 If you are using LLM Engine, you can get your API key from
-[https://spellbook.scale.com/settings](https://spellbook.scale.com/settings). 
+[https://spellbook.scale.com/settings](https://spellbook.scale.com/settings).
 Set the `SCALE_API_KEY` environment variable to your API key.
 
 If you are using your own infrastructure, you can set the
 `LLM_ENGINE_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `llmengine` endpoint.
 
 ```python
 from llmengine import Completion
 
 response = Completion.create(
-    model="llama-7b",
+    model="llama-2-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
```

### Comparing `scale_llm_engine-0.0.0b3/llmengine/__init__.py` & `scale_llm_engine-0.0.0b4/llmengine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta3"
+__version__ = "0.0.0.beta4"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
```

### Comparing `scale_llm_engine-0.0.0b3/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b4/llmengine/api_engine.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b3/llmengine/completion.py` & `scale_llm_engine-0.0.0b4/llmengine/completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     ) -> Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters asynchronously (with `asyncio`).
 
         This API can be used to get the LLM to generate a completion *asynchronously*.
         It takes as parameters the `model` ([see Model Zoo](../../model_zoo)) and the `prompt`.
         Optionally it takes `max_new_tokens`, `temperature`, `timeout` and `stream`.
-        It returns
-        [CompletionSyncV1Response](../../api/data_types/#llmengine.CompletionSyncV1Response)
+        It returns a
+        [CompletionSyncResponse](../../api/data_types/#llmengine.CompletionSyncResponse)
         if `stream=False` or an async iterator of
-        [CompletionStreamV1Response](../../api/data_types/#llmengine.CompletionStreamV1Response)
+        [CompletionStreamResponse](../../api/data_types/#llmengine.CompletionStreamResponse)
         with `request_id` and `outputs` fields.
 
         Args:
             model (str):
                 Name of the model to use. See [Model Zoo](../../model_zoo) for a list of Models that are supported.
             prompt (str):
                 The prompt to generate completions for, encoded as a string.
@@ -67,77 +67,72 @@
                 Whether to stream the response. If true, the return type is an
                 `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
                 When streaming, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format).
 
         Returns:
             response (Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]): The generated response (if `stream=False`) or iterator of response chunks (if `stream=True`)
 
-        Token streaming can be used to reduce _percieved_ latency for applications:
-
-        === "Asynchronous completion without token streaming in python"
+        === "Asynchronous completion without token streaming in Python"
             ```python
             import asyncio
             from llmengine import Completion
 
             async def main():
                 response = await Completion.acreate(
-                    model="llama-7b",
+                    model="llama-2-7b",
                     prompt="Hello, my name is",
                     max_new_tokens=10,
                     temperature=0.2,
                 )
                 print(response.json())
 
             asyncio.run(main())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
-                "request_id": "b1b2c3d4e5f6g7h8i9j0",
-                "outputs":
-                [
-                    {
-                        "text": "_______, and I am a _____",
-                        "num_completion_tokens": 10
-                    }
-                ],
+                "request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0",
+                "output": {
+                    "text": "_______ and I am a _______",
+                    "num_completion_tokens": 10
+                }
             }
             ```
 
-        Here is how applications can use streaming:
+        Token streaming can be used to reduce _perceived_ latency for applications. Here is how applications can use streaming:
 
-        === "Asynchronous completion with token streaming in python"
+        === "Asynchronous completion with token streaming in Python"
             ```python
             import asyncio
             from llmengine import Completion
 
             async def main():
                 stream = await Completion.acreate(
-                    model="llama-7b",
+                    model="llama-2-7b",
                     prompt="why is the sky blue?",
                     max_new_tokens=5,
                     temperature=0.2,
                     stream=True,
                 )
 
                 async for response in stream:
                     if response.output:
                         print(response.json())
 
             asyncio.run(main())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
-            {"request_id": "0123456789", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1}}
-            {"request_id": "0123456789", "output": {"text": "I", "finished": false, "num_completion_tokens": 2}}
-            {"request_id": "0123456789", "output": {"text": " think", "finished": false, "num_completion_tokens": 3}}
-            {"request_id": "0123456789", "output": {"text": " the", "finished": false, "num_completion_tokens": 4}}
-            {"request_id": "0123456789", "output": {"text": " sky", "finished": true, "num_completion_tokens": 5}}
+            {"request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1}}
+            {"request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0", "output": {"text": "I", "finished": false, "num_completion_tokens": 2}}
+            {"request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0", "output": {"text": " think", "finished": false, "num_completion_tokens": 3}}
+            {"request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0", "output": {"text": " the", "finished": false, "num_completion_tokens": 4}}
+            {"request_id": "9cfe4d5a-f86f-4094-a935-87f871d90ec0", "output": {"text": " sky", "finished": true, "num_completion_tokens": 5}}
             ```
         """
         if stream:
 
             async def _acreate_stream(
                 **kwargs,
             ) -> AsyncIterable[CompletionStreamResponse]:
@@ -185,18 +180,18 @@
     ) -> Union[CompletionSyncResponse, Iterator[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters synchronously.
 
         This API can be used to get the LLM to generate a completion *synchronously*.
         It takes as parameters the `model` ([see Model Zoo](../../model_zoo)) and the `prompt`.
         Optionally it takes `max_new_tokens`, `temperature`, `timeout` and `stream`.
-        It returns
-        [CompletionSyncV1Response](../../api/data_types/#llmengine.CompletionSyncV1Response)
+        It returns a
+        [CompletionSyncResponse](../../api/data_types/#llmengine.CompletionSyncResponse)
         if `stream=False` or an async iterator of
-        [CompletionStreamV1Response](../../api/data_types/#llmengine.CompletionStreamV1Response)
+        [CompletionStreamResponse](../../api/data_types/#llmengine.CompletionStreamResponse)
         with `request_id` and `outputs` fields.
 
         Args:
             model (str):
                 Name of the model to use. See [Model Zoo](../../model_zoo) for a list of Models that are supported.
 
             prompt (str):
@@ -220,70 +215,64 @@
                 `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
                 When streaming, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format).
 
 
         Returns:
             response (Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]): The generated response (if `stream=False`) or iterator of response chunks (if `stream=True`)
 
-        Token streaming can be used to reduce _percieved_ latency for applications:
-
-        === "Synchronous completion without token streaming in python"
+        === "Synchronous completion without token streaming in Python"
             ```python
             from llmengine import Completion
 
             response = Completion.create(
-                model="llama-7b",
+                model="llama-2-7b",
                 prompt="Hello, my name is",
                 max_new_tokens=10,
                 temperature=0.2,
             )
             print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
-                "request_id": "0123456789",
-                "outputs":
-                [
-                    {
-                        "text": "_______ and I am a _______",
-                        "num_completion_tokens": 10
-                    }
-                ],
-                "traceback": null
+                "request_id": "8bbd0e83-f94c-465b-a12b-aabad45750a9",
+                "output": {
+                    "text": "_______ and I am a _______",
+                    "num_completion_tokens": 10
+                }
             }
             ```
 
-        Here is how applications can use streaming:
+        Token streaming can be used to reduce _perceived_ latency for applications. Here is how applications can use streaming:
 
-        === "Synchronous completion with token streaming in python"
+        === "Synchronous completion with token streaming in Python"
             ```python
             from llmengine import Completion
 
             stream = Completion.create(
-                model="llama-7b",
+                model="llama-2-7b",
                 prompt="why is the sky blue?",
                 max_new_tokens=5,
                 temperature=0.2,
                 stream=True,
             )
 
             for response in stream:
                 if response.output:
                     print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
-            {"request_id": "0123456789", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1 } }
-            {"request_id": "0123456789", "output": {"text": "I", "finished": false, "num_completion_tokens": 2 } }
-            {"request_id": "0123456789", "output": {"text": " don", "finished": false, "num_completion_tokens": 3 } }
-            {"request_id": "0123456789", "output": {"text": "’", "finished": false, "num_completion_tokens": 4 } }
-            {"request_id": "0123456789", "output": {"text": "t", "finished": true, "num_completion_tokens": 5 } }
+            {"request_id": "ebbde00c-8c31-4c03-8306-24f37cd25fa2", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1 } }
+            {"request_id": "ebbde00c-8c31-4c03-8306-24f37cd25fa2", "output": {"text": "I", "finished": false, "num_completion_tokens": 2 } }
+            {"request_id": "ebbde00c-8c31-4c03-8306-24f37cd25fa2", "output": {"text": " don", "finished": false, "num_completion_tokens": 3 } }
+            {"request_id": "ebbde00c-8c31-4c03-8306-24f37cd25fa2", "output": {"text": "’", "finished": false, "num_completion_tokens": 4 } }
+            {"request_id": "ebbde00c-8c31-4c03-8306-24f37cd25fa2", "output": {"text": "t", "finished": true, "num_completion_tokens": 5 } }
             ```
         """
         if stream:
 
             def _create_stream(**kwargs):
                 data_stream = CompletionStreamV1Request(**kwargs).dict()
                 response_stream = cls.post_stream(
```

### Comparing `scale_llm_engine-0.0.0b3/llmengine/data_types.py` & `scale_llm_engine-0.0.0b4/llmengine/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,26 @@
     last_updated_at: datetime.datetime
     deployment_state: Optional[ModelEndpointDeploymentState] = Field(default=None)
     resource_state: Optional[ModelEndpointResourceState] = Field(default=None)
     num_queued_items: Optional[int] = Field(default=None)
     public_inference: Optional[bool] = Field(default=None)
 
 
+class PostInferenceHooks(str, Enum):
+    """
+    Post-inference hooks are functions that are called after inference is complete.
+
+    Attributes:
+        CALLBACK: The callback hook is called with the inference response and the task ID.
+    """
+
+    # INSIGHT = "insight"
+    CALLBACK: str = "callback"
+
+
 class CreateLLMEndpointRequest(BaseModel):
     name: str
 
     # LLM specific fields
     model_name: str
     source: LLMSource = LLMSource.HUGGING_FACE
     inference_framework: LLMInferenceFramework = LLMInferenceFramework.DEEPSPEED
@@ -156,42 +168,50 @@
     Response object for retrieving a Model.
     """
 
     id: Optional[str] = Field(
         default=None, description="(For self-hosted users) The autogenerated ID of the model."
     )
     """(For self-hosted users) The autogenerated ID of the model."""
+
     name: str = Field(
         description="The name of the model. Use this for making inference requests to the model."
     )
     """The name of the model. Use this for making inference requests to the model."""
+
     model_name: Optional[str] = Field(
         default=None,
         description="(For self-hosted users) For fine-tuned models, the base model. For base models, this will be the same as `name`.",
     )
     """(For self-hosted users) For fine-tuned models, the base model. For base models, this will be the same as `name`."""
+
     source: LLMSource = Field(description="The source of the model, e.g. Hugging Face.")
     """The source of the model, e.g. Hugging Face."""
+
     inference_framework: LLMInferenceFramework = Field(
         description="The inference framework used by the model."
     )
-    """The inference framework used by the model."""
+    """(For self-hosted users) The inference framework used by the model."""
+
     inference_framework_tag: Optional[str] = Field(
         default=None,
         description="(For self-hosted users) The Docker image tag used to run the model.",
     )
     """(For self-hosted users) The Docker image tag used to run the model."""
+
     num_shards: Optional[int] = Field(
         default=None, description="(For self-hosted users) The number of shards."
     )
     """(For self-hosted users) The number of shards."""
+
     quantize: Optional[Quantization] = Field(
         default=None, description="(For self-hosted users) The quantization method."
     )
     """(For self-hosted users) The quantization method."""
+
     spec: Optional[GetModelEndpointResponse] = Field(
         default=None, description="(For self-hosted users) Model endpoint details."
     )
     """(For self-hosted users) Model endpoint details."""
 
 
 class ListLLMEndpointsResponse(BaseModel):
@@ -243,15 +263,21 @@
 
 class CompletionSyncResponse(BaseModel):
     """
     Response object for a synchronous prompt completion.
     """
 
     request_id: str
-    """Unique ID of request."""
+    """The unique ID of the corresponding Completion request. This `request_id` is generated on the server, and all logs 
+    associated with the request are grouped by the `request_id`, which allows for easier troubleshooting of errors as
+    follows:
+
+    * When running the *Scale-hosted* LLM Engine, please provide the `request_id` in any bug reports.
+    * When running the *self-hosted* LLM Engine, the `request_id` serves as a trace ID in your observability 
+    provider."""
 
     output: CompletionOutput
     """Completion output."""
 
 
 class CompletionStreamV1Request(BaseModel):
     """
@@ -276,15 +302,21 @@
 
 class CompletionStreamResponse(BaseModel):
     """
     Response object for a stream prompt completion task.
     """
 
     request_id: str
-    """Unique ID of request."""
+    """The unique ID of the corresponding Completion request. This `request_id` is generated on the server, and all logs 
+    associated with the request are grouped by the `request_id`, which allows for easier troubleshooting of errors as
+    follows:
+
+    * When running the *Scale-hosted* LLM Engine, please provide the `request_id` in any bug reports.
+    * When running the *self-hosted* LLM Engine, the `request_id` serves as a trace ID in your observability 
+    provider."""
 
     output: Optional[CompletionStreamOutput] = None
     """Completion output."""
 
 
 class CreateFineTuneRequest(BaseModel):
     """
```

### Comparing `scale_llm_engine-0.0.0b3/llmengine/errors.py` & `scale_llm_engine-0.0.0b4/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b3/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b4/llmengine/fine_tuning.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 from llmengine.api_engine import DEFAULT_TIMEOUT, APIEngine
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CreateFineTuneRequest,
     CreateFineTuneResponse,
     GetFineTuneEventsResponse,
@@ -11,71 +11,79 @@
 )
 
 
 class FineTune(APIEngine):
     """
     FineTune API. This API is used to fine-tune models.
 
-    Fine-tuning is a process where the LLM is further trained on a task-specific dataset, allowing the model to adjust its parameters to better align with the task at hand. Fine-tuning is a supervised training phase, where prompt/response pairs are provided to optimize the performance of the LLM.
+    Fine-tuning is a process where the LLM is further trained on a task-specific dataset, allowing the model to adjust its parameters to better align with the task at hand. Fine-tuning is a supervised training phase, where prompt/response pairs are provided to optimize the performance of the LLM. LLM Engine currently uses [LoRA](https://arxiv.org/abs/2106.09685) for fine-tuning. Support for additional fine-tuning methods is upcoming.
 
     LLM Engine provides APIs to create fine-tunes on a base model with training & validation datasets. APIs are also provided to list, cancel and retrieve fine-tuning jobs.
 
     Creating a fine-tune will end with the creation of a Model, which you can view using `Model.get(model_name)` or delete using `Model.delete(model_name)`.
     """
 
     @classmethod
     def create(
         cls,
         model: str,
         training_file: str,
         validation_file: Optional[str] = None,
-        hyperparameters: Optional[Dict[str, str]] = None,
+        hyperparameters: Optional[Dict[str, Union[str, int, float]]] = None,
         suffix: Optional[str] = None,
     ) -> CreateFineTuneResponse:
         """
-        Creates a job that fine-tunes a specified model from a given dataset.
+        Creates a job that fine-tunes a specified model with a given dataset.
 
         This API can be used to fine-tune a model. The _model_ is the name of base model
         ([Model Zoo](../../model_zoo) for available models) to fine-tune. The training
-        file should consist of prompt and response pairs. Your data must be formatted as a CSV file
+        and validation files should consist of prompt and response pairs. `training_file`
+        and `validation_file` must be publicly accessible HTTP or HTTPS URLs to a CSV file
         that includes two columns: `prompt` and `response`. A maximum of 100,000 rows of data is
         currently supported. At least 200 rows of data is recommended to start to see benefits from
-        fine-tuning.
+        fine-tuning. For sequences longer than the native `max_seq_length` of the model, the sequences
+        will be truncated.
+
+        A fine-tuning job can take roughly 30 minutes for a small dataset (~200 rows)
+        and several hours for larger ones.
 
         Args:
             model (`str`):
                 The name of the base model to fine-tune. See [Model Zoo](../../model_zoo) for the list of available models to fine-tune.
 
             training_file (`str`):
                 Publicly accessible URL to a CSV file for training.
 
             validation_file (`Optional[str]`):
-                Publicly accessible URL to a CSV file for validation.
+                Publicly accessible URL to a CSV file for validation. The validation file is used to compute metrics which let LLM Engine pick the best fine-tuned checkpoint, which will be used for inference when fine-tuning is complete.
 
             hyperparameters (`Optional[Dict[str, str]]`):
                 A dict of hyperparameters to customize fine-tuning behavior.
 
                 Currently supported hyperparameters:
 
-                * `lr`: Peak learning rate used during fine-tuning. It decays with a cosine schedule afterward. (Default: 2e-5)
+                * `lr`: Peak learning rate used during fine-tuning. It decays with a cosine schedule afterward. (Default: 2e-3)
                 * `warmup_ratio`: Ratio of training steps used for learning rate warmup. (Default: 0.03)
-                * `epochs`: Number of fine-tuning epochs. (Default: 5)
+                * `epochs`: Number of fine-tuning epochs. This should be less than 20. (Default: 5)
                 * `weight_decay`: Regularization penalty applied to learned weights. (Default: 0.001)
-                * `max_seq_length`: Maximum number of tokens per sequence in the dataset. (Default: 1024)
 
             suffix (`Optional[str]`):
-                A string that will be added to your fine-tuned model name.
+                A string that will be added to your fine-tuned model name. If present, the entire fine-tuned model name
+                will be formatted like `"[model].[suffix].[YYYY-MM-DD-HH-MM-SS]"`. If absent, the
+                fine-tuned model name will be formatted `"[model].[YYYY-MM-DD-HH-MM-SS]"`.
+                For example, if `suffix` is `"my-experiment"`, the fine-tuned model name could be
+                `"llama-2-7b.my-experiment.2023-07-17-23-01-50"`.
 
         Returns:
             CreateFineTuneResponse: an object that contains the ID of the created fine-tuning job
 
         Here is an example script to create a 5-row CSV of properly formatted data for fine-tuning
         an airline question answering bot:
 
-        === "Formatting data in python"
+        === "Formatting data in Python"
         ```python
         import csv
 
         # Define data
         data = [
           ("What is your policy on carry-on luggage?", "Our policy allows each passenger to bring one piece of carry-on luggage and one personal item such as a purse or briefcase. The maximum size for carry-on luggage is 22 x 14 x 9 inches."),
           ("How can I change my flight?", "You can change your flight through our website or mobile app. Go to 'Manage my booking' section, enter your booking reference and last name, then follow the prompts to change your flight."),
@@ -87,31 +95,40 @@
         # Write data to a CSV file
         with open('customer_service_data.csv', 'w', newline='') as file:
             writer = csv.writer(file)
             writer.writerow(["prompt", "response"])
             writer.writerows(data)
         ```
 
+        Currently, data needs to be uploaded to a publicly accessible web URL so that it can be read
+        for fine-tuning. Publicly accessible HTTP and HTTPS URLs are currently supported.
+        Support for privately sharing data with the LLM Engine API is coming shortly. For quick
+        iteration, you can look into tools like Pastebin or GitHub Gists to quickly host your CSV
+        files in a public manner. An example Github Gist can be found
+        [here](https://gist.github.com/tigss/7cec73251a37de72756a3b15eace9965). To use the gist,
+        you can use the URL given when you click the “Raw” button
+        ([URL](https://gist.githubusercontent.com/tigss/7cec73251a37de72756a3b15eace9965/raw/85d9742890e1e6b0c06468507292893b820c13c9/llm_sample_data.csv)).
+
         Example code for fine-tuning:
-        === "Fine-tuning in python"
+        === "Fine-tuning in Python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.create(
-                model="llama-7b",
+                model="llama-2-7b",
                 training_file="https://my-bucket.s3.us-west-2.amazonaws.com/path/to/training-file.csv",
             )
 
             print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
-                "fine_tune_id": "ft_abc123"
+                "fine_tune_id": "ft-cir3eevt71r003ks6il0"
             }
             ```
 
         """
         request = CreateFineTuneRequest(
             model=model,
             training_file=training_file,
@@ -144,29 +161,29 @@
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
             GetFineTuneResponse: an object that contains the ID and status of the requested job
 
-        === "Getting status of fine-tuning in python"
+        === "Getting status of fine-tuning in Python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.get(
-                fine_tune_id="ft_abc123",
+                fine_tune_id="ft-cir3eevt71r003ks6il0",
             )
 
             print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
-                "fine_tune_id": "ft_abc123",
+                "fine_tune_id": "ft-cir3eevt71r003ks6il0",
                 "status": "STARTED"
             }
             ```
         """
         response = cls._get(f"v1/llm/fine-tunes/{fine_tune_id}", timeout=DEFAULT_TIMEOUT)
         return GetFineTuneResponse.parse_obj(response)
 
@@ -178,28 +195,28 @@
         This API can be used to list all the fine-tuning jobs.
         It returns a list of pairs of `fine_tune_id` and `status` for
         all existing jobs.
 
         Returns:
             ListFineTunesResponse: an object that contains a list of all fine-tuning jobs and their statuses
 
-        === "Listing fine-tuning jobs in python"
+        === "Listing fine-tuning jobs in Python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.list()
             print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
                 "jobs": [
                     {
-                        "fine_tune_id": "ft_abc123",
+                        "fine_tune_id": "ft-cir3eevt71r003ks6il0",
                         "status": "STARTED"
                     },
                     {
                         "fine_tune_id": "ft_def456",
                         "status": "SUCCESS"
                     }
                 ]
@@ -211,34 +228,34 @@
 
     @classmethod
     def cancel(cls, fine_tune_id: str) -> CancelFineTuneResponse:
         """
         Cancel a fine-tuning job.
 
         This API can be used to cancel an existing fine-tuning job if
-        it's no longer required. It takes as parameter the `fine_tune_id`
+        it's no longer required. It takes the `fine_tune_id` as a parameter
         and returns a response object which has a `success` field
         confirming if the cancellation was successful.
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
             CancelFineTuneResponse: an object that contains whether the cancellation was successful
 
-        === "Cancelling fine-tuning job in python"
+        === "Cancelling fine-tuning job in Python"
             ```python
             from llmengine import FineTune
 
-            response = FineTune.cancel(fine_tune_id="ft_abc123")
+            response = FineTune.cancel(fine_tune_id="ft-cir3eevt71r003ks6il0")
             print(response.json())
             ```
 
-        === "Response in json"
+        === "Response in JSON"
             ```json
             {
                 "success": true
             }
             ```
         """
         response = cls.put(
@@ -249,48 +266,59 @@
         return CancelFineTuneResponse.parse_obj(response)
 
     @classmethod
     def get_events(cls, fine_tune_id: str) -> GetFineTuneEventsResponse:
         """
         Get events of a fine-tuning job.
 
-        This API can be used to get the list of events for a fine-tuning job.
-        It takes as parameter the `fine_tune_id` and returns a response object
-        which has a list of events that has happened for the fine-tuning job.
+        This API can be used to get the list of detailed events for a fine-tuning job.
+        It takes the `fine_tune_id` as a parameter and returns a response object
+        which has a list of events that has happened for the fine-tuning job. Two events
+        are logged periodically: an evaluation of the training loss, and an
+        evaluation of the eval loss. This API will return all events for the fine-tuning job.
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
             GetFineTuneEventsResponse: an object that contains the list of events for the fine-tuning job
 
-        Example:
+        === "Getting events for  fine-tuning jobs in Python"
             ```python
             from llmengine import FineTune
 
-            response = FineTune.get_events(fine_tune_id="ft_abc123")
+            response = FineTune.get_events(fine_tune_id="ft-cir3eevt71r003ks6il0")
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in JSON"
             ```json
             {
+                "events":
                 [
                     {
-                        "timestamp": 1689644480.0,
-                        "message": "Fine-tune job created",
-                        "level": "INFO"
-                    }
-                ],
-                [
+                        "timestamp": 1689665099.6704428,
+                        "message": "{'loss': 2.108, 'learning_rate': 0.002, 'epoch': 0.7}",
+                        "level": "info"
+                    },
+                    {
+                        "timestamp": 1689665100.1966307,
+                        "message": "{'eval_loss': 1.67730712890625, 'eval_runtime': 0.2023, 'eval_samples_per_second': 24.717, 'eval_steps_per_second': 4.943, 'epoch': 0.7}",
+                        "level": "info"
+                    },
+                    {
+                        "timestamp": 1689665105.6544185,
+                        "message": "{'loss': 1.8961, 'learning_rate': 0.0017071067811865474, 'epoch': 1.39}",
+                        "level": "info"
+                    },
                     {
-                        "timestamp": 1689645480.0,
-                        "message": "Fine-tune job finished",
-                        "level": "INFO"
+                        "timestamp": 1689665106.159139,
+                        "message": "{'eval_loss': 1.513688564300537, 'eval_runtime': 0.2025, 'eval_samples_per_second': 24.696, 'eval_steps_per_second': 4.939, 'epoch': 1.39}",
+                        "level": "info"
                     }
                 ]
             }
             ```
         """
         response = cls._get(
             f"v1/llm/fine-tunes/{fine_tune_id}/events",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scale_llm_engine-0.0.0b3/pyproject.toml` & `scale_llm_engine-0.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta3"
+version = "0.0.0.beta4"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b3/PKG-INFO` & `scale_llm_engine-0.0.0b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b3
+Version: 0.0.0b4
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
@@ -35,26 +35,26 @@
 ```shell
 pip install scale-llm-engine
 ```
 
 ### Usage
 
 If you are using LLM Engine, you can get your API key from
-[https://spellbook.scale.com/settings](https://spellbook.scale.com/settings). 
+[https://spellbook.scale.com/settings](https://spellbook.scale.com/settings).
 Set the `SCALE_API_KEY` environment variable to your API key.
 
 If you are using your own infrastructure, you can set the
 `LLM_ENGINE_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `llmengine` endpoint.
 
 ```python
 from llmengine import Completion
 
 response = Completion.create(
-    model="llama-7b",
+    model="llama-2-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
```

