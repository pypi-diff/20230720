# Comparing `tmp/open_interpreter-0.0.234.tar.gz` & `tmp/open_interpreter-0.0.235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.234.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.235.tar", max compression
```

## Comparing `open_interpreter-0.0.234.tar` & `open_interpreter-0.0.235.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.234/LICENSE
--rw-r--r--   0        0        0     5780 2023-07-20 06:15:17.947255 open_interpreter-0.0.234/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.234/interpreter/__init__.py
--rw-r--r--   0        0        0     6250 2023-07-19 17:32:49.664772 open_interpreter-0.0.234/interpreter/exec.py
--rw-r--r--   0        0        0     6864 2023-07-19 18:26:31.864566 open_interpreter-0.0.234/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.234/interpreter/json_utils.py
--rw-r--r--   0        0        0     3329 2023-07-19 07:36:51.682957 open_interpreter-0.0.234/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.234/interpreter/system_message.txt
--rw-r--r--   0        0        0     3512 2023-07-19 07:31:27.646247 open_interpreter-0.0.234/interpreter/view.py
--rw-r--r--   0        0        0      564 2023-07-20 06:28:33.855292 open_interpreter-0.0.234/pyproject.toml
--rw-r--r--   0        0        0     6404 1970-01-01 00:00:00.000000 open_interpreter-0.0.234/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.235/LICENSE
+-rw-r--r--   0        0        0     5758 2023-07-20 09:17:29.372901 open_interpreter-0.0.235/README.md
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.235/interpreter/__init__.py
+-rw-r--r--   0        0        0     6250 2023-07-20 18:39:30.718945 open_interpreter-0.0.235/interpreter/exec.py
+-rw-r--r--   0        0        0     6864 2023-07-19 18:26:31.864566 open_interpreter-0.0.235/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.235/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3329 2023-07-19 07:36:51.682957 open_interpreter-0.0.235/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2399 2023-07-19 15:47:18.035279 open_interpreter-0.0.235/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3512 2023-07-19 07:31:27.646247 open_interpreter-0.0.235/interpreter/view.py
+-rw-r--r--   0        0        0      564 2023-07-20 18:40:14.875408 open_interpreter-0.0.235/pyproject.toml
+-rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 open_interpreter-0.0.235/PKG-INFO
```

### Comparing `open_interpreter-0.0.234/LICENSE` & `open_interpreter-0.0.235/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/README.md` & `open_interpreter-0.0.235/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 ```
 Absolutely. First, let's check if any speech-to-text libraries are installed...
 ```
 
 <br>
 
-![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/misc/banner.png)
+![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
 
 <p align="right">
     <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
 </p>
 
 ## What is this?
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 # Open Interpreter A lightweight, open-source implementation of OpenAI's code
 interpreter. ```python interpreter.chat('Hey, can you add subtitles to
 video.mp4 on my Desktop?') ``` ``` Absolutely. First, let's check if any
 speech-to-text libraries are installed... ```
-![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/
-misc/banner.png)
+![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
        Illustration by Open Interpreter. Inspired by Ruby_Chen's GPT-4 artwork.
 ## What is this?
 > Having access to a junior programmer working at the speed of your fingertips
 ... can make new workflows effortless and efficient, as well as open the
 benefits of programming to new audiences. > > â _OpenAI's Code Interpreter
 Release_
 **Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open
```

### Comparing `open_interpreter-0.0.234/interpreter/exec.py` & `open_interpreter-0.0.235/interpreter/exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     old_stdout = sys.stdout
     old_stderr = sys.stderr
 
     # Create new instance of InteractiveShell
     shell = InteractiveShell.instance()
 
     # Disable automatic stdout/stderr flushing
-    #shell.ast_node_interactivity = "last_expr_or_assign"
+    shell.ast_node_interactivity = "last_expr_or_assign"
     # No wait, this should be none so we can handle printing the last node on our own. Why did we have it set to last_expr_or_assign?
-    shell.ast_node_interactivity = "none"
+    #shell.ast_node_interactivity = "none"
     
     # Store the original traceback handler
     old_showtraceback = shell.showtraceback
 
     # Define a new traceback handler
     def custom_showtraceback(*args, **kwargs):
         etype, value, tb = sys.exc_info()
```

### Comparing `open_interpreter-0.0.234/interpreter/interpreter.py` & `open_interpreter-0.0.235/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/interpreter/json_utils.py` & `open_interpreter-0.0.235/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/interpreter/openai_utils.py` & `open_interpreter-0.0.235/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/interpreter/system_message.txt` & `open_interpreter-0.0.235/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/interpreter/view.py` & `open_interpreter-0.0.235/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.234/pyproject.toml` & `open_interpreter-0.0.235/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.234"
+version = "0.0.235"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.234/PKG-INFO` & `open_interpreter-0.0.235/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.234
+Version: 0.0.235
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,15 +25,15 @@
 ```
 ```
 Absolutely. First, let's check if any speech-to-text libraries are installed...
 ```
 
 <br>
 
-![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/misc/banner.png)
+![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
 
 <p align="right">
     <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
 </p>
 
 ## What is this?
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.234 Summary: Ask GPT-
+Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.235 Summary: Ask GPT-
 4 to run code locally. Author: Killian Lucas Author-email:
 killian@drinkwater.ai Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: astor
 (>=0.8.1,<0.9.0) Requires-Dist: git-python (>=1.0.3,<2.0.0) Requires-Dist:
 ipython (>=8.14.0,<9.0.0) Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-
 Dist: rich (>=13.4.2,<14.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown # Open Interpreter A lightweight, open-
 source implementation of OpenAI's code interpreter. ```python interpreter.chat
 ('Hey, can you add subtitles to video.mp4 on my Desktop?') ``` ``` Absolutely.
 First, let's check if any speech-to-text libraries are installed... ```
-![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/
-misc/banner.png)
+![Banner Image](https://i.ibb.co/ZHfB9sm/open-interpreter-banner.png)
        Illustration by Open Interpreter. Inspired by Ruby_Chen's GPT-4 artwork.
 ## What is this?
 > Having access to a junior programmer working at the speed of your fingertips
 ... can make new workflows effortless and efficient, as well as open the
 benefits of programming to new audiences. > > â _OpenAI's Code Interpreter
 Release_
 **Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open
```

