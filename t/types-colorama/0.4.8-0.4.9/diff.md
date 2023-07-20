# Comparing `tmp/types-colorama-0.4.8.tar.gz` & `tmp/types-colorama-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-colorama-0.4.8.tar", last modified: Mon Jan 31 00:57:55 2022, max compression
+gzip compressed data, was "types-colorama-0.4.9.tar", last modified: Wed Mar 16 15:19:20 2022, max compression
```

## Comparing `types-colorama-0.4.8.tar` & `types-colorama-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:55.087494 types-colorama-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-01-31 00:57:54.000000 types-colorama-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-31 00:57:54.000000 types-colorama-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-01-31 00:57:55.087494 types-colorama-0.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:55.087494 types-colorama-0.4.8/colorama-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-31 00:57:54.000000 types-colorama-0.4.8/colorama-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/ansi.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/ansitowin32.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/initialise.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/win32.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-01-31 00:57:40.000000 types-colorama-0.4.8/colorama-stubs/winterm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-31 00:57:55.087494 types-colorama-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-01-31 00:57:54.000000 types-colorama-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-31 00:57:55.087494 types-colorama-0.4.8/types_colorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-01-31 00:57:55.000000 types-colorama-0.4.8/types_colorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-01-31 00:57:55.000000 types-colorama-0.4.8/types_colorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-31 00:57:55.000000 types-colorama-0.4.8/types_colorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-31 00:57:55.000000 types-colorama-0.4.8/types_colorama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:19:20.919103 types-colorama-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-03-16 15:19:20.000000 types-colorama-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-16 15:19:20.000000 types-colorama-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-16 15:19:20.919103 types-colorama-0.4.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:19:20.919103 types-colorama-0.4.9/colorama-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-16 15:19:20.000000 types-colorama-0.4.9/colorama-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/ansi.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/ansitowin32.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/initialise.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/win32.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-03-16 15:18:39.000000 types-colorama-0.4.9/colorama-stubs/winterm.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 15:19:20.919103 types-colorama-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-03-16 15:19:20.000000 types-colorama-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 15:19:20.919103 types-colorama-0.4.9/types_colorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-16 15:19:20.000000 types-colorama-0.4.9/types_colorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-03-16 15:19:20.000000 types-colorama-0.4.9/types_colorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 15:19:20.000000 types-colorama-0.4.9/types_colorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-16 15:19:20.000000 types-colorama-0.4.9/types_colorama.egg-info/top_level.txt
```

### Comparing `types-colorama-0.4.8/PKG-INFO` & `types-colorama-0.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-colorama
-Version: 0.4.8
+Version: 0.4.9
 Summary: Typing stubs for colorama
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/colorama.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `colorama` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `colorama`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/colorama. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `3ab250eec828a15d5649053e3613e16c0369263d`.
```

### Comparing `types-colorama-0.4.8/colorama-stubs/ansi.pyi` & `types-colorama-0.4.9/colorama-stubs/ansi.pyi`

 * *Files identical despite different names*

### Comparing `types-colorama-0.4.8/colorama-stubs/ansitowin32.pyi` & `types-colorama-0.4.9/colorama-stubs/ansitowin32.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from _typeshed import SupportsWrite
-from typing import Any, Callable, Optional, Pattern, Sequence, TextIO, Union
+from typing import Any, Callable, Pattern, Sequence, TextIO, Union
 
 if sys.platform == "win32":
     from .winterm import WinTerm
 
     winterm: WinTerm
 else:
     winterm: None
@@ -15,15 +15,15 @@
     def __enter__(self, *args: object, **kwargs: object) -> TextIO: ...
     def __exit__(self, *args: Any, **kwargs: Any) -> None: ...
     def write(self, text: str) -> None: ...
     def isatty(self) -> bool: ...
     @property
     def closed(self) -> bool: ...
 
-_WinTermCall = Callable[[Optional[int], bool, bool], None]
+_WinTermCall = Callable[[int | None, bool, bool], None]
 _WinTermCallDict = dict[int, Union[tuple[_WinTermCall], tuple[_WinTermCall, int], tuple[_WinTermCall, int, bool]]]
 
 class AnsiToWin32:
     ANSI_CSI_RE: Pattern[str] = ...
     ANSI_OSC_RE: Pattern[str] = ...
     wrapped: TextIO = ...
     autoreset: bool = ...
```

### Comparing `types-colorama-0.4.8/colorama-stubs/initialise.pyi` & `types-colorama-0.4.9/colorama-stubs/initialise.pyi`

 * *Files identical despite different names*

### Comparing `types-colorama-0.4.8/colorama-stubs/win32.pyi` & `types-colorama-0.4.9/colorama-stubs/win32.pyi`

 * *Files identical despite different names*

### Comparing `types-colorama-0.4.8/colorama-stubs/winterm.pyi` & `types-colorama-0.4.9/colorama-stubs/winterm.pyi`

 * *Files identical despite different names*

### Comparing `types-colorama-0.4.8/setup.py` & `types-colorama-0.4.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `colorama` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `colorama`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/colorama. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `3ab250eec828a15d5649053e3613e16c0369263d`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.4.8",
+      version="0.4.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/colorama.md",
```

### Comparing `types-colorama-0.4.8/types_colorama.egg-info/PKG-INFO` & `types-colorama-0.4.9/types_colorama.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-colorama
-Version: 0.4.8
+Version: 0.4.9
 Summary: Typing stubs for colorama
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/colorama.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `colorama` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `colorama`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/colorama. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `b88a6f19cdcf031be8135941b940f839e13064d8`.
+This package was generated from typeshed commit `3ab250eec828a15d5649053e3613e16c0369263d`.
```

