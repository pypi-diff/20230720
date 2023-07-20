# Comparing `tmp/torch_grammar-0.3.2.tar.gz` & `tmp/torch_grammar-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_grammar-0.3.2.tar", max compression
+gzip compressed data, was "torch_grammar-0.3.3.tar", max compression
```

## Comparing `torch_grammar-0.3.2.tar` & `torch_grammar-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1890 2023-06-27 14:34:41.788242 torch_grammar-0.3.2/README.md
--rw-r--r--   0        0        0      588 2023-06-28 16:16:07.654313 torch_grammar-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.3.2/torch_grammar/__init__.py
--rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.3.2/torch_grammar/grammar_parser.py
--rw-r--r--   0        0        0     6473 2023-06-28 16:11:27.863024 torch_grammar-0.3.2/torch_grammar/grammar_sampler.py
--rw-r--r--   0        0        0     2626 2023-06-27 14:34:57.299812 torch_grammar-0.3.2/torch_grammar/token_trie.py
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 torch_grammar-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1890 2023-06-27 14:34:41.788242 torch_grammar-0.3.3/README.md
+-rw-r--r--   0        0        0      588 2023-07-20 16:00:42.108401 torch_grammar-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-06-19 15:27:17.327365 torch_grammar-0.3.3/torch_grammar/__init__.py
+-rw-r--r--   0        0        0     9709 2023-06-19 17:39:52.938166 torch_grammar-0.3.3/torch_grammar/grammar_parser.py
+-rw-r--r--   0        0        0     6976 2023-07-20 16:00:25.136683 torch_grammar-0.3.3/torch_grammar/grammar_sampler.py
+-rw-r--r--   0        0        0     2626 2023-06-27 14:34:57.299812 torch_grammar-0.3.3/torch_grammar/token_trie.py
+-rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 torch_grammar-0.3.3/PKG-INFO
```

### Comparing `torch_grammar-0.3.2/README.md` & `torch_grammar-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.3.2/torch_grammar/grammar_parser.py` & `torch_grammar-0.3.3/torch_grammar/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.3.2/torch_grammar/grammar_sampler.py` & `torch_grammar-0.3.3/torch_grammar/grammar_sampler.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,15 +63,17 @@
     def logits_processor(self):
         return LogitsProcessor(self)
 
     def init_stacks(self):
         stack = [self.start_rule + 2]
         return self.advance_stack(tuple(stack))
 
-    @lru_cache(maxsize=8000)
+    # For each stack, resolve rules to find the actual characters that are
+    # accepted by this stack (not the set of sub-rules).
+    @lru_cache(maxsize=32768)
     def advance_stack(self, stack):
         stack = list(stack)
         if len(stack) == 0:
             return [stack]
 
         pos = stack[-1]
 
@@ -131,27 +133,34 @@
 
         for byte in self.token_trie.id2str(token):
             stacks = self.accept(byte, stacks)
             assert stacks != []
 
         return stacks
 
+    # For each sub-rule in the grammar, cache whether each byte is accepted.
     @lru_cache(maxsize=None)
     def pos_char_acceptance(self, pos):
         acceptance = [False] * 256
         num_chars = self.src[pos]
         pos += 1
         for i in range(0, num_chars, 2):
             start = self.src[pos + i]
             end = self.src[pos + i + 1]
             for j in range(start, end + 1):
                 acceptance[j] = True
         return acceptance
 
-    @lru_cache(maxsize=8192)
+    # Probably this should be configurable. If the grammar has an exceedingly
+    # large number of states, the correct setting is a tradeoff between GPU
+    # RAM usage and recomputation time.
+    #
+    # The main variable that pushes usage up here is number of states in the
+    # grammar.
+    @lru_cache(maxsize=32768)
     def token_acceptance_for_stack(self, stack, device):
         st = time.time()
         stack = list(stack)  # needs to come in as a tuple for lru_cache
 
         accepts = [False] * len(self.token_trie)
         accepts[self.eos_token_id] = len(stack) == 0
```

### Comparing `torch_grammar-0.3.2/torch_grammar/token_trie.py` & `torch_grammar-0.3.3/torch_grammar/token_trie.py`

 * *Files identical despite different names*

### Comparing `torch_grammar-0.3.2/PKG-INFO` & `torch_grammar-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-grammar
-Version: 0.3.2
+Version: 0.3.3
 Summary: Restrict LLM generations to a context-free grammar
 License: MIT
 Author: Burke Libbey
 Author-email: burke.libbey@shopify.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

