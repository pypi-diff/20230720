# Comparing `tmp/docblock-0.0.1a1.tar.gz` & `tmp/docblock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docblock-0.0.1a1.tar", max compression
+gzip compressed data, was "docblock-0.0.2.tar", max compression
```

## Comparing `docblock-0.0.1a1.tar` & `docblock-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-07-20 14:21:49.042286 docblock-0.0.1a1/LICENSE.md
--rw-r--r--   0        0        0     2198 2023-07-20 14:21:49.042286 docblock-0.0.1a1/README.md
--rw-r--r--   0        0        0       78 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/__init__.py
--rw-r--r--   0        0        0      988 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/grammar.py
--rw-r--r--   0        0        0     2110 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/parse.py
--rw-r--r--   0        0        0      779 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/show_versions.py
--rw-r--r--   0        0        0      792 2023-07-20 14:21:49.042286 docblock-0.0.1a1/docblock/utils.py
--rw-r--r--   0        0        0     1827 2023-07-20 14:21:49.042286 docblock-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 docblock-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 15:17:55.835454 docblock-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3012 2023-07-20 15:17:55.835454 docblock-0.0.2/README.md
+-rw-r--r--   0        0        0       78 2023-07-20 15:17:55.835454 docblock-0.0.2/docblock/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-20 15:17:55.835454 docblock-0.0.2/docblock/grammar.py
+-rw-r--r--   0        0        0     2110 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/parse.py
+-rw-r--r--   0        0        0      779 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/show_versions.py
+-rw-r--r--   0        0        0      792 2023-07-20 15:17:55.839454 docblock-0.0.2/docblock/utils.py
+-rw-r--r--   0        0        0     1825 2023-07-20 15:17:55.839454 docblock-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 docblock-0.0.2/PKG-INFO
```

### Comparing `docblock-0.0.1a1/LICENSE.md` & `docblock-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docblock-0.0.1a1/docblock/grammar.py` & `docblock-0.0.2/docblock/grammar.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 ID = pp.Word(pp.identbodychars)
 QUALIFIED_ID = pp.Combine(pp.OneOrMore(pp.Optional(ID + "::") + ID))
 
 LPAR, RPAR = pp.Literal("("), pp.Literal(")")
 LBRACE, RBRACE = pp.Literal("{"), pp.Literal("}")
 CLOSE_STMT = pp.Literal(";")
 
-
 # Namespace, class (struct) and function definitions. These are fairly crude
 # but seem to work well.
 NAMESPACE = pp.Keyword("namespace").suppress() + QUALIFIED_ID
 CLASS = (pp.Keyword("struct") | pp.Keyword("class")).suppress() + QUALIFIED_ID
-FUNC = QUALIFIED_ID + (LPAR + ... + CLOSE_STMT).suppress()
+
+# Exclude braces: we only want the delcarations, not any implementations.
+# Assumes those are separated.
+FUNC = QUALIFIED_ID + (LPAR + ... + RPAR + ID[...] + CLOSE_STMT).suppress()
 
 # Line comment and documentation blocks.
 LINE_COMMENT = pp.dbl_slash_comment
 DOCBLOCK = pp.c_style_comment
 
 # Complete syntax we match on, ignoring (end-of-)line comments.
 _ITEMS = NAMESPACE | CLASS | FUNC | LBRACE | RBRACE | DOCBLOCK
```

### Comparing `docblock-0.0.1a1/docblock/parse.py` & `docblock-0.0.2/docblock/parse.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.1a1/docblock/show_versions.py` & `docblock-0.0.2/docblock/show_versions.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.1a1/docblock/utils.py` & `docblock-0.0.2/docblock/utils.py`

 * *Files identical despite different names*

### Comparing `docblock-0.0.1a1/pyproject.toml` & `docblock-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docblock"
-version = "0.0.1a1"
+version = "0.0.2"
 description = "Reads and parses documentation from header files in pure Python."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/docblock"
 include = [
     "LICENSE.md",
```

