# Comparing `tmp/sphinx_apitree-1.2.0.tar.gz` & `tmp/sphinx_apitree-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.2.0.tar` & `sphinx_apitree-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/LICENSE
--rw-r--r--   0        0        0     1980 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/README.md
--rw-r--r--   0        0        0      105 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/__init__.py
--rw-r--r--   0        0        0     1338 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ast_utils.py
--rw-r--r--   0        0        0     4146 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/conf_util.py
--rw-r--r--   0        0        0      761 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ext/docstring.py
--rw-r--r--   0        0        0      443 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ext/linkify.py
--rw-r--r--   0        0        0     1691 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/html_helper.py
--rw-r--r--   0        0        0       30 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/structs.py
--rw-r--r--   0        0        0     9597 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/symbol_match.py
--rw-r--r--   0        0        0      183 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/api.md
--rw-r--r--   0        0        0       13 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/function.md
--rw-r--r--   0        0        0      154 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/module.md
--rw-r--r--   0        0        0       13 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1693 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/tree_extractor.py
--rw-r--r--   0        0        0      782 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/writer.py
--rw-r--r--   0        0        0     1508 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 sphinx_apitree-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1980 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/README.md
+-rw-r--r--   0        0        0      105 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/__init__.py
+-rw-r--r--   0        0        0     2631 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ast_utils.py
+-rw-r--r--   0        0        0     4708 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/conf_util.py
+-rw-r--r--   0        0        0     1058 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/context.py
+-rw-r--r--   0        0        0     1761 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/auto_ref.py
+-rw-r--r--   0        0        0      808 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/docstring.py
+-rw-r--r--   0        0        0     2908 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/ext/github_link.py
+-rw-r--r--   0        0        0     1691 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/html_helper.py
+-rw-r--r--   0        0        0       30 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/structs.py
+-rw-r--r--   0        0        0    10880 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/symbol_match.py
+-rw-r--r--   0        0        0      183 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/api.md
+-rw-r--r--   0        0        0       42 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/function.md
+-rw-r--r--   0        0        0      154 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/module.md
+-rw-r--r--   0        0        0      121 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1728 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      738 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/apitree/writer.py
+-rw-r--r--   0        0        0     1556 2023-07-20 16:17:31.503757 sphinx_apitree-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 sphinx_apitree-1.3.0/PKG-INFO
```

### Comparing `sphinx_apitree-1.2.0/LICENSE` & `sphinx_apitree-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.2.0/README.md` & `sphinx_apitree-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.2.0/apitree/conf_util.py` & `sphinx_apitree-1.3.0/apitree/conf_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import functools
 import pathlib
+import tomllib
 from typing import Any
 
-import tomllib
+import sphinx
 from etils import epath, epy
 
 from apitree import structs, writer
-from apitree.ext import docstring
+from apitree.ext import github_link
 
 
 def setup(app, *, callbacks):
   for callback in callbacks:
     callback()
-  # Fix bad ```python md formatting
-  docstring.setup(app)
 
 
 def make_project(
     *,
     modules: dict[str, str] | structs.ModuleInfo,
     includes_paths: dict[str, str] = {},
     globals: dict[str, Any],
@@ -42,20 +41,24 @@
       copyright=f'2023, {project_name} authors',
       author=f'{project_name} authors',
       # General configuration
       extensions=[
           'myst_nb',  # Notebook support
           'sphinx.ext.napoleon',  # Numpy-style docstrings
           'sphinx.ext.autodoc',  # API Doc generator
+          'sphinx.ext.linkcode',  # Links to GitHub
           # Others:
           # 'sphinx_autodoc_typehints',
           # 'sphinx.ext.linkcode',
           # 'sphinx.ext.inheritance_diagram',
           # 'autoapi.extension',
           # 'myst_parser',
+          # API Tree
+          'apitree.ext.docstring',  # Fix bad ```python md formatting
+          'apitree.ext.auto_ref',  # Add cross ref for inline code
       ],
       exclude_patterns=[
           '_build',
           'jupyter_execute',
           'Thumbs.db',
           '.DS_Store',
       ],
@@ -92,14 +95,16 @@
                   _write_include_paths,
                   repo_dir=repo_dir,
                   docs_dir=docs_dir,
                   includes_paths=includes_paths,
               ),
           ],
       ),
+      # ---- linkcode -------------------------------------------------
+      linkcode_resolve=github_link.linkcode_resolve,
   )
 
 
 def _write_api_doc(
     *,
     docs_dir: pathlib.Path,
     modules: dict[str, str] | structs.ModuleInfo,
@@ -122,24 +127,32 @@
 
 def _write_include_paths(
     *,
     repo_dir: pathlib.Path,
     docs_dir: pathlib.Path,
     includes_paths: dict[str, str],
 ):
-  del repo_dir  # Could dynamically compute the `../../../`
   for repo_path, doc_path in includes_paths.items():
-    # repo_dir.parent / 'etils'
-    content = epy.dedent(
-        f"""
-        ```{{include}} ../{repo_path}
-        ```
-        """
-    )
-    docs_dir.joinpath(doc_path).write_text(content)
+    src_path = repo_dir / repo_path
+    dst_path = docs_dir / doc_path
+    match repo_path.suffix:
+      case '.md':
+        # repo_dir.parent / 'etils'
+        # Could dynamically compute the `../../../`
+        content = epy.dedent(
+            f"""
+            ```{{include}} ../{repo_path}
+            ```
+            """
+        )
+        dst_path.write_text(content)
+      case '.ipynb':
+        dst_path.write_bytes(src_path.read_bytes())
+      case default:
+        raise ValueError(f'Invalid suffix: {default}')
 
 
 def _get_project_name(repo_dir):
   # TODO(epot): This hardcode too much assumption on the program
   path = repo_dir / 'pyproject.toml'
   info = tomllib.loads(path.read_text())
   return info['project']['name']
```

### Comparing `sphinx_apitree-1.2.0/apitree/ext/docstring.py` & `sphinx_apitree-1.3.0/apitree/ext/docstring.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Fix bad ```python md formatting."""
 
+from sphinx.application import Sphinx
+
 
 def _preprocess_docstring(app, what, name, obj, options, lines):
   # Modify each line of the docstring
   is_block = False
   new_lines = []
   for line in lines:
     if line == '```python':
@@ -21,10 +23,10 @@
     else:
       if is_block:
         line = f'  {line}'
       new_lines.append(line)
   lines[:] = new_lines
 
 
-def setup(app):
+def setup(app: Sphinx):
   # Fix bad ```python md formatting
   app.connect('autodoc-process-docstring', _preprocess_docstring)
```

### Comparing `sphinx_apitree-1.2.0/apitree/html_helper.py` & `sphinx_apitree-1.3.0/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.2.0/apitree/symbol_match.py` & `sphinx_apitree-1.3.0/apitree/symbol_match.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import dataclasses
 import functools
 import os
 import pathlib
 import types
+import typing
 from collections.abc import Callable, Iterator
 from typing import Any
 
 import typing_extensions
 from etils import edc, epath, epy
 
 from apitree import ast_utils, md_utils, tree_extractor
+from apitree.ext import github_link
 
 
 @edc.dataclass
 @dataclasses.dataclass
 class Context:
   module_name: str
   alias: str
@@ -50,27 +52,31 @@
     return self.value.__name__.startswith(self.ctx.module_name)
 
   @functools.cached_property
   def match(self) -> type[Match]:
     return Match.root_match(self)
 
   @functools.cached_property
-  def qualname(self) -> bool:
+  def qualname(self) -> str:
     """Exemple: `dca.typing.Float`."""
     if self.parent_symb is None:  # root node
       # assert self.ctx.module_name == self.name
       return self.ctx.alias
     return f'{self.parent_symb.symbol.qualname}.{self.name}'
 
   @functools.cached_property
-  def qualname_no_alias(self) -> bool:
+  def qualname_no_alias(self) -> str:
     """Exemple: `dataclass_array.typing.Float`."""
-    if self.parent_symb is None:  # root node
-      return self.name
-    return f'{self.parent_symb.symbol.qualname_no_alias}.{self.name}'
+    if isinstance(self.value, types.ModuleType):
+      try:
+        return self.value.__name__
+      except Exception:  # TODO(epot): Better lazy-modules
+        return ''
+    else:
+      return f'{self.parent_symb.symbol.qualname_no_alias}.{self.name}'
 
   # Return type
 
 
 class Match:
   symbol: Symbol
 
@@ -208,14 +214,15 @@
   @property
   def extra_template_kwargs(self):
     return dict(
         toctree=self.toctree,
         symbols_table=self.make_symbols_table(
             self.symbol.node.documented_childs
         ),
+        **super().extra_template_kwargs,
     )
 
   @property
   def toctree(self) -> str:
     items = []
     for n in self.symbol.node.documented_childs:
       path = n.match.filename.relative_to(self.filename.parent)
@@ -357,21 +364,50 @@
     # Only document imported values when the parent is a package
     return not self.symbol.is_imported or _is_package(self.symbol.parent)
 
 
 # TODO(epot): How to duplicate this with _ImportedValue ?
 
 
-class _TypeAliasValue(_DocumentedValue):
+class _WithSourceLink(Match):
+
+  @property
+  def extra_template_kwargs(self):
+    module_name = self.symbol.parent.__name__
+    filepath = github_link._get_definition_line(module_name, self.symbol.name)
+    source_link = f'{github_link._get_github_url()}/tree/main/{filepath}'
+    return dict(
+        source_link=source_link,
+        **super().extra_template_kwargs,
+    )
+
+
+class _TypeAliasValue(_DocumentedValue, _WithSourceLink):
   icon = 't'
   template_name = 'type_alias'
 
   def match(self):
     # TODO(epot): How to detect `Any`,...
-    return typing_extensions.get_origin(self.symbol.value) is not None
+
+    return (
+        isinstance(self.symbol.value, typing.TypeVar)
+        or typing_extensions.get_origin(self.symbol.value) is not None
+    )
+
+  @property
+  def extra_template_kwargs(self):
+    # TODO(epot): Extract the first and last line of the assignment
+    # module_name = self.symbol.parent.__name__
+    # filepath = github_link._get_definition_line(module_name, self.symbol.name)
+    # source_link = f'{github_link._get_github_url()}/tree/main/{filepath}'
+    source_code = ''
+    return dict(
+        source_code=source_code,
+        **super().extra_template_kwargs,
+    )
 
 
 class _ClassValue(_WithDocstring, _DocumentedValue):
   icon = 'c'
   template_name = 'class'
 
   def match(self):
@@ -380,19 +416,26 @@
 
 class _FunctionValue(_WithDocstring, _DocumentedValue):
   icon = 'f'
   template_name = 'function'
 
   def match(self):
     return isinstance(
-        self.symbol.value, (types.FunctionType, functools.partial)
+        self.symbol.value,
+        (
+            types.FunctionType,
+            types.BuiltinFunctionType,
+            types.BuiltinMethodType,
+            types.MethodType,
+            types.MethodWrapperType,
+        ),
     )
 
 
-class _AttributeValue(_DocumentedValue):
+class _AttributeValue(_DocumentedValue, _WithSourceLink):
   icon = 'a'
   template_name = 'attribute'
 
   # TODO(epot): Extract doc from parent
 
 
 def _is_package(module: types.ModuleType) -> bool:
```

### Comparing `sphinx_apitree-1.2.0/apitree/tree_extractor.py` & `sphinx_apitree-1.3.0/apitree/tree_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import functools
 import importlib
 import types
 from typing import Iterator
 
 from etils import edc, epy
 
-from apitree import structs, symbol_match
+from apitree import context, structs, symbol_match
 
 
 @dataclasses.dataclass
 class Node:
   symbol: symbol_match.Symbol
 
   def __post_init__(self):
     self.symbol.node = self
+    context.add_ref(self)
 
   @property
   def match(self):
     return self.symbol.match
 
   @functools.cached_property
   def childs(self) -> list[Node]:
```

### Comparing `sphinx_apitree-1.2.0/apitree/writer.py` & `sphinx_apitree-1.3.0/apitree/writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from apitree import structs, symbol_match, tree_extractor
 
 
 def write_doc(
     info: structs.ModuleInfo,
     *,
     verbose=True,
-    module_info: structs.ModuleInfo = None,
     root_dir: epath.Path = None,
 ) -> None:
   node = tree_extractor.get_api_tree(info)
   if not root_dir:
     root_dir = epath.resource_path(node.symbol.value)
     root_dir = root_dir.parent / 'docs/api'
```

### Comparing `sphinx_apitree-1.2.0/pyproject.toml` & `sphinx_apitree-1.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 [project.optional-dependencies]
 dev = [
     "pytest>=3.4",
     "pytest-xdist",
     # Development deps (linting, formating,...)
     "pylint>=2.6.0",
     "pyink",
+    "sphinx-apitree[ext]",
+    "etils[ecolab]",
 ]
 # Extensions used by `apitree.make_project`
 ext = [
     "sphinx",
     "myst_nb",
     "sphinx_book_theme",
 ]
```

### Comparing `sphinx_apitree-1.2.0/PKG-INFO` & `sphinx_apitree-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.2.0
+Version: 1.3.0
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -12,14 +12,16 @@
 Classifier: Intended Audience :: Developers
 Requires-Dist: etils[edc,enp,epath,epy,etree]
 Requires-Dist: typing_extensions
 Requires-Dist: pytest>=3.4 ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
 Requires-Dist: pyink ; extra == "dev"
+Requires-Dist: sphinx-apitree[ext] ; extra == "dev"
+Requires-Dist: etils[ecolab] ; extra == "dev"
 Requires-Dist: sphinx ; extra == "ext"
 Requires-Dist: myst_nb ; extra == "ext"
 Requires-Dist: sphinx_book_theme ; extra == "ext"
 Project-URL: homepage, https://github.com/conchylicultor/sphinx-apitree
 Project-URL: repository, https://github.com/conchylicultor/sphinx-apitree
 Provides-Extra: dev
 Provides-Extra: ext
```

