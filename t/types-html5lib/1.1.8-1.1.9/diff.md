# Comparing `tmp/types-html5lib-1.1.8.tar.gz` & `tmp/types-html5lib-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-html5lib-1.1.8.tar", last modified: Mon Jul 11 09:22:24 2022, max compression
+gzip compressed data, was "types-html5lib-1.1.9.tar", last modified: Tue Jul 19 09:30:05 2022, max compression
```

## Comparing `types-html5lib-1.1.8.tar` & `types-html5lib-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-11 09:22:23.000000 types-html5lib-1.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-11 09:22:23.000000 types-html5lib-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.345071 types-html5lib-1.1.8/html5lib-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-11 09:22:23.000000 types-html5lib-1.1.8/html5lib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_ihatexml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_inputstream.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_tokenizer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.345071 types-html5lib-1.1.8/html5lib-stubs/_trie/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_trie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_trie/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_trie/py.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.345071 types-html5lib-1.1.8/html5lib-stubs/filters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/alphabeticalattributes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/inject_meta_charset.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/lint.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/optionaltags.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/sanitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/filters/whitespace.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/html5parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/serializer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/html5lib-stubs/treeadapters/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treeadapters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treeadapters/genshi.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treeadapters/sax.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/html5lib-stubs/treebuilders/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treebuilders/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treebuilders/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treebuilders/dom.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treebuilders/etree.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treebuilders/etree_lxml.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/html5lib-stubs/treewalkers/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/base.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/dom.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/etree.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/etree_lxml.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-11 09:22:11.000000 types-html5lib-1.1.8/html5lib-stubs/treewalkers/genshi.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-07-11 09:22:23.000000 types-html5lib-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 09:22:24.349071 types-html5lib-1.1.8/types_html5lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-07-11 09:22:24.000000 types-html5lib-1.1.8/types_html5lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-07-11 09:22:24.000000 types-html5lib-1.1.8/types_html5lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 09:22:24.000000 types-html5lib-1.1.8/types_html5lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-11 09:22:24.000000 types-html5lib-1.1.8/types_html5lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/html5lib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_ihatexml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_inputstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_tokenizer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/_trie/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_trie/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_trie/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_trie/py.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/alphabeticalattributes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/inject_meta_charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/lint.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/optionaltags.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/sanitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/filters/whitespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/html5parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/treeadapters/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treeadapters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treeadapters/genshi.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treeadapters/sax.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/treebuilders/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treebuilders/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treebuilders/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treebuilders/dom.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treebuilders/etree.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treebuilders/etree_lxml.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/html5lib-stubs/treewalkers/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/dom.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/etree.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/etree_lxml.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-19 09:29:25.000000 types-html5lib-1.1.9/html5lib-stubs/treewalkers/genshi.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 09:30:05.971816 types-html5lib-1.1.9/types_html5lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/types_html5lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/types_html5lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/types_html5lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-19 09:30:05.000000 types-html5lib-1.1.9/types_html5lib.egg-info/top_level.txt
```

### Comparing `types-html5lib-1.1.8/CHANGELOG.md` & `types-html5lib-1.1.9/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.1.9 (2022-07-19)
+
+Third-party stubs: enforce CamelCase for type alias names (#8256)
+
+Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
+
 ## 1.1.8 (2022-07-11)
 
 Remove Python 3.6 branches from typeshed (#8269)
 
 ## 1.1.7 (2022-04-16)
 
 Use `TypeAlias` where possible for type aliases (#7630)
```

### Comparing `types-html5lib-1.1.8/PKG-INFO` & `types-html5lib-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-html5lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: Typing stubs for html5lib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/html5lib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `html5lib` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `html5lib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/html5lib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `edc0ecd8579389cc6bb75b343e1001424009c09b`.
+This package was generated from typeshed commit `e3d4bdc91a792bcef5d8eae2c1abab3d4ba27541`.
```

### Comparing `types-html5lib-1.1.8/html5lib-stubs/_ihatexml.pyi` & `types-html5lib-1.1.9/html5lib-stubs/_ihatexml.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/_inputstream.pyi` & `types-html5lib-1.1.9/html5lib-stubs/_inputstream.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/_tokenizer.pyi` & `types-html5lib-1.1.9/html5lib-stubs/_tokenizer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any
-from typing_extensions import TypeAlias
 
 entitiesTrie: Any
-attributeMap: TypeAlias = dict[Any, Any]
+attributeMap = dict
 
 class HTMLTokenizer:
     stream: Any
     parser: Any
     escapeFlag: bool
     lastFourChars: Any
     state: Any
```

### Comparing `types-html5lib-1.1.8/html5lib-stubs/_utils.pyi` & `types-html5lib-1.1.9/html5lib-stubs/_utils.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/constants.pyi` & `types-html5lib-1.1.9/html5lib-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/filters/sanitizer.pyi` & `types-html5lib-1.1.9/html5lib-stubs/filters/sanitizer.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/html5parser.pyi` & `types-html5lib-1.1.9/html5lib-stubs/html5parser.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/serializer.pyi` & `types-html5lib-1.1.9/html5lib-stubs/serializer.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/treebuilders/base.pyi` & `types-html5lib-1.1.9/html5lib-stubs/treebuilders/base.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/treebuilders/etree_lxml.pyi` & `types-html5lib-1.1.9/html5lib-stubs/treebuilders/etree_lxml.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/treewalkers/base.pyi` & `types-html5lib-1.1.9/html5lib-stubs/treewalkers/base.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/html5lib-stubs/treewalkers/etree_lxml.pyi` & `types-html5lib-1.1.9/html5lib-stubs/treewalkers/etree_lxml.pyi`

 * *Files identical despite different names*

### Comparing `types-html5lib-1.1.8/setup.py` & `types-html5lib-1.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `html5lib` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `html5lib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/html5lib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `edc0ecd8579389cc6bb75b343e1001424009c09b`.
+This package was generated from typeshed commit `e3d4bdc91a792bcef5d8eae2c1abab3d4ba27541`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.8",
+      version="1.1.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/html5lib.md",
```

### Comparing `types-html5lib-1.1.8/types_html5lib.egg-info/PKG-INFO` & `types-html5lib-1.1.9/types_html5lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-html5lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: Typing stubs for html5lib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/html5lib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `html5lib` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `html5lib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/html5lib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `edc0ecd8579389cc6bb75b343e1001424009c09b`.
+This package was generated from typeshed commit `e3d4bdc91a792bcef5d8eae2c1abab3d4ba27541`.
```

### Comparing `types-html5lib-1.1.8/types_html5lib.egg-info/SOURCES.txt` & `types-html5lib-1.1.9/types_html5lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

