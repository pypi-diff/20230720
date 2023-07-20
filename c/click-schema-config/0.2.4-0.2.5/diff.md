# Comparing `tmp/click_schema_config-0.2.4.tar.gz` & `tmp/click_schema_config-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.2.4.tar", max compression
+gzip compressed data, was "click_schema_config-0.2.5.tar", max compression
```

## Comparing `click_schema_config-0.2.4.tar` & `click_schema_config-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.4/LICENSE
--rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/README.md
--rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.4/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2551 2023-07-13 12:37:29.353520 click_schema_config-0.2.4/click_schema_config/click.py
--rw-r--r--   0        0        0     3344 2023-07-12 12:39:05.946883 click_schema_config-0.2.4/click_schema_config/commands/codegen.py
--rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/commands/templates/__init__.py.jinja
--rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/commands/templates/dataclass.py.jinja
--rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.4/click_schema_config/py.typed
--rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/read_config.py
--rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/types.py
--rwxr-xr-x   0        0        0      762 2023-07-19 08:27:48.805517 click_schema_config-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 click_schema_config-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-20 21:06:01.033916 click_schema_config-0.2.5/LICENSE
+-rwxr-xr-x   0        0        0     5255 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-20 21:06:01.041916 click_schema_config-0.2.5/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2436 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/click_schema_config/click.py
+-rw-r--r--   0        0        0     3344 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/click_schema_config/commands/codegen.py
+-rw-r--r--   0        0        0       69 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/click_schema_config/commands/templates/__init__.py.jinja
+-rw-r--r--   0        0        0      768 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/click_schema_config/commands/templates/dataclass.py.jinja
+-rw-r--r--   0        0        0        0 2023-07-20 21:06:01.037916 click_schema_config-0.2.5/click_schema_config/py.typed
+-rwxr-xr-x   0        0        0     3803 2023-07-20 21:06:01.049916 click_schema_config-0.2.5/click_schema_config/read_config.py
+-rw-r--r--   0        0        0      499 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      762 2023-07-20 21:06:01.045916 click_schema_config-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 click_schema_config-0.2.5/PKG-INFO
```

### Comparing `click_schema_config-0.2.4/LICENSE` & `click_schema_config-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.4/README.md` & `click_schema_config-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.4/click_schema_config/click.py` & `click_schema_config-0.2.5/click_schema_config/click.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,43 @@
+from typing import TYPE_CHECKING
+
 __all__ = ["schema_from_inis"]
 
-from typing import Any, Callable, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from _typeshed import IdentityFunction
-from .types import FileLike
+from typing import Any, Callable, Iterable
+from click_schema_config.types import FileLike
 
 import builtins
 
 import click
 from .read_config import read_configs
 
 FC = Callable[..., Any]
 
 
 def schema_from_inis(
-    files: list[FileLike] | FileLike = ["config.default.ini", "config.ini"],
+    filenames: Iterable[FileLike] | FileLike = ["config.default.ini", "config.ini"],
     insecure_eval: bool = False,
-    **kwargs: Any,  # type: ignore[return-value]
+    **kwargs: Any,
 ) -> "IdentityFunction":
     """Decorate a click command to load options from a config file.
 
     Parameters
     ----------
-    filenames : list[FileLike] | FileLike, optional
-        List of files (either open file-pointers or filenames) to load, by default ["config.default.ini", "config.ini"]
-    insecure_eval : bool, optional
+    filenames
+        List of filenames to load, by default ["config.default.ini", "config.ini"]
+    insecure_eval
         Whether or not to allow arbitrary code execution, by default False
-    **kwargs : Any
-        Passed to click.option
+    **kwargs
+        Passed to click.option directly
     """
 
-    if isinstance(files, str):
-        files = [files]
-
-    config = read_configs(files)
+    config = read_configs(filenames)
 
     def decorator(func: FC, /) -> FC:
         # We use reverse-order so that the options are added in the order they appear in the file
         for section in reversed(config.values()):
             for d in reversed(section.values()):
                 type_evalled = d.type
                 if type_evalled is not None:
```

### Comparing `click_schema_config-0.2.4/click_schema_config/commands/codegen.py` & `click_schema_config-0.2.5/click_schema_config/commands/codegen.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.4/click_schema_config/commands/templates/dataclass.py.jinja` & `click_schema_config-0.2.5/click_schema_config/commands/templates/dataclass.py.jinja`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.4/click_schema_config/read_config.py` & `click_schema_config-0.2.5/click_schema_config/read_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 __all__ = ["read_config", "read_configs"]
 
+
+from typing import Iterable
 from .types import Config, FileLike, Variable
 
 from dataclasses import dataclass
 import dataclasses
 
+import pathlib
+
 import ast
 import re
 
 
 @dataclass
 class Regexes:
     section: re.Pattern[str]
@@ -16,33 +20,37 @@
     variable: re.Pattern[str]
 
 
 regexes = Regexes(
     section=re.compile(r"^\[(?P<section>.*)\](#.*)?$"),
     comment=re.compile(r"^[#;]\s?(?P<comment>.*)$"),
     variable=re.compile(
-        r"^(?P<name>\w+(-\w+)*)\s*(:\s*(?P<type>\w+))?\s*((?P<not_required>=)\s*(?P<value>.*))?\s*([#;].*)?$"
+        r"^(?P<name>\w+(-\w+)*)\s*(:\s*(?P<type>\w+))?\s*(?P<not_required>=\s*(?P<value>.*))?\s*([#;].*)?$"
     ),
 )
 
 
 def read_config(config: FileLike, preconfig: Config | None = None) -> Config:
-    if isinstance(config, str):
-        with open(config) as file:
-            return read_config(file, preconfig)
+    # Mypy does not seem to like EAFP well
+    try:
+        config = pathlib.Path(config).read_text().splitlines()  # type: ignore[arg-type]
+    except TypeError:
+        pass
+    config_lines: Iterable[str] = config  # type: ignore[assignment]
+
     result: Config = (preconfig or {}).copy()
     result.setdefault(None, {})
 
     @dataclass
     class Current:
         section: str | None
         description: list[str]
 
     current = Current(section=None, description=[])
-    for i in config:
+    for i in config_lines:
         match i.strip():
             case "":
                 current.description = []
 
             case i if m := regexes.section.match(i):
                 current.section = m.group("section")
                 result[current.section] = result.get(current.section, {})
@@ -94,17 +102,17 @@
             case i:
                 raise ValueError(f"Could not parse line: {i}")
 
     return result
 
 
 def read_configs(
-    filenames: FileLike | list[FileLike], preconfig: Config | None = None
+    filenames: FileLike | Iterable[FileLike], preconfig: Config | None = None
 ) -> Config:
-    result = (preconfig or {}).copy()
-    if not isinstance(filenames, list):
+    if isinstance(filenames, str) or not isinstance(filenames, Iterable):
         filenames = [filenames]
+    result = (preconfig or {}).copy()
 
     for file in filenames:
         result = read_config(file, result)
 
     return result
```

### Comparing `click_schema_config-0.2.4/pyproject.toml` & `click_schema_config-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "click-schema-config"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Joy Void Joy <joy.void.joy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "click_schema_config"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `click_schema_config-0.2.4/PKG-INFO` & `click_schema_config-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

