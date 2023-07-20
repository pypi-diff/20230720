# Comparing `tmp/harmonai-tools-0.0.2.tar.gz` & `tmp/harmonai-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonai-tools-0.0.2.tar", last modified: Tue Jul 18 06:06:43 2023, max compression
+gzip compressed data, was "harmonai-tools-0.0.3.tar", last modified: Thu Jul 20 08:28:29 2023, max compression
```

## Comparing `harmonai-tools-0.0.2.tar` & `harmonai-tools-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.2/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/__init__.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/data/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/data/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.2/harmonai_tools/data/dataset.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/data/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/inference/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/inference/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2931 2023-07-13 09:03:05.000000 harmonai-tools-0.0.2/harmonai_tools/inference/generation.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5195 2023-07-10 05:18:12.000000 harmonai-tools-0.0.2/harmonai_tools/inference/sampling.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/interface/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.2/harmonai_tools/interface/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4472 2023-07-10 05:25:04.000000 harmonai-tools-0.0.2/harmonai_tools/interface/gradio.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/models/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15254 2023-07-12 02:44:15.000000 harmonai-tools-0.0.2/harmonai_tools/models/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.2/harmonai_tools/models/blocks.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.2/harmonai_tools/models/bottleneck.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11828 2023-07-15 04:13:53.000000 harmonai-tools-0.0.2/harmonai_tools/models/conditioners.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17998 2023-07-15 04:57:40.000000 harmonai-tools-0.0.2/harmonai_tools/models/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.2/harmonai_tools/models/discriminators.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4114 2023-07-12 03:20:54.000000 harmonai-tools-0.0.2/harmonai_tools/models/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/pretransforms.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/wavelets.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/training/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.2/harmonai_tools/training/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11635 2023-07-15 02:48:45.000000 harmonai-tools-0.0.2/harmonai_tools/training/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18736 2023-07-11 18:15:31.000000 harmonai-tools-0.0.2/harmonai_tools/training/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4457 2023-07-12 02:51:29.000000 harmonai-tools-0.0.2/harmonai_tools/training/factory.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1041 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      409 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.2/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1088 2023-07-18 06:06:26.000000 harmonai-tools-0.0.2/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.3/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/__init__.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/data/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/data/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.3/harmonai_tools/data/dataset.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/data/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/inference/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/inference/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2961 2023-07-20 08:07:05.000000 harmonai-tools-0.0.3/harmonai_tools/inference/generation.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5195 2023-07-10 05:18:12.000000 harmonai-tools-0.0.3/harmonai_tools/inference/sampling.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/interface/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.3/harmonai_tools/interface/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4641 2023-07-20 08:25:46.000000 harmonai-tools-0.0.3/harmonai_tools/interface/gradio.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/models/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15254 2023-07-12 02:44:15.000000 harmonai-tools-0.0.3/harmonai_tools/models/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.3/harmonai_tools/models/blocks.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.3/harmonai_tools/models/bottleneck.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    12143 2023-07-18 19:21:16.000000 harmonai-tools-0.0.3/harmonai_tools/models/conditioners.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17998 2023-07-15 04:57:40.000000 harmonai-tools-0.0.3/harmonai_tools/models/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.3/harmonai_tools/models/discriminators.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4114 2023-07-12 03:20:54.000000 harmonai-tools-0.0.3/harmonai_tools/models/factory.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/pretransforms.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.3/harmonai_tools/models/wavelets.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools/training/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.3/harmonai_tools/training/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11803 2023-07-19 19:11:44.000000 harmonai-tools-0.0.3/harmonai_tools/training/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18736 2023-07-11 18:15:31.000000 harmonai-tools-0.0.3/harmonai_tools/training/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4457 2023-07-12 02:51:29.000000 harmonai-tools-0.0.3/harmonai_tools/training/factory.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1041 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      417 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/harmonai_tools.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.3/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-20 08:28:29.000000 harmonai-tools-0.0.3/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1096 2023-07-20 08:28:12.000000 harmonai-tools-0.0.3/setup.py
```

### Comparing `harmonai-tools-0.0.2/LICENSE` & `harmonai-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/data/dataset.py` & `harmonai-tools-0.0.3/harmonai_tools/data/dataset.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/data/utils.py` & `harmonai-tools-0.0.3/harmonai_tools/data/utils.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/inference/generation.py` & `harmonai-tools-0.0.3/harmonai_tools/inference/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,21 @@
         if io_channels == 1:
             # Convert to mono
             init_audio = init_audio.mean(1, keepdim=True)
 
         if model.pretransform is not None:
             init_audio = model.pretransform.encode(init_audio)
 
-        sampled = variation_k(model.model, init_audio, init_noise_level, steps, **sampler_kwargs, **conditioning_tensors, cfg_scale=cfg_scale, batch_cfg=True, scale_cfg=True)
+        sampled = variation_k(model.model, init_audio, init_noise_level, steps, **sampler_kwargs, **conditioning_tensors, cfg_scale=cfg_scale, batch_cfg=True, scale_cfg=True, device=device)
     else:
         if model.pretransform is not None:
             sample_size = sample_size // model.pretransform.downsampling_ratio
 
         noise = torch.randn([batch_size, model.io_channels, sample_size], device=device)
-        sampled = sample_k(model.model, noise, steps, **sampler_kwargs, **conditioning_tensors, cfg_scale=cfg_scale, batch_cfg=True, scale_cfg=True)
+        sampled = sample_k(model.model, noise, steps, **sampler_kwargs, **conditioning_tensors, cfg_scale=cfg_scale, batch_cfg=True, scale_cfg=True, device=device)
 
 
     if model.pretransform is not None:
         sampled = model.pretransform.decode(sampled)
 
     return sampled
```

### Comparing `harmonai-tools-0.0.2/harmonai_tools/inference/sampling.py` & `harmonai-tools-0.0.3/harmonai_tools/inference/sampling.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/interface/gradio.py` & `harmonai-tools-0.0.3/harmonai_tools/interface/gradio.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         init_noise_level=1.0,
         batch_size=1,
         ):
     # Return fake stereo audio
 
     conditioning = [{"prompt": prompt, "seconds_start": seconds_start, "seconds_total": seconds_total}] * batch_size
 
+    #Get the device from the model
+    device = next(model.parameters()).device
+
     seed = int(seed)
 
     if not use_init:
         init_audio = None
     
     if init_audio is not None:
         in_sr, init_audio = init_audio
@@ -66,15 +69,15 @@
         conditioning=conditioning,
         steps=steps,
         cfg_scale=cfg_scale,
         batch_size=batch_size,
         sample_size=sample_size,
         sample_rate=sample_rate,
         seed=seed,
-        device="cuda",
+        device=device,
         sampler_type=sampler_type,
         sigma_min=sigma_min,
         sigma_max=sigma_max,
         init_audio=init_audio,
         init_noise_level=init_noise_level,
     )
 
@@ -91,29 +94,29 @@
     
     with gr.Row():
         # Timing controls
         seconds_start_slider = gr.Slider(minimum=0, maximum=512, step=1, value=0, label="Seconds start")
         seconds_total_slider = gr.Slider(minimum=0, maximum=512, step=1, value=60, label="Seconds total")
         
         # Steps slider
-        steps_slider = gr.Slider(minimum=1, maximum=500, step=1, value=250, label="Steps")
+        steps_slider = gr.Slider(minimum=1, maximum=500, step=1, value=200, label="Steps")
 
         # CFG scale 
-        cfg_scale_slider = gr.Slider(minimum=0.0, maximum=25.0, step=0.1, value=6.0, label="CFG scale")
+        cfg_scale_slider = gr.Slider(minimum=0.0, maximum=25.0, step=0.1, value=7.0, label="CFG scale")
 
     with gr.Accordion("Sampler params", open=False):
     
         # Seed
         seed_textbox = gr.Textbox(label="Seed (set to -1 for random seed)", value="-1")
 
     # Sampler params
         with gr.Row():
             sampler_type_dropdown = gr.Dropdown(["dpmpp-2m-sde", "k-heun", "k-lms", "k-dpmpp-2s-ancestral", "k-dpm-2", "k-dpm-fast"], label="Sampler type", value="dpmpp-2m-sde")
-            sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.5, label="Sigma min")
-            sigma_max_slider = gr.Slider(minimum=0.0, maximum=100.0, step=0.1, value=50.0, label="Sigma max")
+            sigma_min_slider = gr.Slider(minimum=0.0, maximum=2.0, step=0.01, value=0.95, label="Sigma min")
+            sigma_max_slider = gr.Slider(minimum=0.0, maximum=100.0, step=0.1, value=77, label="Sigma max")
 
     with gr.Accordion("Init audio", open=False):
         init_audio_checkbox = gr.Checkbox(label="Use init audio")
         init_audio_input = gr.Audio(label="Init audio")
         init_noise_level_slider = gr.Slider(minimum=0.0, maximum=100.0, step=0.01, value=0.1, label="Init noise level")
 
     audio_output = gr.Audio(label="Output audio")
@@ -132,13 +135,14 @@
         init_audio_checkbox,
         init_audio_input,
         init_noise_level_slider,
         ], outputs=audio_output, api_name="generate")
 
 
 def create_ui(model_config, ckpt_path):
-    load_model(model_config, ckpt_path)
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    load_model(model_config, ckpt_path, device=device)
     with gr.Blocks() as ui:
         with gr.Tab("Generation"):
             create_sampling_ui()
         
     return ui
```

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/autoencoders.py` & `harmonai-tools-0.0.3/harmonai_tools/models/autoencoders.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/blocks.py` & `harmonai-tools-0.0.3/harmonai_tools/models/blocks.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/bottleneck.py` & `harmonai-tools-0.0.3/harmonai_tools/models/bottleneck.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/conditioners.py` & `harmonai-tools-0.0.3/harmonai_tools/models/conditioners.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,20 @@
         return prompt_features, attention_mask
 
     def forward(self, texts: tp.List[str], device: tp.Any = "cuda") -> tp.Any:
 
         self.model.to(device)
 
         if self.use_text_features:
-            text_features, text_attention_mask = self.get_clap_features(texts, layer_ix=self.feature_layer_ix, device=device)
+            if len(texts) == 1:
+                text_features, text_attention_mask = self.get_clap_features([texts[0], ""], layer_ix=self.feature_layer_ix, device=device)
+                text_features = text_features[:1, ...]
+                text_attention_mask = text_attention_mask[:1, ...]
+            else:
+                text_features, text_attention_mask = self.get_clap_features(texts, layer_ix=self.feature_layer_ix, device=device)
             return [self.proj_out(text_features), text_attention_mask]
 
         # Fix for CLAP bug when only one text is passed
         if len(texts) == 1:
             text_embedding = self.model.get_text_embedding([texts[0], ""], use_tensor=True)[:1, ...]
         else:
             text_embedding = self.model.get_text_embedding(texts, use_tensor=True)
```

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/diffusion.py` & `harmonai-tools-0.0.3/harmonai_tools/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/discriminators.py` & `harmonai-tools-0.0.3/harmonai_tools/models/discriminators.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/factory.py` & `harmonai-tools-0.0.3/harmonai_tools/models/factory.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/pretransforms.py` & `harmonai-tools-0.0.3/harmonai_tools/models/pretransforms.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/models/wavelets.py` & `harmonai-tools-0.0.3/harmonai_tools/models/wavelets.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/training/autoencoders.py` & `harmonai-tools-0.0.3/harmonai_tools/training/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,19 @@
                 
             
         self.log_dict(log_dict, prog_bar=True, on_step=True)
 
         return loss
     
     def export_model(self, path):
-        export_state_dict = {"state_dict": self.autoencoder.state_dict()}
+        if self.autoencoder_ema is not None:
+            export_state_dict = {"state_dict": self.autoencoder_ema.ema_model.state_dict()}
+        else:
+            export_state_dict = {"state_dict": self.autoencoder.state_dict()}
+            
         torch.save(export_state_dict, path)
         
 
 class AutoencoderDemoCallback(pl.Callback):
     def __init__(
         self, 
         demo_dl,
```

### Comparing `harmonai-tools-0.0.2/harmonai_tools/training/diffusion.py` & `harmonai-tools-0.0.3/harmonai_tools/training/diffusion.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools/training/factory.py` & `harmonai-tools-0.0.3/harmonai_tools/training/factory.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/harmonai_tools.egg-info/SOURCES.txt` & `harmonai-tools-0.0.3/harmonai_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.2/setup.py` & `harmonai-tools-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='harmonai-tools',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/Harmonai-org/harmonai-tools.git',
     author='Harmonai',
     description='Training and inference tools for generative audio models from Harmonai',
     packages=find_packages(),  
     install_requires=[
         'aeiou',
         'alias-free-torch',
@@ -29,15 +29,15 @@
         'PyWavelets',
         'sentencepiece',
         's3fs',
         'torch',
         'torchaudio',
         'torchmetrics==0.11.4',
         'tqdm',
-        'transformers',
+        'transformers==4.30.2',
         'v-diffusion-pytorch',
         'vector-quantize-pytorch',
         'wandb',
         'webdataset',
         'x-transformers'
     ],
 )
```

