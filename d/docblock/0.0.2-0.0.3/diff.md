# Comparing `tmp/docblock-0.0.2.tar.gz` & `tmp/docblock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docblock-0.0.2.tar", max compression
+gzip compressed data, was "docblock-0.0.3.tar", max compression
```

## Comparing `docblock-0.0.2.tar` & `docblock-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-20 15:17:55.835454 docblock-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     3012 2023-07-20 15:17:55.835454 docblock-0.0.2/README.md
--rw-r--r--   0        0        0       78 2023-07-20 15:17:55.835454 docblock-0.0.2/docblock/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-20 15:17:55.835454 docblock-0.0.2/docblock/grammar.py
--rw-r--r--   0        0        0     2110 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/parse.py
--rw-r--r--   0        0        0      779 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/show_versions.py
--rw-r--r--   0        0        0      792 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/utils.py
--rw-r--r--   0        0        0     1825 2023-07-20 15:17:55.839454 docblock-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 docblock-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 17:26:25.195425 docblock-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     3041 2023-07-20 17:26:25.195425 docblock-0.0.3/README.md
+-rw-r--r--   0        0        0       78 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/grammar.py
+-rw-r--r--   0        0        0     2110 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/parse.py
+-rw-r--r--   0        0        0      779 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/show_versions.py
+-rw-r--r--   0        0        0      832 2023-07-20 17:26:25.199426 docblock-0.0.3/docblock/utils.py
+-rw-r--r--   0        0        0     1825 2023-07-20 17:26:25.199426 docblock-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 docblock-0.0.3/PKG-INFO
```

### Comparing `docblock-0.0.2/LICENSE.md` & `docblock-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.2/README.md` & `docblock-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```cpp
 /**
  * Text
  */
 void func();
 ```
 That is, the documentation block starts with `/*` or `/**`, and ends with `*/`.
-Any starting `*` on documentation lines in the block are allowed, but not required.
+Any starting `*` on documentation lines in the block are allowed, but not required unless you care about significant whitespace.
 > To avoid parsing issues, non-documentation block comments SHOULD NOT use C-style comments. 
 
 The `docblock` package is a pure Python package and depends only on `pyparsing`.
 It can be installed as
 ```shell
 pip install docblock
 ``` 
@@ -49,26 +49,28 @@
     /**
      * A method.
      */
     void aMethod() const;
 };
 };  // namespace test
 ```
-This file may be parsed as
+This file may be parsed as:
 ```python
 from docblock import parse_file
 
 res = parse_file("test.h")
 ```
-This is pretty-printed as
+Now, `res` contains:
 ```python
 >>> print(res)
-{'test': ['Test namespace.'],
-             'test::Test::Test': ['First constructor', 'Second constructor'],
-             'test::Test::aMethod': ['A method.']}
+{
+    'test': ['Test namespace.'],
+    'test::Test::Test': ['First constructor', 'Second constructor'],
+    'test::Test::aMethod': ['A method.']
+}
 ```
 Observe that `docblock` understands scoping, and returns docstrings using qualified names.
 For overloads, multiple docstrings are returned: one for each documented overload.
 
 ## Why `docblock`?
 
 Parsing documentation from header files is common practice to generate documentation, particularly in mixed-language projects where the C++ components are intended to be used from another language.
```

### Comparing `docblock-0.0.2/docblock/grammar.py` & `docblock-0.0.3/docblock/grammar.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.2/docblock/parse.py` & `docblock-0.0.3/docblock/parse.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.2/docblock/show_versions.py` & `docblock-0.0.3/docblock/show_versions.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.2/docblock/utils.py` & `docblock-0.0.3/docblock/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,11 +25,11 @@
     lines = doc.splitlines()
     lines[0] = lines[0].replace("/**", "").replace("/*", "")
     lines[-1] = lines[-1].replace("*/", "")
 
     def clean(line):
         line = line.strip()
         if line.startswith("*"):
-            line = line[1:]
-        return line.strip()
+            line = line[2:] if line.startswith("* ") else line[1:]
+        return line.rstrip()
 
     return "\n".join(map(clean, lines)).strip()
```

### Comparing `docblock-0.0.2/pyproject.toml` & `docblock-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docblock"
-version = "0.0.2"
+version = "0.0.3"
 description = "Reads and parses documentation from header files in pure Python."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/docblock"
 include = [
     "LICENSE.md",
```

### Comparing `docblock-0.0.2/PKG-INFO` & `docblock-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docblock
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reads and parses documentation from header files in pure Python.
 Home-page: https://github.com/N-Wouda/docblock
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 ```cpp
 /**
  * Text
  */
 void func();
 ```
 That is, the documentation block starts with `/*` or `/**`, and ends with `*/`.
-Any starting `*` on documentation lines in the block are allowed, but not required.
+Any starting `*` on documentation lines in the block are allowed, but not required unless you care about significant whitespace.
 > To avoid parsing issues, non-documentation block comments SHOULD NOT use C-style comments. 
 
 The `docblock` package is a pure Python package and depends only on `pyparsing`.
 It can be installed as
 ```shell
 pip install docblock
 ``` 
@@ -72,26 +72,28 @@
     /**
      * A method.
      */
     void aMethod() const;
 };
 };  // namespace test
 ```
-This file may be parsed as
+This file may be parsed as:
 ```python
 from docblock import parse_file
 
 res = parse_file("test.h")
 ```
-This is pretty-printed as
+Now, `res` contains:
 ```python
 >>> print(res)
-{'test': ['Test namespace.'],
-             'test::Test::Test': ['First constructor', 'Second constructor'],
-             'test::Test::aMethod': ['A method.']}
+{
+    'test': ['Test namespace.'],
+    'test::Test::Test': ['First constructor', 'Second constructor'],
+    'test::Test::aMethod': ['A method.']
+}
 ```
 Observe that `docblock` understands scoping, and returns docstrings using qualified names.
 For overloads, multiple docstrings are returned: one for each documented overload.
 
 ## Why `docblock`?
 
 Parsing documentation from header files is common practice to generate documentation, particularly in mixed-language projects where the C++ components are intended to be used from another language.
```

