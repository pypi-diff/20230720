# Comparing `tmp/descript-audio-codec-0.0.5.tar.gz` & `tmp/descript-audio-codec-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descript-audio-codec-0.0.5.tar", last modified: Wed Jul  5 15:59:29 2023, max compression
+gzip compressed data, was "descript-audio-codec-1.0.0.tar", last modified: Thu Jul 20 18:10:05 2023, max compression
```

## Comparing `descript-audio-codec-0.0.5.tar` & `descript-audio-codec-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/
--rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/LICENSE
--rw-r--r--   0 ishaan    (1016) research  (1001)     6342 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)     5585 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/README.md
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/
--rw-r--r--   0 ishaan    (1016) research  (1001)      237 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      690 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.5/dac/__main__.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/compare/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/compare/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/compare/encodec.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.291028 descript-audio-codec-0.0.5/dac/model/
--rw-r--r--   0 ishaan    (1016) research  (1001)       91 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     4190 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/base.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    10483 2023-06-14 20:20:06.000000 descript-audio-codec-0.0.5/dac/model/dac.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/model/discriminator.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/dac/nn/
--rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/layers.py
--rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/dac/nn/loss.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     9151 2023-06-19 19:31:34.000000 descript-audio-codec-0.0.5/dac/nn/quantize.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/dac/utils/
--rw-r--r--   0 ishaan    (1016) research  (1001)     2783 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     5901 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/decode.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     6367 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/dac/utils/encode.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/
--rw-r--r--   0 ishaan    (1016) research  (1001)     6342 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/PKG-INFO
--rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/SOURCES.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/dependency_links.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/requires.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-07-05 15:59:29.000000 descript-audio-codec-0.0.5/descript_audio_codec.egg-info/top_level.txt
--rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/setup.cfg
--rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/setup.py
-drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-05 15:59:29.295028 descript-audio-codec-0.0.5/tests/
--rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/tests/__init__.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2241 2023-07-05 15:59:13.000000 descript-audio-codec-0.0.5/tests/test_cli.py
--rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-0.0.5/tests/test_train.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.163054 descript-audio-codec-1.0.0/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1074 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/LICENSE
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7125 2023-07-20 18:10:05.163054 descript-audio-codec-1.0.0/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)     6368 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/README.md
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/dac/
+-rw-r--r--   0 ishaan    (1016) research  (1001)      307 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      666 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/__main__.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/dac/compare/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/compare/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1592 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/compare/encodec.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/dac/model/
+-rw-r--r--   0 ishaan    (1016) research  (1001)      117 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/model/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     9384 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/model/base.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    11064 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/model/dac.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7056 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/model/discriminator.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/dac/nn/
+-rw-r--r--   0 ishaan    (1016) research  (1001)       63 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/nn/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)      809 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/nn/layers.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)    12042 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/dac/nn/loss.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     9060 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/nn/quantize.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/dac/utils/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     3290 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/utils/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2998 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/utils/decode.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     3117 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/dac/utils/encode.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.159054 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/
+-rw-r--r--   0 ishaan    (1016) research  (1001)     7125 2023-07-20 18:10:05.000000 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/PKG-INFO
+-rw-r--r--   0 ishaan    (1016) research  (1001)      596 2023-07-20 18:10:05.000000 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)        1 2023-07-20 18:10:05.000000 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)      194 2023-07-20 18:10:05.000000 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/requires.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       10 2023-07-20 18:10:05.000000 descript-audio-codec-1.0.0/descript_audio_codec.egg-info/top_level.txt
+-rw-r--r--   0 ishaan    (1016) research  (1001)       38 2023-07-20 18:10:05.163054 descript-audio-codec-1.0.0/setup.cfg
+-rw-r--r--   0 ishaan    (1016) research  (1001)     1548 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/setup.py
+drwxr-xr-x   0 ishaan    (1016) research  (1001)        0 2023-07-20 18:10:05.163054 descript-audio-codec-1.0.0/tests/
+-rw-r--r--   0 ishaan    (1016) research  (1001)        0 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/tests/__init__.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2275 2023-07-20 18:09:56.000000 descript-audio-codec-1.0.0/tests/test_cli.py
+-rw-r--r--   0 ishaan    (1016) research  (1001)     2752 2023-06-13 21:55:11.000000 descript-audio-codec-1.0.0/tests/test_train.py
```

### Comparing `descript-audio-codec-0.0.5/LICENSE` & `descript-audio-codec-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/PKG-INFO` & `descript-audio-codec-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.5
+Version: 1.0.0
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -83,41 +83,50 @@
 It will also preserve the directory structure relative to input root and
 re-create it in the output directory. Please use `python -m dac decode --help`
 for more options.
 
 ### Programmatic Usage
 ```py
 import dac
-from dac.utils import load_model
-from dac.model import DAC
-
-from dac.utils.encode import process as encode
-from dac.utils.decode import process as decode
-
 from audiotools import AudioSignal
 
-# Init an empty model
-model = DAC()
+# Download a model
+model_path = dac.utils.download(model_type="44khz")
+model = dac.DAC.load(model_path)
 
-# Load compatible pre-trained model
-model = load_model(tag="latest", model_type="44khz")
-model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
-# Encode audio signal
-encoded_out = encode(signal, 'cuda', model)
+# Encode audio signal as one long file
+# (may run out of GPU memory on long files)
+signal.to(model.device)
+
+x = model.preprocess(signal.audio_data, signal.sample_rate)
+z, codes, latents, _, _ = model.encode(x)
 
 # Decode audio signal
-recon = decode(encoded_out, 'cuda', model, preserve_sample_rate=True)
+y = model.decode(z)
+
+# Alternatively, use the `compress` and `decompress` functions
+# to compress long files.
+
+signal = signal.cpu()
+x = model.compress(signal)
+
+# Save and load to and from disk
+x.save("compressed.dac")
+x = dac.DACFile.load("compressed.dac")
+
+# Decompress it back to an AudioSignal
+y = model.decompress(x)
 
 # Write to file
-recon.write('recon.wav')
+y.write('output.wav')
 ```
 
 ### Docker image
 We provide a dockerfile to build a docker image with all the necessary
 dependencies.
 1. Building the image.
     ```
@@ -148,14 +157,36 @@
 
 ### Pre-requisites
 Please install the correct dependencies
 ```
 pip install -e ".[dev]"
 ```
 
+## Environment setup
+
+We have provided a Dockerfile and docker compose setup that makes running experiments easy.
+
+To build the docker image do:
+
+```
+docker compose build
+```
+
+Then, to launch a container, do:
+
+```
+docker compose run -p 8888:8888 -p 6006:6006 dev
+```
+
+The port arguments (`-p`) are optional, but useful if you want to launch a Jupyter and Tensorboard instances within the container. The
+default password for Jupyter is `password`, and the current directory
+is mounted to `/u/home/src`, which also becomes the working directory.
+
+Then, run your training command.
+
 
 ### Single GPU training
 ```
 export CUDA_VISIBLE_DEVICES=0
 python scripts/train.py --args.load conf/ablations/baseline.yml --save_path runs/baseline/
 ```
```

### Comparing `descript-audio-codec-0.0.5/README.md` & `descript-audio-codec-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -62,41 +62,50 @@
 It will also preserve the directory structure relative to input root and
 re-create it in the output directory. Please use `python -m dac decode --help`
 for more options.
 
 ### Programmatic Usage
 ```py
 import dac
-from dac.utils import load_model
-from dac.model import DAC
-
-from dac.utils.encode import process as encode
-from dac.utils.decode import process as decode
-
 from audiotools import AudioSignal
 
-# Init an empty model
-model = DAC()
+# Download a model
+model_path = dac.utils.download(model_type="44khz")
+model = dac.DAC.load(model_path)
 
-# Load compatible pre-trained model
-model = load_model(tag="latest", model_type="44khz")
-model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
-# Encode audio signal
-encoded_out = encode(signal, 'cuda', model)
+# Encode audio signal as one long file
+# (may run out of GPU memory on long files)
+signal.to(model.device)
+
+x = model.preprocess(signal.audio_data, signal.sample_rate)
+z, codes, latents, _, _ = model.encode(x)
 
 # Decode audio signal
-recon = decode(encoded_out, 'cuda', model, preserve_sample_rate=True)
+y = model.decode(z)
+
+# Alternatively, use the `compress` and `decompress` functions
+# to compress long files.
+
+signal = signal.cpu()
+x = model.compress(signal)
+
+# Save and load to and from disk
+x.save("compressed.dac")
+x = dac.DACFile.load("compressed.dac")
+
+# Decompress it back to an AudioSignal
+y = model.decompress(x)
 
 # Write to file
-recon.write('recon.wav')
+y.write('output.wav')
 ```
 
 ### Docker image
 We provide a dockerfile to build a docker image with all the necessary
 dependencies.
 1. Building the image.
     ```
@@ -127,14 +136,36 @@
 
 ### Pre-requisites
 Please install the correct dependencies
 ```
 pip install -e ".[dev]"
 ```
 
+## Environment setup
+
+We have provided a Dockerfile and docker compose setup that makes running experiments easy.
+
+To build the docker image do:
+
+```
+docker compose build
+```
+
+Then, to launch a container, do:
+
+```
+docker compose run -p 8888:8888 -p 6006:6006 dev
+```
+
+The port arguments (`-p`) are optional, but useful if you want to launch a Jupyter and Tensorboard instances within the container. The
+default password for Jupyter is `password`, and the current directory
+is mounted to `/u/home/src`, which also becomes the working directory.
+
+Then, run your training command.
+
 
 ### Single GPU training
 ```
 export CUDA_VISIBLE_DEVICES=0
 python scripts/train.py --args.load conf/ablations/baseline.yml --save_path runs/baseline/
 ```
```

### Comparing `descript-audio-codec-0.0.5/dac/__main__.py` & `descript-audio-codec-1.0.0/dac/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 import argbind
 
-from dac.utils import ensure_default_model as download
+from dac.utils import download
 from dac.utils.decode import decode
 from dac.utils.encode import encode
 
 STAGES = ["encode", "decode", "download"]
 
 
 def run(stage: str):
```

### Comparing `descript-audio-codec-0.0.5/dac/compare/encodec.py` & `descript-audio-codec-1.0.0/dac/compare/encodec.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/dac/model/dac.py` & `descript-audio-codec-1.0.0/dac/model/dac.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,19 @@
             Snake1d(dim),
             WNConv1d(dim, dim, kernel_size=7, dilation=dilation, padding=pad),
             Snake1d(dim),
             WNConv1d(dim, dim, kernel_size=1),
         )
 
     def forward(self, x):
-        return x + self.block(x)
+        y = self.block(x)
+        pad = (x.shape[-1] - y.shape[-1]) // 2
+        if pad > 0:
+            x = x[..., pad:-pad]
+        return x + y
 
 
 class EncoderBlock(nn.Module):
     def __init__(self, dim: int = 16, stride: int = 1):
         super().__init__()
         self.block = nn.Sequential(
             ResidualUnit(dim // 2, dilation=1),
@@ -58,28 +62,29 @@
 
 
 class Encoder(nn.Module):
     def __init__(
         self,
         d_model: int = 64,
         strides: list = [2, 4, 8, 8],
+        d_latent: int = 64,
     ):
         super().__init__()
         # Create first convolution
         self.block = [WNConv1d(1, d_model, kernel_size=7, padding=3)]
 
         # Create EncoderBlocks that double channels as they downsample by `stride`
         for stride in strides:
             d_model *= 2
             self.block += [EncoderBlock(d_model, stride=stride)]
 
         # Create last convolution
         self.block += [
             Snake1d(d_model),
-            WNConv1d(d_model, d_model, kernel_size=3, padding=1),
+            WNConv1d(d_model, d_latent, kernel_size=3, padding=1),
         ]
 
         # Wrap black into nn.Sequential
         self.block = nn.Sequential(*self.block)
         self.enc_dim = d_model
 
     def forward(self, x):
@@ -140,14 +145,15 @@
 
 
 class DAC(BaseModel, CodecMixin):
     def __init__(
         self,
         encoder_dim: int = 64,
         encoder_rates: List[int] = [2, 4, 8, 8],
+        latent_dim: int = None,
         decoder_dim: int = 1536,
         decoder_rates: List[int] = [8, 8, 4, 2],
         n_codebooks: int = 9,
         codebook_size: int = 1024,
         codebook_dim: Union[int, list] = 8,
         quantizer_dropout: bool = False,
         sample_rate: int = 44100,
@@ -156,62 +162,65 @@
 
         self.encoder_dim = encoder_dim
         self.encoder_rates = encoder_rates
         self.decoder_dim = decoder_dim
         self.decoder_rates = decoder_rates
         self.sample_rate = sample_rate
 
-        self.hop_length = np.prod(decoder_rates)
-        self.encoder = Encoder(encoder_dim, encoder_rates)
+        if latent_dim is None:
+            latent_dim = encoder_dim * (2 ** len(encoder_rates))
+
+        self.latent_dim = latent_dim
+
+        self.hop_length = np.prod(encoder_rates)
+        self.encoder = Encoder(encoder_dim, encoder_rates, latent_dim)
 
         self.n_codebooks = n_codebooks
         self.codebook_size = codebook_size
         self.codebook_dim = codebook_dim
-
         self.quantizer = ResidualVectorQuantize(
-            self.encoder.enc_dim,
+            input_dim=latent_dim,
             n_codebooks=n_codebooks,
             codebook_size=codebook_size,
             codebook_dim=codebook_dim,
             quantizer_dropout=quantizer_dropout,
         )
 
         self.decoder = Decoder(
-            self.encoder.enc_dim,
+            latent_dim,
             decoder_dim,
             decoder_rates,
         )
         self.sample_rate = sample_rate
         self.apply(init_weights)
 
+        self.delay = self.get_delay()
+
     def preprocess(self, audio_data, sample_rate):
         if sample_rate is None:
             sample_rate = self.sample_rate
         assert sample_rate == self.sample_rate
 
         length = audio_data.shape[-1]
         right_pad = math.ceil(length / self.hop_length) * self.hop_length - length
         audio_data = nn.functional.pad(audio_data, (0, right_pad))
-        return audio_data, length
+
+        return audio_data
 
     def encode(
         self,
         audio_data: torch.Tensor,
-        sample_rate: int = None,
         n_quantizers: int = None,
     ):
         """Encode given audio data and return quantized latent codes
 
         Parameters
         ----------
         audio_data : Tensor[B x 1 x T]
             Audio data to encode
-        sample_rate : int, optional
-            Sample rate of audio data in Hz, by default None
-            If None, defaults to `self.sample_rate`
         n_quantizers : int, optional
             Number of quantizers to use, by default None
             If None, all quantizers are used.
 
         Returns
         -------
         dict
@@ -227,23 +236,21 @@
                 Commitment loss to train encoder to predict vectors closer to codebook
                 entries
             "vq/codebook_loss" : Tensor[1]
                 Codebook loss to update the codebook
             "length" : int
                 Number of samples in input audio
         """
-        out = {}
-        audio_data, length = self.preprocess(audio_data, sample_rate)
-        out["length"] = length
-
-        out["z"] = self.encoder(audio_data)
-        out.update(self.quantizer(out["z"], n_quantizers))
-        return out
+        z = self.encoder(audio_data)
+        z, codes, latents, commitment_loss, codebook_loss = self.quantizer(
+            z, n_quantizers
+        )
+        return z, codes, latents, commitment_loss, codebook_loss
 
-    def decode(self, z: torch.Tensor, length: int = None):
+    def decode(self, z: torch.Tensor):
         """Decode given latent codes and return audio data
 
         Parameters
         ----------
         z : Tensor[B x D x T]
             Quantized continuous representation of input
         length : int, optional
@@ -252,18 +259,15 @@
         Returns
         -------
         dict
             A dictionary with the following keys:
             "audio" : Tensor[B x 1 x length]
                 Decoded audio data.
         """
-        out = {}
-        x = self.decoder(z)
-        out["audio"] = x[..., :length]
-        return out
+        return self.decoder(z)
 
     def forward(
         self,
         audio_data: torch.Tensor,
         sample_rate: int = None,
         n_quantizers: int = None,
     ):
@@ -297,25 +301,36 @@
             "vq/codebook_loss" : Tensor[1]
                 Codebook loss to update the codebook
             "length" : int
                 Number of samples in input audio
             "audio" : Tensor[B x 1 x length]
                 Decoded audio data.
         """
-        out = {}
-        out.update(self.encode(audio_data, sample_rate, n_quantizers))
-        out.update(self.decode(out["z"], out["length"]))
-        return out
+        length = audio_data.shape[-1]
+        audio_data = self.preprocess(audio_data, sample_rate)
+        z, codes, latents, commitment_loss, codebook_loss = self.encode(
+            audio_data, n_quantizers
+        )
+
+        x = self.decode(z)
+        return {
+            "audio": x[..., :length],
+            "z": z,
+            "codes": codes,
+            "latents": latents,
+            "vq/commitment_loss": commitment_loss,
+            "vq/codebook_loss": codebook_loss,
+        }
 
 
 if __name__ == "__main__":
     import numpy as np
     from functools import partial
 
-    model = DAC()
+    model = DAC().to("cpu")
 
     for n, m in model.named_modules():
         o = m.extra_repr()
         p = sum([np.prod(p.size()) for p in m.parameters()])
         fn = lambda o, p: o + f" {p/1e6:<.3f}M params."
         setattr(m, "extra_repr", partial(fn, o=o, p=p))
     print(model)
@@ -324,21 +339,26 @@
     length = 88200 * 2
     x = torch.randn(1, 1, length).to(model.device)
     x.requires_grad_(True)
     x.retain_grad()
 
     # Make a forward pass
     out = model(x)["audio"]
+    print("Input shape:", x.shape)
+    print("Output shape:", out.shape)
 
     # Create gradient variable
     grad = torch.zeros_like(out)
     grad[:, :, grad.shape[-1] // 2] = 1
 
     # Make a backward pass
     out.backward(grad)
 
     # Check non-zero values
     gradmap = x.grad.squeeze(0)
     gradmap = (gradmap != 0).sum(0)  # sum across features
     rf = (gradmap != 0).sum()
 
     print(f"Receptive field: {rf.item()}")
+
+    x = AudioSignal(torch.randn(1, 1, 44100 * 60), 44100)
+    model.decompress(model.compress(x, verbose=True), verbose=True)
```

### Comparing `descript-audio-codec-0.0.5/dac/model/discriminator.py` & `descript-audio-codec-1.0.0/dac/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/dac/nn/layers.py` & `descript-audio-codec-1.0.0/dac/nn/layers.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/dac/nn/loss.py` & `descript-audio-codec-1.0.0/dac/nn/loss.py`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/dac/nn/quantize.py` & `descript-audio-codec-1.0.0/dac/nn/quantize.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,18 @@
             # Sum losses
             commitment_loss += (commitment_loss_i * mask).mean()
             codebook_loss += (codebook_loss_i * mask).mean()
 
             codebook_indices.append(indices_i)
             latents.append(z_e_i)
 
-        return {
-            "z": z_q,
-            "codes": torch.stack(codebook_indices, dim=1),
-            "latents": torch.cat(latents, dim=1),
-            "vq/commitment_loss": commitment_loss,
-            "vq/codebook_loss": codebook_loss,
-        }
+        codes = torch.stack(codebook_indices, dim=1)
+        latents = torch.cat(latents, dim=1)
+
+        return z_q, codes, latents, commitment_loss, codebook_loss
 
     def from_codes(self, codes: torch.Tensor):
         """Given the quantized codes, reconstruct the continuous representation
         Parameters
         ----------
         codes : Tensor[B x N x T]
             Quantized discrete representation of input
```

### Comparing `descript-audio-codec-0.0.5/dac/utils/__init__.py` & `descript-audio-codec-1.0.0/dac/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,46 +5,60 @@
 
 import dac
 
 DAC = dac.model.DAC
 Accelerator = ml.Accelerator
 
 __MODEL_LATEST_TAGS__ = {
-    "44khz": "0.0.1",
-    "24khz": "0.0.4",
-    "16khz": "0.0.5",
+    ("44khz", "8kbps"): "0.0.1",
+    ("24khz", "8kbps"): "0.0.4",
+    ("16khz", "8kbps"): "0.0.5",
+    ("44khz", "16kbps"): "1.0.0",
 }
 
 __MODEL_URLS__ = {
     (
         "44khz",
         "0.0.1",
+        "8kbps",
     ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.1/weights.pth",
     (
         "24khz",
         "0.0.4",
+        "8kbps",
     ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.4/weights_24khz.pth",
     (
         "16khz",
         "0.0.5",
+        "8kbps",
     ): "https://github.com/descriptinc/descript-audio-codec/releases/download/0.0.5/weights_16khz.pth",
+    (
+        "44khz",
+        "1.0.0",
+        "16kbps",
+    ): "https://github.com/descriptinc/descript-audio-codec/releases/download/1.0.0/weights_44khz_16kbps.pth",
 }
 
 
 @argbind.bind(group="download", positional=True, without_prefix=True)
-def ensure_default_model(tag: str = "latest", model_type: str = "44khz"):
+def download(
+    model_type: str = "44khz", model_bitrate: str = "8kbps", tag: str = "latest"
+):
     """
     Function that downloads the weights file from URL if a local cache is not found.
 
     Parameters
     ----------
-    tag : str
-        The tag of the model to download. Defaults to "latest".
     model_type : str
         The type of model to download. Must be one of "44khz", "24khz", or "16khz". Defaults to "44khz".
+    model_bitrate: str
+        Bitrate of the model. Must be one of "8kbps", or "16kbps". Defaults to "8kbps".
+        Only 44khz model supports 16kbps.
+    tag : str
+        The tag of the model to download. Defaults to "latest".
 
     Returns
     -------
     Path
         Directory path required to load model via audiotools.
     """
     model_type = model_type.lower()
@@ -52,26 +66,35 @@
 
     assert model_type in [
         "44khz",
         "24khz",
         "16khz",
     ], "model_type must be one of '44khz', '24khz', or '16khz'"
 
+    assert model_bitrate in [
+        "8kbps",
+        "16kbps",
+    ], "model_bitrate must be one of '8kbps', or '16kbps'"
+
     if tag == "latest":
-        tag = __MODEL_LATEST_TAGS__[model_type]
+        tag = __MODEL_LATEST_TAGS__[(model_type, model_bitrate)]
 
-    download_link = __MODEL_URLS__.get((model_type, tag), None)
+    download_link = __MODEL_URLS__.get((model_type, tag, model_bitrate), None)
 
     if download_link is None:
         raise ValueError(
             f"Could not find model with tag {tag} and model type {model_type}"
         )
 
     local_path = (
-        Path.home() / ".cache" / "descript" / model_type / tag / "dac" / f"weights.pth"
+        Path.home()
+        / ".cache"
+        / "descript"
+        / "dac"
+        / f"weights_{model_type}_{model_bitrate}_{tag}.pth"
     )
     if not local_path.exists():
         local_path.parent.mkdir(parents=True, exist_ok=True)
 
         # Download the model
         import requests
 
@@ -79,26 +102,22 @@
 
         if response.status_code != 200:
             raise ValueError(
                 f"Could not download model. Received response code {response.status_code}"
             )
         local_path.write_bytes(response.content)
 
-    # return the path required by audiotools to load the model
-    return local_path.parent.parent
+    return local_path
 
 
 def load_model(
-    tag: str = "latest",
-    load_path: str = "",
     model_type: str = "44khz",
+    model_bitrate: str = "8kbps",
+    tag: str = "latest",
+    load_path: str = None,
 ):
     if not load_path:
-        load_path = ensure_default_model(tag, model_type)
-    kwargs = {
-        "folder": load_path,
-        "map_location": "cpu",
-        "package": False,
-    }
-    print(f"Loading weights from {kwargs['folder']}")
-    generator, _ = DAC.load_from_folder(**kwargs)
+        load_path = download(
+            model_type=model_type, model_bitrate=model_bitrate, tag=tag
+        )
+    generator = DAC.load(load_path)
     return generator
```

### Comparing `descript-audio-codec-0.0.5/descript_audio_codec.egg-info/PKG-INFO` & `descript-audio-codec-1.0.0/descript_audio_codec.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descript-audio-codec
-Version: 0.0.5
+Version: 1.0.0
 Summary: A high-quality general neural audio codec.
 Home-page: https://github.com/descriptinc/descript-audio-codec
 Author: Prem Seetharaman, Rithesh Kumar
 Author-email: prem@descript.com
 License: MIT
 Keywords: audio,compression,machine learning
 Classifier: Intended Audience :: Developers
@@ -83,41 +83,50 @@
 It will also preserve the directory structure relative to input root and
 re-create it in the output directory. Please use `python -m dac decode --help`
 for more options.
 
 ### Programmatic Usage
 ```py
 import dac
-from dac.utils import load_model
-from dac.model import DAC
-
-from dac.utils.encode import process as encode
-from dac.utils.decode import process as decode
-
 from audiotools import AudioSignal
 
-# Init an empty model
-model = DAC()
+# Download a model
+model_path = dac.utils.download(model_type="44khz")
+model = dac.DAC.load(model_path)
 
-# Load compatible pre-trained model
-model = load_model(tag="latest", model_type="44khz")
-model.eval()
 model.to('cuda')
 
 # Load audio signal file
 signal = AudioSignal('input.wav')
 
-# Encode audio signal
-encoded_out = encode(signal, 'cuda', model)
+# Encode audio signal as one long file
+# (may run out of GPU memory on long files)
+signal.to(model.device)
+
+x = model.preprocess(signal.audio_data, signal.sample_rate)
+z, codes, latents, _, _ = model.encode(x)
 
 # Decode audio signal
-recon = decode(encoded_out, 'cuda', model, preserve_sample_rate=True)
+y = model.decode(z)
+
+# Alternatively, use the `compress` and `decompress` functions
+# to compress long files.
+
+signal = signal.cpu()
+x = model.compress(signal)
+
+# Save and load to and from disk
+x.save("compressed.dac")
+x = dac.DACFile.load("compressed.dac")
+
+# Decompress it back to an AudioSignal
+y = model.decompress(x)
 
 # Write to file
-recon.write('recon.wav')
+y.write('output.wav')
 ```
 
 ### Docker image
 We provide a dockerfile to build a docker image with all the necessary
 dependencies.
 1. Building the image.
     ```
@@ -148,14 +157,36 @@
 
 ### Pre-requisites
 Please install the correct dependencies
 ```
 pip install -e ".[dev]"
 ```
 
+## Environment setup
+
+We have provided a Dockerfile and docker compose setup that makes running experiments easy.
+
+To build the docker image do:
+
+```
+docker compose build
+```
+
+Then, to launch a container, do:
+
+```
+docker compose run -p 8888:8888 -p 6006:6006 dev
+```
+
+The port arguments (`-p`) are optional, but useful if you want to launch a Jupyter and Tensorboard instances within the container. The
+default password for Jupyter is `password`, and the current directory
+is mounted to `/u/home/src`, which also becomes the working directory.
+
+Then, run your training command.
+
 
 ### Single GPU training
 ```
 export CUDA_VISIBLE_DEVICES=0
 python scripts/train.py --args.load conf/ablations/baseline.yml --save_path runs/baseline/
 ```
```

### Comparing `descript-audio-codec-0.0.5/descript_audio_codec.egg-info/SOURCES.txt` & `descript-audio-codec-1.0.0/descript_audio_codec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `descript-audio-codec-0.0.5/setup.py` & `descript-audio-codec-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="descript-audio-codec",
-    version="0.0.5",
+    version="1.0.0",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Topic :: Artistic Software",
         "Topic :: Multimedia",
         "Topic :: Multimedia :: Sound/Audio",
@@ -24,15 +24,15 @@
     author_email="prem@descript.com",
     url="https://github.com/descriptinc/descript-audio-codec",
     license="MIT",
     packages=find_packages(),
     keywords=["audio", "compression", "machine learning"],
     install_requires=[
         "argbind>=0.3.7",
-        "descript-audiotools==0.7.1",
+        "descript-audiotools>=0.7.2",
         "einops",
         "numpy",
         "torch",
         "torchaudio",
         "tqdm",
     ],
     extras_require={
```

### Comparing `descript-audio-codec-0.0.5/tests/test_cli.py` & `descript-audio-codec-1.0.0/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     # Test decoding
     input_dir = output_dir
     output_dir = input_dir.parent / model_type / "decoded_output"
     args = {
         "input": str(input_dir),
         "output": str(output_dir),
+        "model_type": model_type,
     }
     with argbind.scope(args):
         run("decode")
 
 
 def test_compression():
     # Test encoding
```

### Comparing `descript-audio-codec-0.0.5/tests/test_train.py` & `descript-audio-codec-1.0.0/tests/test_train.py`

 * *Files identical despite different names*

