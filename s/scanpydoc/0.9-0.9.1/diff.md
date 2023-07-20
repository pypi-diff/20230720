# Comparing `tmp/scanpydoc-0.9.tar.gz` & `tmp/scanpydoc-0.9.1.tar.gz`

## Comparing `scanpydoc-0.9.tar` & `scanpydoc-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9/.editorconfig
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9/.prettierrc.yaml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.9/.readthedocs.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 scanpydoc-0.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9/.vscode/settings.json
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 scanpydoc-0.9/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9/docs/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/_version.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/py.typed
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/rtd_github_links/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/rtd_github_links/_linkcode.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9/src/scanpydoc/theme/static/styles/scanpy.css
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9/tests/test_base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 scanpydoc-0.9/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9/.gitignore
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9/README.rst
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 scanpydoc-0.9/pyproject.toml
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 scanpydoc-0.9/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.editorconfig
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.prettierrc.yaml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/requirements.lock
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/_linkcode.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/static/styles/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/README.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/PKG-INFO
```

### Comparing `scanpydoc-0.9/.pre-commit-config.yaml` & `scanpydoc-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/.github/workflows/ci.yml` & `scanpydoc-0.9.1/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
           path: |
             ~/.cache/pip
             ~/.cache/pre-commit
           key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
       - name: dependencies
         run: |
           pip install --upgrade pip wheel
-          pip install -e .[test,typehints]
+          pip install .[test,typehints]
       - name: tests
         run: pytest --color=yes
```

### Comparing `scanpydoc-0.9/docs/conf.py` & `scanpydoc-0.9.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import sys
 from datetime import datetime
 from importlib.metadata import metadata
 from pathlib import Path
 
 from sphinx.application import Sphinx
 
 
 HERE = Path(__file__).parent
 
-# necessary for rtd_gh_links’ linkcode support
-sys.path.insert(0, HERE.parent / "src")
-
 # Clean build env
 for file in HERE.glob("scanpydoc.*.rst"):
     file.unlink()
 
 extensions = [
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
@@ -45,14 +41,15 @@
 version = release = meta["version"]
 
 master_doc = "index"
 templates_path = ["_templates"]
 
 # Generate .rst stubs for modules using autosummary
 autosummary_generate = True
+autosummary_ignore_module_all = False
 # Don’t add module paths to documented functions’ names
 add_module_names = False
 
 html_theme = "scanpydoc"
 html_context = dict(
     repository_url="https://github.com/theislab/scanpydoc",
     repository_branch="main",
```

### Comparing `scanpydoc-0.9/docs/_templates/autosummary/module.rst` & `scanpydoc-0.9.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/__init__.py` & `scanpydoc-0.9.1/src/scanpydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.9.1/src/scanpydoc/autosummary_generate_imported.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.9.1/src/scanpydoc/definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 from sphinx.config import Config
 from sphinx.ext.autodoc import ClassDocumenter
 
 from .. import _setup_sig, metadata
 from .example import example_func
 
 
+__all__ = ["example_func", "setup"]
+
+
 HERE = Path(__file__).parent.resolve()
 
 qualname_overrides_default = {
     "anndata.base.AnnData": "anndata.AnnData",
     "anndata.core.anndata.AnnData": "anndata.AnnData",
     "anndata._core.anndata.AnnData": "anndata.AnnData",
     "matplotlib.axes._axes.Axes": "matplotlib.axes.Axes",
@@ -84,17 +87,14 @@
         )
     if config.typehints_defaults is None and config.annotate_defaults:
         # override default for “typehints_defaults”
         config.typehints_defaults = "braces"
     config.html_static_path.append(str(HERE / "static"))
 
 
-example_func.__module__ = "scanpydoc.elegant_typehints"  # Make it show up here
-
-
 @_setup_sig
 def setup(app: Sphinx) -> dict[str, Any]:
     """Patches :mod:`sphinx_autodoc_typehints` for a more elegant display."""
     # TODO: Unsure if “html” is sufficient or if we need to do “env”;
     #       Depends on when the autodoc-process-docstring event is handled.
     app.add_config_value("qualname_overrides", {}, "html")
     app.add_config_value("annotate_defaults", True, "html")
```

### Comparing `scanpydoc-0.9/src/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/rtd_github_links/__init__.py` & `scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 
 #. It registers a :ref:`Jinja filter <jinja:filters>` called :func:`github_url`
    that you can use to convert a module path into a GitHub URL.
 #. It configures :mod:`sphinx.ext.linkcode` for you if loaded after it in ``conf.py``:
 
    .. code:: python
 
-      import sys
-      from pathlib import Path
-
-      HERE = Path(__file__).parent
-      # make sure modules are import from the right place
-      sys.path.insert(0, HERE.parent / "src")
-
       extensions = [
           "scanpydoc",
           "sphinx.ext.linkcode",
       ]
 
       # no need to define `linkcode_resolve`
 
@@ -63,14 +56,15 @@
 .. _autosummary templates: \
    http://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html#customizing-templates
 """
 from __future__ import annotations
 
 import inspect
 import sys
+from importlib import import_module
 from pathlib import Path, PurePosixPath
 from types import ModuleType
 from typing import Any
 
 from jinja2.defaults import DEFAULT_FILTERS
 from sphinx.application import Sphinx
 from sphinx.config import Config
@@ -104,22 +98,26 @@
     while modname not in sys.modules:
         modname, leaf = modname.rsplit(".", 1)
         attr_path.insert(0, leaf)
 
     # retrieve object and find original module name
     mod = sys.modules[modname]
     obj = None
+    del modname
     for attr_name in attr_path:
         try:
             thing = getattr(mod if obj is None else obj, attr_name)
-        except AttributeError:
+        except AttributeError as e:
             if is_dataclass(obj):
                 thing = next(f for f in fields(obj) if f.name == attr_name)
             else:
-                raise
+                try:
+                    thing = import_module(f"{mod.__name__}.{attr_name}")
+                except ImportError:
+                    raise e from None
         if isinstance(thing, ModuleType):
             mod = thing
         else:
             obj = thing
             mod_orig = getattr(obj, "__module__", None)
             if mod_orig is not None:
                 mod = sys.modules[mod_orig]
@@ -133,20 +131,23 @@
         lines, start = inspect.getsourcelines(obj)
     except TypeError:
         return None, None
     else:
         return start, start + len(lines) - 1
 
 
-def _module_path(module: ModuleType) -> PurePosixPath:
-    stem = PurePosixPath(*module.__name__.split("."))
-    if Path(module.__file__).name == "__init__.py":
-        return stem / "__init__.py"
-    else:
-        return stem.with_suffix(".py")
+def _module_path(obj: Any, module: ModuleType) -> PurePosixPath:
+    """Relative module path to parent directory of toplevel module."""
+    try:
+        file = Path(inspect.getabsfile(obj))
+    except TypeError:
+        file = Path(module.__file__)
+    offset = -1 if file.name == "__init__.py" else 0
+    parts = module.__name__.split(".")
+    return PurePosixPath(*file.parts[offset - len(parts) :])
 
 
 def github_url(qualname: str) -> str:
     """Get the full GitHub URL for some object’s qualname.
 
     Args:
         qualname: The full qualified name of a function, class, method or module
@@ -155,15 +156,15 @@
         A GitHub URL derived from the :confval:`html_context`.
     """
     try:
         obj, module = _get_obj_module(qualname)
     except Exception:
         print(f"Error in github_url({qualname!r}):", file=sys.stderr)
         raise
-    path = rtd_links_prefix / _module_path(module)
+    path = rtd_links_prefix / _module_path(obj, module)
     start, end = _get_linenos(obj)
     fragment = f"#L{start}-L{end}" if start and end else ""
     return f"{github_base_url}/{path}{fragment}"
 
 
 def _check_html_context(config: Config):
     try:
```

### Comparing `scanpydoc-0.9/src/scanpydoc/rtd_github_links/_linkcode.py` & `scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/_linkcode.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/theme/__init__.py` & `scanpydoc-0.9.1/src/scanpydoc/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/theme/layout.html` & `scanpydoc-0.9.1/src/scanpydoc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/src/scanpydoc/theme/theme.conf` & `scanpydoc-0.9.1/src/scanpydoc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/tests/conftest.py` & `scanpydoc-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/tests/test_base.py` & `scanpydoc-0.9.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/tests/test_definition_list_typed_field.py` & `scanpydoc-0.9.1/tests/test_definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/tests/test_elegant_typehints.py` & `scanpydoc-0.9.1/tests/test_elegant_typehints.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/LICENSE` & `scanpydoc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/README.rst` & `scanpydoc-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9/pyproject.toml` & `scanpydoc-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 [tool.hatch.version]
 source = 'vcs'
 [tool.hatch.build.hooks.vcs]
 version-file = 'src/scanpydoc/_version.py'
 
 [tool.hatch.envs.docs]
+python = '3.11'
 features = ['doc']
 [tool.hatch.envs.docs.scripts]
 build = 'sphinx-build -M html docs docs/_build'
 
 [[tool.hatch.envs.test.matrix]]
 python = ['3.8', '3.9', '3.10', '3.11']
 [tool.hatch.envs.test]
```

### Comparing `scanpydoc-0.9/PKG-INFO` & `scanpydoc-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.9
+Version: 0.9.1
 Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
 Project-URL: Source, https://github.com/theislab/scanpydoc/
 Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Author-email: Philipp Angerer <phil.angerer@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Sphinx :: Extension
```

