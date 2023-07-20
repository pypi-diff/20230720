# Comparing `tmp/open_interpreter-0.0.235.tar.gz` & `tmp/open_interpreter-0.0.236.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.235.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.236.tar", max compression
```

## Comparing `open_interpreter-0.0.235.tar` & `open_interpreter-0.0.236.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.235/LICENSE
--rw-r--r--   0        0        0     5758 2023-07-20 09:17:29.372901 open_interpreter-0.0.235/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.235/interpreter/__init__.py
--rw-r--r--   0        0        0     6250 2023-07-20 18:39:30.718945 open_interpreter-0.0.235/interpreter/exec.py
--rw-r--r--   0        0        0     6864 2023-07-19 18:26:31.864566 open_interpreter-0.0.235/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.235/interpreter/json_utils.py
--rw-r--r--   0        0        0     3329 2023-07-19 07:36:51.682957 open_interpreter-0.0.235/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.235/interpreter/system_message.txt
--rw-r--r--   0        0        0     3512 2023-07-19 07:31:27.646247 open_interpreter-0.0.235/interpreter/view.py
--rw-r--r--   0        0        0      564 2023-07-20 18:40:14.875408 open_interpreter-0.0.235/pyproject.toml
--rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 open_interpreter-0.0.235/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.236/LICENSE
+-rw-r--r--   0        0        0     5758 2023-07-20 09:17:29.372901 open_interpreter-0.0.236/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.236/interpreter/__init__.py
+-rw-r--r--   0        0        0     6428 2023-07-20 19:07:00.625777 open_interpreter-0.0.236/interpreter/exec.py
+-rw-r--r--   0        0        0     6864 2023-07-20 19:07:26.540398 open_interpreter-0.0.236/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.236/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3329 2023-07-19 07:36:51.682957 open_interpreter-0.0.236/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.236/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3512 2023-07-19 07:31:27.646247 open_interpreter-0.0.236/interpreter/view.py
+-rw-r--r--   0        0        0      564 2023-07-20 19:09:42.022099 open_interpreter-0.0.236/pyproject.toml
+-rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 open_interpreter-0.0.236/PKG-INFO
```

### Comparing `open_interpreter-0.0.235/LICENSE` & `open_interpreter-0.0.236/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/README.md` & `open_interpreter-0.0.236/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/interpreter/exec.py` & `open_interpreter-0.0.236/interpreter/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     old_stdout = sys.stdout
     old_stderr = sys.stderr
 
     # Create new instance of InteractiveShell
     shell = InteractiveShell.instance()
 
     # Disable automatic stdout/stderr flushing
-    shell.ast_node_interactivity = "last_expr_or_assign"
+    #shell.ast_node_interactivity = "last_expr_or_assign"
     # No wait, this should be none so we can handle printing the last node on our own. Why did we have it set to last_expr_or_assign?
-    #shell.ast_node_interactivity = "none"
+    shell.ast_node_interactivity = "none"
     
     # Store the original traceback handler
     old_showtraceback = shell.showtraceback
 
     # Define a new traceback handler
     def custom_showtraceback(*args, **kwargs):
         etype, value, tb = sys.exc_info()
@@ -107,19 +107,24 @@
         try:
             check_for_syntax_errors(code)
         except SyntaxError:
             # Do the same thing you do in custom_showtraceback
             etype, value, tb = sys.exc_info()
             traceback_str = ''.join(itb.structured_traceback(etype, value, tb))
             rich_stdout.write(traceback_str)
+
+            live.refresh() # Sometimes this can happen so quickly, it doesn't auto refresh in time
+
             return rich_stdout.data.strip()
 
         # If syntax is correct, execute the code
         with redirect_stdout(rich_stdout), redirect_stderr(rich_stdout), live:
-            exec_result = shell.run_cell(code)
+            shell.run_cell(code)
+
+        live.refresh() # Sometimes this can happen so quickly, it doesn't auto refresh in time
 
         return rich_stdout.data.strip()
     finally:
         # Restore stdout and stderr
         sys.stdout = old_stdout
         sys.stderr = old_stderr
 
@@ -147,15 +152,15 @@
 
     # Create the new version of the code without magic commands
     code_without_magic = '\n'.join(code_lines_without_magic)
 
     # Try to parse the code without magic commands as an AST
     try:
         tree = ast.parse(code_without_magic)
-    except SyntaxError as e:
+    except SyntaxError:
         return code
 
     # A single pip command would do this
     if len(tree.body) == 0:
         return code
 
     # Replace last statement with print if needed
```

### Comparing `open_interpreter-0.0.235/interpreter/interpreter.py` & `open_interpreter-0.0.236/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/interpreter/json_utils.py` & `open_interpreter-0.0.236/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/interpreter/openai_utils.py` & `open_interpreter-0.0.236/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/interpreter/system_message.txt` & `open_interpreter-0.0.236/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/interpreter/view.py` & `open_interpreter-0.0.236/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.235/pyproject.toml` & `open_interpreter-0.0.236/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.235"
+version = "0.0.236"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.235/PKG-INFO` & `open_interpreter-0.0.236/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.235
+Version: 0.0.236
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.235 Summary: Ask GPT-
+Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.236 Summary: Ask GPT-
 4 to run code locally. Author: Killian Lucas Author-email:
 killian@drinkwater.ai Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: astor
 (>=0.8.1,<0.9.0) Requires-Dist: git-python (>=1.0.3,<2.0.0) Requires-Dist:
 ipython (>=8.14.0,<9.0.0) Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-
 Dist: rich (>=13.4.2,<14.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
```

