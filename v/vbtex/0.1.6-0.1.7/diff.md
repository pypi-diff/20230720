# Comparing `tmp/vbtex-0.1.6.tar.gz` & `tmp/vbtex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.6.tar", max compression
+gzip compressed data, was "vbtex-0.1.7.tar", max compression
```

## Comparing `vbtex-0.1.6.tar` & `vbtex-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.6/README.md
--rw-r--r--   0        0        0      370 2023-07-20 13:34:02.227563 vbtex-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.6/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.6/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.6/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.6/vbtex/choice_option.py
--rw-r--r--   0        0        0     1816 2023-07-20 13:33:55.075019 vbtex-0.1.6/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.6/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.6/vbtex/padded.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.7/README.md
+-rw-r--r--   0        0        0      370 2023-07-20 13:38:56.440648 vbtex-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.7/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.7/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.7/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.7/vbtex/choice_option.py
+-rw-r--r--   0        0        0     1798 2023-07-20 13:38:48.707557 vbtex-0.1.7/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.7/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.7/vbtex/padded.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.7/PKG-INFO
```

### Comparing `vbtex-0.1.6/vbtex/.DS_Store` & `vbtex-0.1.7/vbtex/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.6/vbtex/choice_option.py` & `vbtex-0.1.7/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.6/vbtex/framed.py` & `vbtex-0.1.7/vbtex/framed.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 @click.command(
     help="Renders tex expressions into pdf"
 )
 @click.option(
     '-i',
     '--input_text',
-    type=click.get_text_stream('stdin'),
+    type=click.STRING,
     default=None,
     show_default=True,
     help="It takes std inputs and try to render as pdf"
 )
 @click.option(
     '-s',
     '--size',
```

### Comparing `vbtex-0.1.6/vbtex/padded.py` & `vbtex-0.1.7/vbtex/padded.py`

 * *Files identical despite different names*

