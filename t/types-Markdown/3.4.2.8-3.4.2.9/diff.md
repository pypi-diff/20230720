# Comparing `tmp/types-Markdown-3.4.2.8.tar.gz` & `tmp/types-Markdown-3.4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Markdown-3.4.2.8.tar", last modified: Wed May  3 12:29:47 2023, max compression
+gzip compressed data, was "types-Markdown-3.4.2.9.tar", last modified: Wed May 10 15:20:46 2023, max compression
```

## Comparing `types-Markdown-3.4.2.8.tar` & `types-Markdown-3.4.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.400845 types-Markdown-3.4.2.8/markdown-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/markdown-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/__meta__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/blockparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/blockprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/markdown-stubs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/abbr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/admonition.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/attr_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/codehilite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/def_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/extra.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/fenced_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/footnotes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/legacy_attrs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/legacy_em.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/md_in_html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/meta.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/nl2br.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/sane_lists.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/smarty.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/toc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/extensions/wikilinks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/inlinepatterns.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/postprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/preprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/serializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/treeprocessors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-03 12:29:30.000000 types-Markdown-3.4.2.8/markdown-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-03 12:29:45.000000 types-Markdown-3.4.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:29:47.404845 types-Markdown-3.4.2.8/types_Markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 12:29:47.000000 types-Markdown-3.4.2.8/types_Markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:46.918545 types-Markdown-3.4.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:20:46.918545 types-Markdown-3.4.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:46.914545 types-Markdown-3.4.2.9/markdown-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/markdown-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/__meta__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/blockparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/blockprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:46.914545 types-Markdown-3.4.2.9/markdown-stubs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/abbr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/admonition.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/attr_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/codehilite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/def_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/extra.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/fenced_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/footnotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/legacy_attrs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/legacy_em.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/md_in_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/meta.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/nl2br.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/sane_lists.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/smarty.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/toc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/extensions/wikilinks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/inlinepatterns.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/postprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/preprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/serializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/treeprocessors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-10 15:19:44.000000 types-Markdown-3.4.2.9/markdown-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:46.918545 types-Markdown-3.4.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:46.918545 types-Markdown-3.4.2.9/types_Markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/types_Markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/types_Markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/types_Markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:20:46.000000 types-Markdown-3.4.2.9/types_Markdown.egg-info/top_level.txt
```

### Comparing `types-Markdown-3.4.2.8/CHANGELOG.md` & `types-Markdown-3.4.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.4.2.9 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 3.4.2.8 (2023-05-03)
 
 Add Markdown.ESCAPED_CHARS to Markdown stubs (#10134)
 
 ## 3.4.2.7 (2023-04-04)
 
 Various improvements to `Markdown` stubs (#10008)
```

### Comparing `types-Markdown-3.4.2.8/PKG-INFO` & `types-Markdown-3.4.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Markdown
-Version: 3.4.2.8
+Version: 3.4.2.9
 Summary: Typing stubs for Markdown
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/blockparser.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/blockparser.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/blockprocessors.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/blockprocessors.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/core.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/extensions/__init__.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/extensions/codehilite.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/extensions/codehilite.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/extensions/footnotes.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/extensions/footnotes.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/extensions/smarty.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/extensions/smarty.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/extensions/toc.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/extensions/toc.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/inlinepatterns.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/inlinepatterns.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/treeprocessors.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/treeprocessors.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/markdown-stubs/util.pyi` & `types-Markdown-3.4.2.9/markdown-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-Markdown-3.4.2.8/setup.py` & `types-Markdown-3.4.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.4.2.8",
+      version="3.4.2.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md",
```

### Comparing `types-Markdown-3.4.2.8/types_Markdown.egg-info/PKG-INFO` & `types-Markdown-3.4.2.9/types_Markdown.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Markdown
-Version: 3.4.2.8
+Version: 3.4.2.9
 Summary: Typing stubs for Markdown
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Markdown.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Markdown`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Markdown. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b5ca0b23855b56ecd1d957f48efad6e392691e7`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-Markdown-3.4.2.8/types_Markdown.egg-info/SOURCES.txt` & `types-Markdown-3.4.2.9/types_Markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

