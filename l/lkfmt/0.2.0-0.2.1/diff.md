# Comparing `tmp/lkfmt-0.2.0-py3-none-any.whl.zip` & `tmp/lkfmt-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7053 bytes, number of entries: 9
--rw-r--r--  2.0 unx      172 b- defN 80-Jan-01 00:00 lkfmt/__init__.py
--rw-r--r--  2.0 unx      631 b- defN 80-Jan-01 00:00 lkfmt/__main__.py
--rw-r--r--  2.0 unx     5802 b- defN 80-Jan-01 00:00 lkfmt/diff.py
--rw-r--r--  2.0 unx     6160 b- defN 80-Jan-01 00:00 lkfmt/main.py
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 lkfmt-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1705 b- defN 80-Jan-01 00:00 lkfmt-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lkfmt-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 lkfmt-0.2.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 lkfmt-0.2.0.dist-info/RECORD
-9 files, 16341 bytes uncompressed, 5923 bytes compressed:  63.8%
+Zip file size: 7289 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 lkfmt/__init__.py
+-rw-r--r--  2.0 unx      641 b- defN 80-Jan-01 00:00 lkfmt/__main__.py
+-rw-r--r--  2.0 unx     5807 b- defN 80-Jan-01 00:00 lkfmt/diff.py
+-rw-r--r--  2.0 unx     6219 b- defN 80-Jan-01 00:00 lkfmt/formatter.py
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2075 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 lkfmt-0.2.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      670 b- defN 16-Jan-01 00:00 lkfmt-0.2.1.dist-info/RECORD
+9 files, 16805 bytes uncompressed, 6149 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: lkfmt/__main__.py
 Comment: 
 
 Filename: lkfmt/diff.py
 Comment: 
 
-Filename: lkfmt/main.py
+Filename: lkfmt/formatter.py
 Comment: 
 
-Filename: lkfmt-0.2.0.dist-info/LICENSE
+Filename: lkfmt-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: lkfmt-0.2.0.dist-info/METADATA
+Filename: lkfmt-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: lkfmt-0.2.0.dist-info/WHEEL
+Filename: lkfmt-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: lkfmt-0.2.0.dist-info/entry_points.txt
+Filename: lkfmt-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: lkfmt-0.2.0.dist-info/RECORD
+Filename: lkfmt-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lkfmt/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .diff import show_diff
 from .diff import stat_changes
-from .main import fmt_all
-from .main import fmt_one
-from .main import fmt_one as fmt_file
+from .formatter import fmt_all
+from .formatter import fmt_one
+from .formatter import fmt_one as fmt_file
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

## lkfmt/__main__.py

```diff
@@ -1,13 +1,13 @@
 from argsense import cli
 from lk_utils import loads
 
 from . import diff
-from .main import fmt_all
-from .main import fmt_one
+from .formatter import fmt_all
+from .formatter import fmt_one
 
 cli.add_cmd(fmt_all, name='fmt')
 
 
 @cli.cmd()
 def show_diff(file: str) -> None:
     src_code = loads(file, 'plain')
```

## lkfmt/diff.py

```diff
@@ -73,15 +73,15 @@
                     )
                 ),
             ),
         )
 
 
 def _diff(a: t.Sequence[str], b: t.Sequence[str]) -> T.Diffs0:
-    from .main import _debug
+    from .formatter import _debug
     out: T.Diffs0 = []
     for diff in ndiff(a, b):
         mask, line = diff[0], diff[2:].replace('\n', '')
         if _debug:
             print(f'[{mask}]', line, ':vsi2')
         out.append((mask, line))  # noqa
     return out
```

## Comparing `lkfmt/main.py` & `lkfmt/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 
 lk_logger.setup(quiet=True, show_funcname=False, show_varnames=False)
 
 
 class Cache:
     _cache: dict  # dict[path, mtime]
     _file: str
-    
+
     def __init__(self):
         self._file = xpath('.cache.pkl')
         if os.path.exists(self._file):
             self._cache = loads(self._file)
         else:
             self._cache = {}
-    
+
     def get(self, path: str) -> t.Union[float, 0]:
         return self._cache.get(path, 0)
-    
+
     def set(self, path: str, mtime: float) -> None:
         self._cache[path] = mtime
-    
+
     def save(self) -> None:
         dumps(self._cache, self._file)
-    
+
     def disable(self) -> None:
         self._cache.clear()
         setattr(self, 'save', lambda: None)
 
 
 _cache = Cache()
 _debug = False
@@ -70,29 +70,29 @@
     global _debug
     if backdoor.get('debug'):
         _debug = True
         print(f'{backdoor = }', ':v')
     if backdoor.get('direct_to_fmt_file'):
         fmt_one(target, inplace, chdir)
         return
-    
+
     root: str
     files: t.List[str]
-    
+
     if target == '.':
         root = fs.abspath(os.getcwd())
     elif os.path.isdir(target):
         root = fs.abspath(target)
     elif os.path.isfile(target):
         _cache.set(target, os.path.getmtime(target))
         fmt_one(target, inplace, chdir)
         return
     else:
         raise ValueError(f'invalid target: {target}')
-    
+
     if no_cache:
         _cache.disable()
     if recursive:
         files = fs.findall_file_paths(root, '.py')
     else:
         files = fs.find_file_paths(root, '.py')
     if not files:
@@ -107,19 +107,19 @@
     if temp:
         files = temp
         if _debug:
             print(files, ':vl')
     else:
         print('[green dim]no file modified[/]', ':rt')
         return
-        
+
     def estimate_best_column_width(files: t.List[str]) -> int:
-        max_width = max(map(len, map(fs.filename, files)))
-        return min((max_width, lk_logger.console.console.width))
-    
+        maxlen = max(map(len, map(fs.filename, files)))
+        return min((maxlen, 80, lk_logger.console.console.width))
+
     file_col_width = estimate_best_column_width(files)
     cnt = 0
     for f in files:
         _, (i, u, d) = fmt_one(f, inplace, chdir, quiet=True)
         if (i, u, d) != (0, 0, 0):
             cnt += 1
         print(
@@ -156,18 +156,18 @@
 ) -> t.Tuple[str, T.Changes]:
     if quiet:
         lk_logger.mute()
     print(':v2s', file)
     assert file.endswith(('.py', '.txt'))
     if chdir:
         os.chdir(os.path.dirname(os.path.abspath(file)))
-    
+
     with open(file, 'r', encoding='utf-8') as f:
         code = origin_code = f.read()
-    
+
     code = black.format_str(
         code,
         mode=black.Mode(
             line_length=80,
             string_normalization=False,
             magic_trailing_comma=False,
             preview=True,
@@ -179,29 +179,31 @@
             case_sensitive=True,
             force_single_line=True,
             line_length=80,
             only_modified=True,
             profile='black',
         ),
     )
-    code = autoflake.fix_code(
-        code,
-        remove_all_unused_imports=True,
-        ignore_pass_statements=False,
-        ignore_pass_after_docstring=False,
-    )
-    
+    if not fs.filename(file) == '__init__.py':
+        # we don't strip any import in `__init__.py`.
+        code = autoflake.fix_code(
+            code,
+            remove_all_unused_imports=True,
+            ignore_pass_statements=False,
+            ignore_pass_after_docstring=False,
+        )
+
     if code == origin_code:
         print('[green dim]no code change[/]', ':rt')
         return code, (0, 0, 0)
-    
+
     if inplace:
         with open(file, 'w', encoding='utf-8') as f:
             f.write(code)
-    
+
     i, u, d = stat_changes(origin_code, code, verbose=False)
     print(
         '[green]reformat code done: '
         '[cyan {dim_i}]{i} insertions,[/] '
         '[yellow {dim_u}]{u} updates,[/] '
         '[red {dim_d}]{d} deletions[/]'
         '[/]'.format(
```

## Comparing `lkfmt-0.2.0.dist-info/LICENSE` & `lkfmt-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lkfmt-0.2.0.dist-info/METADATA` & `lkfmt-0.2.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkfmt
-Version: 0.2.0
+Version: 0.2.1
 Summary: All-in-one Python code formattor which is tailored of `black` + `isort` + `autoflake` for myself taste.
 Home-page: https://github.com/likianta/lkfmt
 License: MIT
 Author: likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -46,17 +46,37 @@
 
 ```sh
 pip install git+https://github.com/likianta/lkfmt.git
 ```
 
 ## Usage
 
-...
+use in command line:
 
-## Screenshots
+```sh
+# after installation, there's an executable named `lkfmt`.
 
-![](./.assets/125742.png)
+# get help
+lkfmt -h
+
+# format files in current dir
+lkfmt .
+# it can also be shorthand as `lkfmt` (no argument)
+
+# format files in current dir and subdirs recursively
+lkfmt -r .
+
+# format one file
+lkfmt $file
+
+# show difference (but not inplace file)
+python -m lkfmt show-diff $file
+```
+
+## Screenshots
 
 ![](./.assets/125758.png)
 
+![](./.assets/125742.png)
+
 ![](./.assets/125801.png)
```

