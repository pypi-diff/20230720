# Comparing `tmp/vbtex-0.1.5.tar.gz` & `tmp/vbtex-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.5.tar", max compression
+gzip compressed data, was "vbtex-0.1.6.tar", max compression
```

## Comparing `vbtex-0.1.5.tar` & `vbtex-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.5/README.md
--rw-r--r--   0        0        0      370 2023-07-20 13:25:13.078644 vbtex-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.5/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.5/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.5/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.5/vbtex/choice_option.py
--rw-r--r--   0        0        0     1812 2023-07-20 13:24:27.451139 vbtex-0.1.5/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.5/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.5/vbtex/padded.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.6/README.md
+-rw-r--r--   0        0        0      370 2023-07-20 13:34:02.227563 vbtex-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.6/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.6/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.6/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.6/vbtex/choice_option.py
+-rw-r--r--   0        0        0     1816 2023-07-20 13:33:55.075019 vbtex-0.1.6/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.6/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.6/vbtex/padded.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.6/PKG-INFO
```

### Comparing `vbtex-0.1.5/vbtex/.DS_Store` & `vbtex-0.1.6/vbtex/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.5/vbtex/choice_option.py` & `vbtex-0.1.6/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.5/vbtex/framed.py` & `vbtex-0.1.6/vbtex/framed.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 @click.command(
     help="Renders tex expressions into pdf"
 )
 @click.option(
     '-i',
-    '--inputtext',
+    '--input_text',
     type=click.get_text_stream('stdin'),
     default=None,
     show_default=True,
     help="It takes std inputs and try to render as pdf"
 )
 @click.option(
     '-s',
@@ -24,20 +24,20 @@
     prompt='Format',
     type=click.Choice(['SQUARE', 'VRECT', 'HRECT']),
     cls=ChoiceOption,
     default=1,
     show_default=True,
     help="Format of the output"
 )
-def framed(inputtext, size):
+def framed(input_text, size):
     
-    if inputtext is None:
+    if input_text is None:
         tex = click.edit()
     else:
-        tex = inputtext
+        tex = input_text
 
     click.echo(tex)
     
     os.makedirs(f'./vbtex', exist_ok=True)
     path_main = os.path.join(f'./vbtex', 'main.tex')
```

### Comparing `vbtex-0.1.5/vbtex/padded.py` & `vbtex-0.1.6/vbtex/padded.py`

 * *Files identical despite different names*

