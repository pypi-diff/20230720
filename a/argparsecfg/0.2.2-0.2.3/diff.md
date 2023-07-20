# Comparing `tmp/argparsecfg-0.2.2.tar.gz` & `tmp/argparsecfg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparsecfg-0.2.2.tar", last modified: Tue May 23 08:06:28 2023, max compression
+gzip compressed data, was "argparsecfg-0.2.3.tar", last modified: Thu Jul 20 09:03:47 2023, max compression
```

## Comparing `argparsecfg-0.2.2.tar` & `argparsecfg-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-03-01 13:23:52.000000 argparsecfg-0.2.2/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)       39 2023-03-01 13:28:51.000000 argparsecfg-0.2.2/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      635 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-03-01 13:26:27.000000 argparsecfg-0.2.2/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.766917 argparsecfg-0.2.2/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.770917 argparsecfg-0.2.2/src/argparsecfg/
--rw-rw-r--   0 aya       (1000) aya       (1000)      168 2023-05-16 08:07:33.000000 argparsecfg-0.2.2/src/argparsecfg/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)    11856 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/src/argparsecfg/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-05-17 17:59:38.000000 argparsecfg-0.2.2/src/argparsecfg/test_tools.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/src/argparsecfg/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.770917 argparsecfg-0.2.2/src/argparsecfg.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)      510 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      560 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       48 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       12 2023-05-23 08:06:28.000000 argparsecfg-0.2.2/src/argparsecfg.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-23 08:06:28.774917 argparsecfg-0.2.2/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     5664 2023-05-17 12:03:24.000000 argparsecfg-0.2.2/tests/test_add_argument_field.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4103 2023-05-23 08:03:10.000000 argparsecfg-0.2.2/tests/test_add_argument_field_errors.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4307 2023-05-11 15:13:36.000000 argparsecfg-0.2.2/tests/test_add_argument_metadata.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2055 2023-05-11 15:13:36.000000 argparsecfg-0.2.2/tests/test_add_argument_simple.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1184 2023-05-06 09:44:14.000000 argparsecfg-0.2.2/tests/test_create_parser.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      517 2023-04-28 14:29:56.000000 argparsecfg-0.2.2/tests/test_parse_args.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3942 2023-05-15 08:47:52.000000 argparsecfg-0.2.2/tests/test_test_tools.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 09:03:47.201756 argparsecfg-0.2.3/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      766 2023-07-20 09:03:47.201756 argparsecfg-0.2.3/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      295 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      635 2023-07-20 09:03:47.201756 argparsecfg-0.2.3/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 09:03:47.193755 argparsecfg-0.2.3/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 09:03:47.197755 argparsecfg-0.2.3/src/argparsecfg/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      168 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/src/argparsecfg/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5944 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/src/argparsecfg/app.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11963 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/src/argparsecfg/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/src/argparsecfg/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/src/argparsecfg/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 09:03:47.197755 argparsecfg-0.2.3/src/argparsecfg.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      766 2023-07-20 09:03:47.000000 argparsecfg-0.2.3/src/argparsecfg.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      583 2023-07-20 09:03:47.000000 argparsecfg-0.2.3/src/argparsecfg.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-20 09:03:47.000000 argparsecfg-0.2.3/src/argparsecfg.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       48 2023-07-20 09:03:47.000000 argparsecfg-0.2.3/src/argparsecfg.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       12 2023-07-20 09:03:47.000000 argparsecfg-0.2.3/src/argparsecfg.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 09:03:47.201756 argparsecfg-0.2.3/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5664 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_add_argument_field.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4103 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_add_argument_field_errors.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4307 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_add_argument_metadata.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2055 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1184 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      517 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3942 2023-05-25 20:13:02.000000 argparsecfg-0.2.3/tests/test_test_tools.py
```

### Comparing `argparsecfg-0.2.2/LICENSE` & `argparsecfg-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/setup.cfg` & `argparsecfg-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/setup.py` & `argparsecfg-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/src/argparsecfg/core.py` & `argparsecfg-0.2.3/src/argparsecfg/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,18 @@
     Parameters same as at argparse.ArgumentParser.
     """
 
     prog: str | None = None
     usage: str | None = None
     description: str | None = None
     epilog: str | None = None
-    parents: list[str] = field(default_factory=list)
+    parents: Sequence[argparse.ArgumentParser] = field(default_factory=list)
     formatter_class: Type[HelpFormatter] = HelpFormatter
     prefix_chars: str = "-"
-    fromfile_prefix_chars: bool | None = None
+    fromfile_prefix_chars: str | None = None
     argument_default: str | None = None
     conflict_handler: str = "error"
     add_help: bool = True
     allow_abbrev: bool = True
     exit_on_error: bool = True
 
 
@@ -71,15 +71,18 @@
 def add_argument_metadata(
     *name_or_flags: str | None,
     flag: str | None = None,
     action: str | None = None,
     nargs: int | str | None = None,
     const: str | None = None,
     default: Any = None,
-    type: str | argparse.FileType | type | None = None,  # pylint: disable=redefined-builtin
+    type: str
+    | argparse.FileType
+    | type
+    | None = None,  # pylint: disable=redefined-builtin
     choices: Iterable[Any] | None = None,
     required: bool | None = None,
     help: str | None = None,  # pylint: disable=redefined-builtin
     metavar: str | tuple[str, ...] | None = None,
     dest: str | None = None,
     # version: str | None = None,  # pylint: disable=unused-argument  # not implemented
 ) -> dict[str, Any]:
@@ -252,15 +255,18 @@
     if dataclasses.is_dataclass(dc):
         for dc_field in dc.__dataclass_fields__.values():
             add_arg(parser, dc_field)
     else:
         print(f"Warning: {type(dc)} not dataclass type")  # ? warning ?
 
 
-def extract_flags(dc: type[Any], prefix: str = "-",):
+def extract_flags(
+    dc: type[Any],
+    prefix: str = "-",
+):
     flag_name: dict[str, str] = {}
     for name, fld in dc.__dataclass_fields__.items():
         flag = fld.metadata.get("flag", None)
         if flag is not None:
             flag = flag.lstrip(prefix)
             if len(flag) > 1:
                 flag_name[flag] = name
@@ -274,23 +280,27 @@
         return None  # ? raise error ?
     kwargs = {
         key: val for key, val in args.__dict__.items() if key in dc.__dataclass_fields__
     }
     flag_name = extract_flags(dc)  # ??prefix
     if flag_name:
         kwargs.update(
-            {flag_name[key]: val for key, val in args.__dict__.items() if key in flag_name}
+            {
+                flag_name[key]: val
+                for key, val in args.__dict__.items()
+                if key in flag_name
+            }
         )
     return dc(**kwargs)
 
 
 def parse_args(
-        cfg: Type[Any],
-        parser_cfg: ArgumentParserCfg | None = None,
-        args: Sequence[str] | None = None,
+    cfg: Type[Any],
+    parser_cfg: ArgumentParserCfg | None = None,
+    args: Sequence[str] | None = None,
 ) -> Any:
     """parse args"""
     parser = create_parser(parser_cfg)
     add_args_from_dc(parser, cfg)
     parsed_args = parser.parse_args(args=args)
     return create_dc_obj(cfg, parsed_args)
 
@@ -305,15 +315,18 @@
     compare: bool = True,
     metadata: Mapping[Any, Any] | None = None,
     kw_only: bool = MISSING,  # type: ignore
     flag: str | None = None,
     action: str | None = None,
     nargs: int | str | None = None,
     const: Any = None,
-    type: str | argparse.FileType | type | None = None,  # pylint: disable=redefined-builtin
+    type: str
+    | argparse.FileType
+    | type
+    | None = None,  # pylint: disable=redefined-builtin
     choices: Iterable[Any] | None = None,
     required: bool | None = None,
     help: str | None = None,  # pylint: disable=redefined-builtin
     metavar: str | None = None,
     dest: str | None = None,
     version: str | None = None,  # pylint: disable=unused-argument
 ) -> Any:
```

### Comparing `argparsecfg-0.2.2/src/argparsecfg/test_tools.py` & `argparsecfg-0.2.3/src/argparsecfg/test_tools.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/src/argparsecfg.egg-info/SOURCES.txt` & `argparsecfg-0.2.3/src/argparsecfg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/argparsecfg/__init__.py
+src/argparsecfg/app.py
 src/argparsecfg/core.py
 src/argparsecfg/test_tools.py
 src/argparsecfg/version.py
 src/argparsecfg.egg-info/PKG-INFO
 src/argparsecfg.egg-info/SOURCES.txt
 src/argparsecfg.egg-info/dependency_links.txt
 src/argparsecfg.egg-info/requires.txt
```

### Comparing `argparsecfg-0.2.2/tests/test_add_argument_field.py` & `argparsecfg-0.2.3/tests/test_add_argument_field.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_add_argument_field_errors.py` & `argparsecfg-0.2.3/tests/test_add_argument_field_errors.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_add_argument_metadata.py` & `argparsecfg-0.2.3/tests/test_add_argument_metadata.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_add_argument_simple.py` & `argparsecfg-0.2.3/tests/test_add_argument_simple.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_create_parser.py` & `argparsecfg-0.2.3/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_parse_args.py` & `argparsecfg-0.2.3/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `argparsecfg-0.2.2/tests/test_test_tools.py` & `argparsecfg-0.2.3/tests/test_test_tools.py`

 * *Files identical despite different names*

