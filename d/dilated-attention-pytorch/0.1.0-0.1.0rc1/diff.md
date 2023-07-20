# Comparing `tmp/dilated-attention-pytorch-0.1.0.tar.gz` & `tmp/dilated-attention-pytorch-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dilated-attention-pytorch-0.1.0.tar", last modified: Thu Jul 20 14:50:29 2023, max compression
+gzip compressed data, was "dilated-attention-pytorch-0.1.0rc1.tar", last modified: Wed Jul 19 02:18:43 2023, max compression
```

## Comparing `dilated-attention-pytorch-0.1.0.tar` & `dilated-attention-pytorch-0.1.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:29.248607 dilated-attention-pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-20 14:50:29.248607 dilated-attention-pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:29.244607 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/dilated_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/long_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:29.248607 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-20 14:50:29.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 14:50:29.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:50:29.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 14:50:29.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 14:50:29.000000 dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 14:50:29.248607 dilated-attention-pytorch-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:50:29.248607 dilated-attention-pytorch-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/tests/test_dilated_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-20 14:50:15.000000 dilated-attention-pytorch-0.1.0/tests/test_long_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/dilated_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/long_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-19 02:18:43.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 02:18:43.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:18:43.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-19 02:18:43.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-19 02:18:43.000000 dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:18:43.367947 dilated-attention-pytorch-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/tests/test_dilated_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-19 02:18:31.000000 dilated-attention-pytorch-0.1.0rc1/tests/test_long_net.py
```

### Comparing `dilated-attention-pytorch-0.1.0/LICENSE` & `dilated-attention-pytorch-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dilated-attention-pytorch-0.1.0/PKG-INFO` & `dilated-attention-pytorch-0.1.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dilated-attention-pytorch
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: project_description
 Home-page: https://github.com/fkodom/dilated-attention-pytorch
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -41,25 +41,14 @@
 # Install all dev dependencies (tests etc.)
 pip install "dilated-attention-pytorch[all] @ git+ssh://git@github.com/fkodom/dilated-attention-pytorch.git"
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
-## Benchmark
-
-I follow the benchmarking procedure from the [LongNet paper](https://arxiv.org/abs/2307.02486) (Section 3.1) as best I can.  They tested in a distributed, multi-GPU setting (and by my estimation, with much better GPUs), and I test on a single GTX 2080 Ti, but the same general scaling trends still apply.  Rather than 1B tokens, I scale the batch size so that the total number of tokens is 32M, which is the largest sequence that fits in memory on my GPU when running dilated attention.
-
-See: [benchmark.py](./benchmark.py)
-
-![benchmark](./doc/benchmark.png)
-
-> **NOTE**: Clearly, there are some inefficiencies in my `DilatedAttention` implementation for shorter sequence lengths.  I'm not sure what's causing this.  If you have any insights, please let me know!
-
-
 ## Usage
 
 ### `DilatedAttention`
 
 The LongNet paper introduces a new attention mechanism called `DilatedAttention`.  It is a drop-in replacement (see below) for "vanilla" attention that allows for much longer sequences to be processed.
 
 > **NOTE**: `DilatedAttention` only supports `batch_first=True`.  This is different from "vanilla" attention in PyTorch, which supports both `batch_first=True` and `batch_first=False`.
```

### Comparing `dilated-attention-pytorch-0.1.0/README.md` & `dilated-attention-pytorch-0.1.0rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,25 +25,14 @@
 # Install all dev dependencies (tests etc.)
 pip install "dilated-attention-pytorch[all] @ git+ssh://git@github.com/fkodom/dilated-attention-pytorch.git"
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
-## Benchmark
-
-I follow the benchmarking procedure from the [LongNet paper](https://arxiv.org/abs/2307.02486) (Section 3.1) as best I can.  They tested in a distributed, multi-GPU setting (and by my estimation, with much better GPUs), and I test on a single GTX 2080 Ti, but the same general scaling trends still apply.  Rather than 1B tokens, I scale the batch size so that the total number of tokens is 32M, which is the largest sequence that fits in memory on my GPU when running dilated attention.
-
-See: [benchmark.py](./benchmark.py)
-
-![benchmark](./doc/benchmark.png)
-
-> **NOTE**: Clearly, there are some inefficiencies in my `DilatedAttention` implementation for shorter sequence lengths.  I'm not sure what's causing this.  If you have any insights, please let me know!
-
-
 ## Usage
 
 ### `DilatedAttention`
 
 The LongNet paper introduces a new attention mechanism called `DilatedAttention`.  It is a drop-in replacement (see below) for "vanilla" attention that allows for much longer sequences to be processed.
 
 > **NOTE**: `DilatedAttention` only supports `batch_first=True`.  This is different from "vanilla" attention in PyTorch, which supports both `batch_first=True` and `batch_first=False`.
```

### Comparing `dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/dilated_attention.py` & `dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/dilated_attention.py`

 * *Files identical despite different names*

### Comparing `dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/long_net.py` & `dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/long_net.py`

 * *Files identical despite different names*

### Comparing `dilated-attention-pytorch-0.1.0/dilated_attention_pytorch/transformer.py` & `dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `dilated-attention-pytorch-0.1.0/dilated_attention_pytorch.egg-info/PKG-INFO` & `dilated-attention-pytorch-0.1.0rc1/dilated_attention_pytorch.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dilated-attention-pytorch
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: project_description
 Home-page: https://github.com/fkodom/dilated-attention-pytorch
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -41,25 +41,14 @@
 # Install all dev dependencies (tests etc.)
 pip install "dilated-attention-pytorch[all] @ git+ssh://git@github.com/fkodom/dilated-attention-pytorch.git"
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
-## Benchmark
-
-I follow the benchmarking procedure from the [LongNet paper](https://arxiv.org/abs/2307.02486) (Section 3.1) as best I can.  They tested in a distributed, multi-GPU setting (and by my estimation, with much better GPUs), and I test on a single GTX 2080 Ti, but the same general scaling trends still apply.  Rather than 1B tokens, I scale the batch size so that the total number of tokens is 32M, which is the largest sequence that fits in memory on my GPU when running dilated attention.
-
-See: [benchmark.py](./benchmark.py)
-
-![benchmark](./doc/benchmark.png)
-
-> **NOTE**: Clearly, there are some inefficiencies in my `DilatedAttention` implementation for shorter sequence lengths.  I'm not sure what's causing this.  If you have any insights, please let me know!
-
-
 ## Usage
 
 ### `DilatedAttention`
 
 The LongNet paper introduces a new attention mechanism called `DilatedAttention`.  It is a drop-in replacement (see below) for "vanilla" attention that allows for much longer sequences to be processed.
 
 > **NOTE**: `DilatedAttention` only supports `batch_first=True`.  This is different from "vanilla" attention in PyTorch, which supports both `batch_first=True` and `batch_first=False`.
```

### Comparing `dilated-attention-pytorch-0.1.0/setup.py` & `dilated-attention-pytorch-0.1.0rc1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,26 +14,15 @@
 
     if version.lower().startswith("fatal"):
         version = "0.0.0"
 
     return version
 
 
-extras_require = {
-    "test": [
-        "black",
-        "flake8",
-        "isort",
-        "kaleido",
-        "mypy",
-        "plotly",
-        "pytest",
-        "pytest-cov",
-    ]
-}
+extras_require = {"test": ["black", "flake8", "isort", "mypy", "pytest", "pytest-cov"]}
 extras_require["dev"] = ["pre-commit", *extras_require["test"]]
 all_require = [r for reqs in extras_require.values() for r in reqs]
 extras_require["all"] = all_require
 
 
 setup(
     name="dilated-attention-pytorch",
```

### Comparing `dilated-attention-pytorch-0.1.0/tests/test_dilated_attention.py` & `dilated-attention-pytorch-0.1.0rc1/tests/test_dilated_attention.py`

 * *Files identical despite different names*

### Comparing `dilated-attention-pytorch-0.1.0/tests/test_long_net.py` & `dilated-attention-pytorch-0.1.0rc1/tests/test_long_net.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
 @pytest.mark.parametrize("d_model", [128])
 @pytest.mark.parametrize("nhead", [4, 8])
 @pytest.mark.parametrize("num_layers", [1, 2])
 @pytest.mark.parametrize("dim_feedforward", [64])
 @pytest.mark.parametrize("dropout", [0.0])
 @pytest.mark.parametrize("activation", ["relu", "gelu"])
-# NOTE: 'is_causal=True' causes issues on CPU
-@pytest.mark.parametrize("is_causal", [False])
+@pytest.mark.parametrize("is_causal", [True, False])
 def test_long_net(
     d_model: int,
     nhead: int,
     num_layers: int,
     dim_feedforward: int,
     segment_lengths: Tuple[int, ...],
     dilation_rates: Tuple[int, ...],
@@ -63,16 +62,15 @@
 @pytest.mark.parametrize("num_tokens", [100])
 @pytest.mark.parametrize("d_model", [128])
 @pytest.mark.parametrize("nhead", [4, 8])
 @pytest.mark.parametrize("num_layers", [1, 2])
 @pytest.mark.parametrize("dim_feedforward", [64])
 @pytest.mark.parametrize("dropout", [0.0])
 @pytest.mark.parametrize("activation", ["relu", "gelu"])
-# NOTE: 'is_causal=True' causes issues on CPU
-@pytest.mark.parametrize("is_causal", [False])
+@pytest.mark.parametrize("is_causal", [True, False])
 def test_long_net_lm(
     num_tokens: int,
     d_model: int,
     nhead: int,
     num_layers: int,
     dim_feedforward: int,
     segment_lengths: Tuple[int, ...],
```

