# Comparing `tmp/scanpydoc-0.9.1.tar.gz` & `tmp/scanpydoc-0.9.2.tar.gz`

## Comparing `scanpydoc-0.9.1.tar` & `scanpydoc-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.editorconfig
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.prettierrc.yaml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.readthedocs.yml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/requirements-dev.lock
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/requirements.lock
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.vscode/settings.json
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/_version.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/py.typed
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/_linkcode.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/src/scanpydoc/theme/static/styles/scanpy.css
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/.gitignore
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/README.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.editorconfig
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.prettierrc.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.readthedocs.yml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/_linkcode.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/static/styles/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/README.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/PKG-INFO
```

### Comparing `scanpydoc-0.9.1/.pre-commit-config.yaml` & `scanpydoc-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/.github/workflows/ci.yml` & `scanpydoc-0.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/docs/conf.py` & `scanpydoc-0.9.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from datetime import datetime
 from importlib.metadata import metadata
-from pathlib import Path
+from pathlib import PurePosixPath
 
 from sphinx.application import Sphinx
 
 
-HERE = Path(__file__).parent
-
-# Clean build env
-for file in HERE.glob("scanpydoc.*.rst"):
-    file.unlink()
-
 extensions = [
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",  # needs to be after napoleon
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "scanpydoc",
@@ -52,15 +46,15 @@
 html_theme = "scanpydoc"
 html_context = dict(
     repository_url="https://github.com/theislab/scanpydoc",
     repository_branch="main",
     use_repository_button=True,
 )
 
-rtd_links_prefix = "src"
+rtd_links_prefix = PurePosixPath("src")
 
 
 def setup(app: Sphinx):
     app.add_object_type(
         "confval",
         "confval",
         objname="configuration value",
```

### Comparing `scanpydoc-0.9.1/docs/_templates/autosummary/module.rst` & `scanpydoc-0.9.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/__init__.py` & `scanpydoc-0.9.2/src/scanpydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.9.2/src/scanpydoc/autosummary_generate_imported.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.9.2/src/scanpydoc/definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 .. _sphinx issue 4826: https://github.com/sphinx-doc/sphinx/issues/4826
 .. _sphinx-autodoc-typehints issue 38: https://github.com/agronholm/sphinx-autodoc-typehints/issues/38
 
 """
 from __future__ import annotations
 
 from collections import ChainMap
+from collections.abc import Callable
+from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from typing import Any
 
 from docutils.parsers.rst import roles
 from sphinx.application import Sphinx
 from sphinx.config import Config
@@ -87,27 +89,34 @@
         )
     if config.typehints_defaults is None and config.annotate_defaults:
         # override default for “typehints_defaults”
         config.typehints_defaults = "braces"
     config.html_static_path.append(str(HERE / "static"))
 
 
+@dataclass
+class PickleableCallable:
+    func: Callable
+
+    __call__ = property(lambda self: self.func)
+
+
 @_setup_sig
 def setup(app: Sphinx) -> dict[str, Any]:
     """Patches :mod:`sphinx_autodoc_typehints` for a more elegant display."""
     # TODO: Unsure if “html” is sufficient or if we need to do “env”;
     #       Depends on when the autodoc-process-docstring event is handled.
     app.add_config_value("qualname_overrides", {}, "html")
     app.add_config_value("annotate_defaults", True, "html")
     app.add_css_file("typehints.css")
     app.connect("config-inited", _init_vars)
 
     from .formatting import _role_annot, format_annotation
 
-    app.config.typehints_formatter = format_annotation
+    app.config["typehints_formatter"] = PickleableCallable(format_annotation)
     for name in ["annotation-terse", "annotation-full"]:
         roles.register_canonical_role(
             name, partial(_role_annot, additional_classes=name.split("-"))
         )
 
     from .autodoc_patch import dir_head_adder
```

### Comparing `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/__init__.py` & `scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/rtd_github_links/_linkcode.py` & `scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/_linkcode.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/theme/__init__.py` & `scanpydoc-0.9.2/src/scanpydoc/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/theme/layout.html` & `scanpydoc-0.9.2/src/scanpydoc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/src/scanpydoc/theme/theme.conf` & `scanpydoc-0.9.2/src/scanpydoc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/tests/conftest.py` & `scanpydoc-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/tests/test_base.py` & `scanpydoc-0.9.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/tests/test_definition_list_typed_field.py` & `scanpydoc-0.9.2/tests/test_definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/tests/test_elegant_typehints.py` & `scanpydoc-0.9.2/tests/test_elegant_typehints.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/tests/test_rtd_github_links.py` & `scanpydoc-0.9.2/tests/test_rtd_github_links.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/LICENSE` & `scanpydoc-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/README.rst` & `scanpydoc-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/pyproject.toml` & `scanpydoc-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.1/PKG-INFO` & `scanpydoc-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.9.1
+Version: 0.9.2
 Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
 Project-URL: Source, https://github.com/theislab/scanpydoc/
 Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Author-email: Philipp Angerer <phil.angerer@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Sphinx :: Extension
```

