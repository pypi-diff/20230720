# Comparing `tmp/types-parsimonious-0.9.0.tar.gz` & `tmp/types-parsimonious-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-parsimonious-0.9.0.tar", last modified: Tue Jun 21 06:23:59 2022, max compression
+gzip compressed data, was "types-parsimonious-0.9.1.tar", last modified: Tue Jul 12 15:26:30 2022, max compression
```

## Comparing `types-parsimonious-0.9.0.tar` & `types-parsimonious-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 06:23:59.886509 types-parsimonious-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-21 06:23:59.886509 types-parsimonious-0.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 06:23:59.882509 types-parsimonious-0.9.0/parsimonious-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/parsimonious-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/expressions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/grammar.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-21 06:23:36.000000 types-parsimonious-0.9.0/parsimonious-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 06:23:59.886509 types-parsimonious-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 06:23:59.886509 types-parsimonious-0.9.0/types_parsimonious.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/types_parsimonious.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/types_parsimonious.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/types_parsimonious.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-21 06:23:59.000000 types-parsimonious-0.9.0/types_parsimonious.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:26:30.824729 types-parsimonious-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-07-12 15:26:30.824729 types-parsimonious-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:26:30.824729 types-parsimonious-0.9.1/parsimonious-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/parsimonious-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/expressions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/grammar.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-07-12 15:25:34.000000 types-parsimonious-0.9.1/parsimonious-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-12 15:26:30.824729 types-parsimonious-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 15:26:30.824729 types-parsimonious-0.9.1/types_parsimonious.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/types_parsimonious.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/types_parsimonious.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/types_parsimonious.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-12 15:26:30.000000 types-parsimonious-0.9.1/types_parsimonious.egg-info/top_level.txt
```

### Comparing `types-parsimonious-0.9.0/CHANGELOG.md` & `types-parsimonious-0.9.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.9.1 (2022-07-12)
+
+Import `Match` and `Pattern` from `re`, not `typing` (#8277)
+
 ## 0.9.0 (2022-06-21)
 
 Bump parsimonious to 0.9.* (#8117)
 
 ## 0.8.5 (2022-05-07)
 
 Import generics from standard modules in all third-party stubs (#7791)
```

### Comparing `types-parsimonious-0.9.0/PKG-INFO` & `types-parsimonious-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-parsimonious
-Version: 0.9.0
+Version: 0.9.1
 Summary: Typing stubs for parsimonious
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/parsimonious.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `parsimonious` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `parsimonious`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/parsimonious. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b36c7705a79a07736aa9cf2607b29e789d0b004d`.
+This package was generated from typeshed commit `6348a58b8b950f894c9bd92f5ee55eeb521a0cbf`.
```

### Comparing `types-parsimonious-0.9.0/parsimonious-stubs/exceptions.pyi` & `types-parsimonious-0.9.1/parsimonious-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-parsimonious-0.9.0/parsimonious-stubs/expressions.pyi` & `types-parsimonious-0.9.1/parsimonious-stubs/expressions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections.abc
 from collections.abc import Callable, Mapping
-from typing import Any, Pattern, Union
+from re import Pattern
+from typing import Any, Union
 from typing_extensions import TypeAlias
 
 from parsimonious.exceptions import ParseError
 from parsimonious.grammar import Grammar
 from parsimonious.nodes import Node
 from parsimonious.utils import StrAndRepr
```

### Comparing `types-parsimonious-0.9.0/parsimonious-stubs/grammar.pyi` & `types-parsimonious-0.9.1/parsimonious-stubs/grammar.pyi`

 * *Files identical despite different names*

### Comparing `types-parsimonious-0.9.0/parsimonious-stubs/nodes.pyi` & `types-parsimonious-0.9.1/parsimonious-stubs/nodes.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections.abc import Callable, Iterator, Sequence
-from typing import Any, Match, NoReturn, TypeVar
+from re import Match
+from typing import Any, NoReturn, TypeVar
 
 from parsimonious.exceptions import VisitationError as VisitationError
 from parsimonious.expressions import Expression
 from parsimonious.grammar import Grammar
 
 class Node:
     expr: Expression
```

### Comparing `types-parsimonious-0.9.0/setup.py` & `types-parsimonious-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `parsimonious` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `parsimonious`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/parsimonious. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b36c7705a79a07736aa9cf2607b29e789d0b004d`.
+This package was generated from typeshed commit `6348a58b8b950f894c9bd92f5ee55eeb521a0cbf`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.0",
+      version="0.9.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/parsimonious.md",
```

### Comparing `types-parsimonious-0.9.0/types_parsimonious.egg-info/PKG-INFO` & `types-parsimonious-0.9.1/types_parsimonious.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-parsimonious
-Version: 0.9.0
+Version: 0.9.1
 Summary: Typing stubs for parsimonious
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/parsimonious.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `parsimonious` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `parsimonious`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/parsimonious. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b36c7705a79a07736aa9cf2607b29e789d0b004d`.
+This package was generated from typeshed commit `6348a58b8b950f894c9bd92f5ee55eeb521a0cbf`.
```

