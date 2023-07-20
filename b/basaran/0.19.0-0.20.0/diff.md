# Comparing `tmp/basaran-0.19.0.tar.gz` & `tmp/basaran-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.19.0.tar", last modified: Sat Jun 10 04:46:31 2023, max compression
+gzip compressed data, was "basaran-0.20.0.tar", last modified: Thu Jul 20 10:49:32 2023, max compression
```

## Comparing `basaran-0.19.0.tar` & `basaran-0.20.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 04:44:14.000000 basaran-0.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 04:44:14.000000 basaran-0.19.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-10 04:46:31.040270 basaran-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-10 04:44:14.000000 basaran-0.19.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/templates/default.chat.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-10 04:44:14.000000 basaran-0.19.0/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.036270 basaran-0.19.0/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 04:46:31.000000 basaran-0.19.0/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 04:46:31.040270 basaran-0.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-10 04:44:14.000000 basaran-0.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-10 04:44:14.000000 basaran-0.19.0/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 04:46:31.040270 basaran-0.19.0/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-10 04:44:14.000000 basaran-0.19.0/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-10 04:44:14.000000 basaran-0.19.0/utils/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.426292 basaran-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-20 10:46:44.000000 basaran-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 10:46:44.000000 basaran-0.20.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-20 10:49:32.426292 basaran-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-07-20 10:46:44.000000 basaran-0.20.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.418292 basaran-0.20.0/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.422292 basaran-0.20.0/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.422292 basaran-0.20.0/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/templates/default.chat.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 10:46:44.000000 basaran-0.20.0/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.418292 basaran-0.20.0/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-20 10:49:32.000000 basaran-0.20.0/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-20 10:49:32.000000 basaran-0.20.0/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:49:32.000000 basaran-0.20.0/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 10:49:32.000000 basaran-0.20.0/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 10:49:32.000000 basaran-0.20.0/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:49:32.426292 basaran-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-20 10:46:44.000000 basaran-0.20.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.422292 basaran-0.20.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-20 10:46:44.000000 basaran-0.20.0/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-20 10:46:44.000000 basaran-0.20.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 10:46:44.000000 basaran-0.20.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:49:32.426292 basaran-0.20.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-20 10:46:44.000000 basaran-0.20.0/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 10:46:44.000000 basaran-0.20.0/utils/render.py
```

### Comparing `basaran-0.19.0/LICENSE` & `basaran-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/PKG-INFO` & `basaran-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.19.0
+Version: 0.20.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.19.0/README.md` & `basaran-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/__init__.py` & `basaran-0.20.0/basaran/__init__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/__main__.py` & `basaran-0.20.0/basaran/__main__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/choice.py` & `basaran-0.20.0/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/model.py` & `basaran-0.20.0/basaran/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         min_tokens=0,
         max_tokens=16,
         temperature=1.0,
         top_p=1.0,
         n=1,
         logprobs=0,
         echo=False,
+        **kwargs,
     ):
         """Create a completion stream for the provided prompt."""
         if isinstance(prompt, str):
             input_ids = self.tokenize(prompt)
         elif isinstance(prompt, torch.Tensor) and prompt.dim() == 1:
             input_ids = prompt
         else:
@@ -65,28 +66,35 @@
             samples = self._sample(token, 0, [], []) if logprobs > 0 else {}
             for i in range(n):
                 text = detokenizers[i].decode(token)
                 offset = detokenizers[i].start
                 if echo:
                     yield map_choice(text, i, text_offset=offset, **samples)
 
+        generate_kwargs = {
+            **dict(
+                logprobs=logprobs,
+                min_new_tokens=min_tokens,
+                max_new_tokens=max_tokens,
+                temperature=temperature,
+                top_p=top_p,
+            ),
+            **kwargs,
+        }
+
         # Generate completion tokens.
         for (
             tokens,
             token_logprobs,
             top_tokens,
             top_logprobs,
             status,
         ) in self.generate(
             input_ids[None, :].repeat(n, 1),
-            logprobs=logprobs,
-            min_new_tokens=min_tokens,
-            max_new_tokens=max_tokens,
-            temperature=temperature,
-            top_p=top_p,
+            **generate_kwargs,
         ):
             for i in range(n):
                 # Check and update the finish status of the sequence.
                 if finish_reasons[i]:
                     continue
                 if status[i] == 0:
                     finish_reasons[i] = "stop"
@@ -335,8 +343,8 @@
     except ValueError:
         model = AutoModelForSeq2SeqLM.from_pretrained(name_or_path, **kwargs)
 
     # Check if the model has text generation capabilities.
     if not model.can_generate():
         raise TypeError(f"{name_or_path} is not a text generation model")
 
-    return StreamModel(model, tokenizer)
+    return StreamModel(model.eval(), tokenizer)
```

### Comparing `basaran-0.19.0/basaran/static/playground.css` & `basaran-0.20.0/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/static/playground.js` & `basaran-0.20.0/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/static/presets.json` & `basaran-0.20.0/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/templates/playground.html` & `basaran-0.20.0/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran/tokenizer.py` & `basaran-0.20.0/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/basaran.egg-info/PKG-INFO` & `basaran-0.20.0/basaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.19.0
+Version: 0.20.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.19.0/basaran.egg-info/SOURCES.txt` & `basaran-0.20.0/basaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/setup.py` & `basaran-0.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.19.0"
+VERSION = "0.20.0"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
```

### Comparing `basaran-0.19.0/tests/test_choice.py` & `basaran-0.20.0/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/tests/test_model.py` & `basaran-0.20.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/tests/test_tokenizer.py` & `basaran-0.20.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/utils/download.py` & `basaran-0.20.0/utils/download.py`

 * *Files identical despite different names*

### Comparing `basaran-0.19.0/utils/render.py` & `basaran-0.20.0/utils/render.py`

 * *Files identical despite different names*

