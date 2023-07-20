# Comparing `tmp/compel-2.0.0rc2.tar.gz` & `tmp/compel-2.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-cnb_kmek/compel-2.0.0rc2.tar", last modified: Fri Jul 14 09:35:16 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-f99dy6mm/compel-2.0.1rc1.tar", last modified: Thu Jul 20 18:55:38 2023, max compression
```

## Comparing `compel-2.0.0rc2.tar` & `compel-2.0.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.0rc2/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-14 09:35:16.000000 compel-2.0.0rc2/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    10494 2023-07-04 22:01:43.000000 compel-2.0.0rc2/README.md
--rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-14 09:33:35.000000 compel-2.0.0rc2/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-14 09:35:16.000000 compel-2.0.0rc2/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.0rc2/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    20356 2023-07-14 09:32:50.000000 compel-2.0.0rc2/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.0rc2/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.0rc2/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.0rc2/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    30339 2023-07-12 22:57:28.000000 compel-2.0.0rc2/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.0rc2/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/test/
--rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-12 22:58:27.000000 compel-2.0.0rc2/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.0rc2/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.0rc2/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.1rc1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    11669 2023-07-18 14:01:58.000000 compel-2.0.1rc1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-20 18:55:28.000000 compel-2.0.1rc1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-20 18:55:38.000000 compel-2.0.1rc1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    20730 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.1rc1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.1rc1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    30822 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.1rc1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-18 10:18:45.000000 compel-2.0.1rc1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.1rc1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.1rc1/test/test_prompt_parser.py
```

### Comparing `compel-2.0.0rc2/LICENSE` & `compel-2.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/PKG-INFO` & `compel-2.0.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.0rc2
+Version: 2.0.1rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,14 +95,33 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+### 2.0.0 - SDXL Support
+
+With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
+
+```
+from compel import Compel, ReturnedEmbeddingsType
+from diffusers import DiffusionPipeline
+pipeline = DiffusionPipeline.from_pretrained("stabilityai/stable-diffusion-xl-base-0.9", variant="fp16", use_safetensors=True, torch_dtype=torch.float16).to("cuda")
+compel = Compel(tokenizer=[pipeline.tokenizer, pipeline.tokenizer_2] , text_encoder=[pipeline.text_encoder, pipeline.text_encoder_2], returned_embeddings_type=ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED, requires_pooled=[False, True])
+# upweight "ball"
+prompt = "a cat playing with a ball++ in the forest"
+conditioning, pooled = compel(prompt)
+# generate image
+image = pipeline(prompt_embeds=conditioning, pooled_prompt_embeds=pooled, num_inference_steps=30).images[0]
+```
+
+Please note that this is a **breaking change** if you've been using clip skip: the old boolean arg `use_penultimate_clip_layer` has been replaced with an enum `ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED`.
+
+
 #### 1.2.1 - actually apply `.and()` weights
 
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`.
```

### Comparing `compel-2.0.0rc2/README.md` & `compel-2.0.1rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,33 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+### 2.0.0 - SDXL Support
+
+With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
+
+```
+from compel import Compel, ReturnedEmbeddingsType
+from diffusers import DiffusionPipeline
+pipeline = DiffusionPipeline.from_pretrained("stabilityai/stable-diffusion-xl-base-0.9", variant="fp16", use_safetensors=True, torch_dtype=torch.float16).to("cuda")
+compel = Compel(tokenizer=[pipeline.tokenizer, pipeline.tokenizer_2] , text_encoder=[pipeline.text_encoder, pipeline.text_encoder_2], returned_embeddings_type=ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED, requires_pooled=[False, True])
+# upweight "ball"
+prompt = "a cat playing with a ball++ in the forest"
+conditioning, pooled = compel(prompt)
+# generate image
+image = pipeline(prompt_embeds=conditioning, pooled_prompt_embeds=pooled, num_inference_steps=30).images[0]
+```
+
+Please note that this is a **breaking change** if you've been using clip skip: the old boolean arg `use_penultimate_clip_layer` has been replaced with an enum `ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED`.
+
+
 #### 1.2.1 - actually apply `.and()` weights
 
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`.
```

### Comparing `compel-2.0.0rc2/pyproject.toml` & `compel-2.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "2.0.0-pre2"
+version = "2.0.1-pre1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-2.0.0rc2/src/compel/compel.py` & `compel-2.0.1rc1/src/compel/compel.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,33 +25,37 @@
                  text_encoder: Union[CLIPTextModel, List[CLIPTextModel]],
                  textual_inversion_manager: Optional[BaseTextualInversionManager] = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate_long_prompts: bool = True,
                  padding_attention_mask_value: int = 1,
                  downweight_mode: DownweightMode = DownweightMode.MASK,
                  returned_embeddings_type: ReturnedEmbeddingsType = ReturnedEmbeddingsType.LAST_HIDDEN_STATES_NORMALIZED,
-                 requires_pooled: bool = False,
+                 requires_pooled: Union[bool, List[bool]] = False,
                  device: Optional[str] = None
                  ):
         """
-        Initialize Compel. The tokenizer and text_encoder can be lifted directly from any DiffusionPipeline.
+        Initialize Compel. The tokenizer and text_encoder can be lifted directly from any DiffusionPipeline. For SDXL,
+        you'll be using multiple Tokenizers and multiple Text Encoders - see `https://github.com/damian0815/compel/pull/41`
+        for details.
 
         `textual_inversion_manager`: Optional instance to handle expanding multi-vector textual inversion tokens.
         `dtype_for_device_getter`: A Callable that returns a torch dtype for a given device. You probably don't need to
             use this.
         `truncate_long_prompts`: if True, truncate input prompts to 77 tokens long including beginning/end markers
             (default behaviour).
             If False, do not truncate, and instead assemble as many 77 token long chunks, each capped by beginning/end
             markers, as is necessary to encode the whole prompt. You will likely need to supply both positive and
             negative prompts in this case - use `pad_conditioning_tensors_to_same_length` to prevent having tensor
             length mismatch errors when passing the embeds on to your DiffusionPipeline for inference.
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: Specifies whether downweighting should be applied by MASKing out the downweighted tokens
             (default) or REMOVEing them (legacy behaviour; messes up position embeddings of tokens following).
-        `returned_embeddings_type`: controls how the embedding vectors are taken from the result of running the text encoder over the parsed prompt's text
+        `returned_embeddings_type`: controls how the embedding vectors are taken from the result of running the text
+            encoder over the parsed prompt's text. For SD<=2.1, use LAST_HIDDEN_STATES_NORMALIZED, or
+            PENULTIMATE_HIDDEN_STATES_NORMALIZED if you want to do "clip skip". For SDXL use PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED.
         `requires_pooled`: for SDXL, append the pooled embeddings when returning conditioning tensors
         `device`: The torch device on which the tensors should be created. If a device is not specified, the device will
             be the same as that of the `text_encoder` at the moment when `build_conditioning_tensor()` is called.
         """
         if isinstance(tokenizer, (tuple, list)) and not isinstance(text_encoder, (tuple, list)):
             raise ValueError("Cannot provide list of tokenizers, but not of text encoders.")
         elif not isinstance(tokenizer, (tuple, list)) and isinstance(text_encoder, (tuple, list)):
@@ -102,15 +106,15 @@
         Build a conditioning tensor by parsing the text for Compel syntax, constructing a Conjunction, and then
         building a conditioning tensor from that Conjunction.
         """
         conjunction = self.parse_prompt_string(text)
         conditioning, _ = self.build_conditioning_tensor_for_conjunction(conjunction)
 
         if self.requires_pooled:
-            pooled = self.conditioning_provider.get_pooled_embeddings([text])
+            pooled = self.conditioning_provider.get_pooled_embeddings([text] )
             return conditioning, pooled
         else:
             return conditioning
 
     @torch.no_grad()
     def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
         """
```

### Comparing `compel-2.0.0rc2/src/compel/conditioning_scheduler.py` & `compel-2.0.1rc1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/src/compel/cross_attention_control.py` & `compel-2.0.1rc1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/src/compel/diffusers_textual_inversion_manager.py` & `compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/src/compel/embeddings_provider.py` & `compel-2.0.1rc1/src/compel/embeddings_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         `textual_inversion_manager`: manage token insertion for textual inversions with vector length >1
         `dtype_for_device_getter`: callback that returns an appropriate dtype for the requested device. if unset, defaults to torch.float32.
         `truncate`: if True, truncate inputs to the maximum length specified by the tokenizer. if False, returns
                     tensors that may be longer than the maximum length (but will always be an integer multiple of maximum length)
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: if MASK, downweight by blending with a version of the prompt with the downweighted terms masked out.
                     if REMOVE, the blend is against a version of the prompt with the downweighted tokens removed
-        `use_penultimate_clip_layer`: Whether to tuse the penultimate hidden state output of the CLIP emcoder (True) or
-                    the final hidden state output (False, default).
-        `requires_pooled`:
+        `returned_embeddings_type`: controls how the embedding vectors are taken from the result of running the text
+            encoder over the parsed prompt's text. For SD<=2.1, use LAST_HIDDEN_STATES_NORMALIZED, or
+            PENULTIMATE_HIDDEN_STATES_NORMALIZED if you want to do "clip skip". For SDXL use PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED.
         """
         self.tokenizer = tokenizer
         self.text_encoder = text_encoder
         self.textual_inversion_manager = textual_inversion_manager
         self.truncate_to_model_max_length = truncate
         self.padding_attention_mask_value = padding_attention_mask_value
         self.downweight_mode = downweight_mode
@@ -186,31 +186,35 @@
         #print(f"assembled all tokens into tensor of shape {batch_z.shape}")
 
         if should_return_tokens:
             return batch_z, batch_tokens
         else:
             return batch_z
 
-    def get_token_ids(self, texts: List[str], include_start_and_end_markers: bool = True, padding: str = 'do_not_pad') -> List[List[int]]:
+    def get_token_ids(self, texts: List[str], include_start_and_end_markers: bool = True, padding: str = 'do_not_pad',
+                      truncation_override: Optional[bool] = None) -> List[List[int]]:
         """
         Convert a list of strings like `["a cat", "a dog", "monkey riding a bicycle"]` into a list of lists of token
         ids like `[[bos, 0, 1, eos], [bos, 0, 2, eos], [bos, 3, 4, 0, 5, eos]]`. bos/eos markers are skipped if
         `include_start_and_end_markers` is `False`. Each list will be restricted to the maximum permitted length
         (typically 75 tokens + eos/bos markers).
 
         :param texts: The strings to convert.
         :param include_start_and_end_markers: If True (default), returned token id lists will start with the beginning
             of sequence marker and end with the end-of-sequence marker (`eos`).
+        :padding: Padding argument passed through to the Tokenizer.
+        :truncation_override: Optional, overrides the `truncate` argument passed to `__init__`.
         :return: A list of lists of token ids corresponding to the input strings.
         """
         # for args documentation of self.tokenizer() see ENCODE_KWARGS_DOCSTRING in tokenization_utils_base.py
         # (part of `transformers` lib)
+        truncation = self.truncate_to_model_max_length if truncation_override is None else truncation_override
         token_ids_list = self.tokenizer(
             texts,
-            truncation=self.truncate_to_model_max_length,
+            truncation=truncation,
             padding=padding,
             return_tensors=None,  # just give me lists of ints
         )['input_ids']
 
         result = []
         for token_ids in token_ids_list:
             # trim eos/bos
@@ -224,15 +228,15 @@
                 token_ids = [self.tokenizer.bos_token_id] + token_ids + [self.tokenizer.eos_token_id]
 
             result.append(token_ids)
 
         return result
 
     def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None) -> Optional[torch.Tensor]:
-        token_ids = self.get_token_ids(texts, padding="max_length")
+        token_ids = self.get_token_ids(texts, padding="max_length", truncation_override=True)
         token_ids = torch.tensor(token_ids, dtype=torch.long).to(self.text_encoder.device)
 
         text_encoder_output = self.text_encoder(token_ids, attention_mask, return_dict=True)
         pooled = text_encoder_output.text_embeds
 
         return pooled
```

### Comparing `compel-2.0.0rc2/src/compel/prompt_parser.py` & `compel-2.0.1rc1/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/src/compel.egg-info/PKG-INFO` & `compel-2.0.1rc1/src/compel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.0rc2
+Version: 2.0.1rc1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,14 +95,33 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+### 2.0.0 - SDXL Support
+
+With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
+
+```
+from compel import Compel, ReturnedEmbeddingsType
+from diffusers import DiffusionPipeline
+pipeline = DiffusionPipeline.from_pretrained("stabilityai/stable-diffusion-xl-base-0.9", variant="fp16", use_safetensors=True, torch_dtype=torch.float16).to("cuda")
+compel = Compel(tokenizer=[pipeline.tokenizer, pipeline.tokenizer_2] , text_encoder=[pipeline.text_encoder, pipeline.text_encoder_2], returned_embeddings_type=ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NON_NORMALIZED, requires_pooled=[False, True])
+# upweight "ball"
+prompt = "a cat playing with a ball++ in the forest"
+conditioning, pooled = compel(prompt)
+# generate image
+image = pipeline(prompt_embeds=conditioning, pooled_prompt_embeds=pooled, num_inference_steps=30).images[0]
+```
+
+Please note that this is a **breaking change** if you've been using clip skip: the old boolean arg `use_penultimate_clip_layer` has been replaced with an enum `ReturnedEmbeddingsType.PENULTIMATE_HIDDEN_STATES_NORMALIZED`.
+
+
 #### 1.2.1 - actually apply `.and()` weights
 
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`.
```

### Comparing `compel-2.0.0rc2/src/compel.egg-info/SOURCES.txt` & `compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/test/test_compel.py` & `compel-2.0.1rc1/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/test/test_embeddings_provider.py` & `compel-2.0.1rc1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc2/test/test_prompt_parser.py` & `compel-2.0.1rc1/test/test_prompt_parser.py`

 * *Files identical despite different names*

