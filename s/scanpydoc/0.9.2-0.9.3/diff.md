# Comparing `tmp/scanpydoc-0.9.2.tar.gz` & `tmp/scanpydoc-0.9.3.tar.gz`

## Comparing `scanpydoc-0.9.2.tar` & `scanpydoc-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.editorconfig
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.prettierrc.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.readthedocs.yml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.vscode/settings.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/_version.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/autosummary_generate_imported.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/definition_list_typed_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/py.typed
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/autodoc_patch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/example.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/formatting.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/return_tuple.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/static/typehints.css
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/_linkcode.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/layout.html
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/theme.conf
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/src/scanpydoc/theme/static/styles/scanpy.css
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_base.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_definition_list_typed_field.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_elegant_typehints.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/tests/test_rtd_github_links.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/.gitignore
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/README.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.editorconfig
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.prettierrc.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.readthedocs.yml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/conf.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/_version.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/autosummary_generate_imported.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/definition_list_typed_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/py.typed
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/autodoc_patch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/example.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/formatting.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/return_tuple.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/static/typehints.css
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/_linkcode.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/layout.html
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/theme.conf
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/src/scanpydoc/theme/static/styles/scanpy.css
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_base.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_definition_list_typed_field.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_elegant_typehints.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/tests/test_rtd_github_links.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/README.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 scanpydoc-0.9.3/PKG-INFO
```

### Comparing `scanpydoc-0.9.2/.pre-commit-config.yaml` & `scanpydoc-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/.github/workflows/ci.yml` & `scanpydoc-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/.github/workflows/publish.yml` & `scanpydoc-0.9.3/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
 
+env:
+  PIP_ROOT_USER_ACTION: ignore
+
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
```

### Comparing `scanpydoc-0.9.2/docs/conf.py` & `scanpydoc-0.9.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # Generate .rst stubs for modules using autosummary
 autosummary_generate = True
 autosummary_ignore_module_all = False
 # Don’t add module paths to documented functions’ names
 add_module_names = False
 
 html_theme = "scanpydoc"
-html_context = dict(
+html_theme_options = dict(
     repository_url="https://github.com/theislab/scanpydoc",
     repository_branch="main",
     use_repository_button=True,
 )
 
 rtd_links_prefix = PurePosixPath("src")
```

### Comparing `scanpydoc-0.9.2/docs/_templates/autosummary/module.rst` & `scanpydoc-0.9.3/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/__init__.py` & `scanpydoc-0.9.3/src/scanpydoc/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/autosummary_generate_imported.py` & `scanpydoc-0.9.3/src/scanpydoc/autosummary_generate_imported.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/definition_list_typed_field.py` & `scanpydoc-0.9.3/src/scanpydoc/definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/__init__.py` & `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/autodoc_patch.py` & `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/autodoc_patch.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/formatting.py` & `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/formatting.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/elegant_typehints/return_tuple.py` & `scanpydoc-0.9.3/src/scanpydoc/elegant_typehints/return_tuple.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/__init__.py` & `scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 -------------
 
 Uses the following config values in ``conf.py``::
 
     rtd_links_prefix: os.PathLike | str = ...  # default: '.'
 
     # sphinx book theme style
-    html_context = dict(
+    html_theme_options = dict(
         repository_url=...,
         repository_branch=...,
     )
     # or RTD theme style:
     html_context = dict(
         github_user=...,
         github_repo=...,
         github_version=...,
     )
 
 The ``rtd_links_prefix`` is for figuring out the .py file path relative to the git root,
 that is to construct the path in the GitHub URL.
 
-Which ``html_context`` style you want to use depends on your theme, e.g.
+Which html configuration style you want to use depends on your theme, e.g.
 :doc:`Sphinx Book Theme <sphinx_book_theme:index>`.
 
 ``:github_url:`` usage
 ----------------------
 
 You can use the filter e.g. in `autosummary templates`_.
 To configure the :doc:`Sphinx Book Theme <sphinx_book_theme:index>`,
@@ -75,22 +75,22 @@
 rtd_links_prefix: Path = None
 github_base_url: str = None
 
 
 def _init_vars(app: Sphinx, config: Config):
     """Called when ``conf.py`` has been loaded."""
     global github_base_url, rtd_links_prefix
-    _check_html_context(config)
+    _check_html_config(config)
     try:
         github_base_url = "https://github.com/{github_user}/{github_repo}/tree/{github_version}".format_map(
             config.html_context
         )
     except KeyError:
         github_base_url = "{repository_url}/tree/{repository_branch}".format_map(
-            config.html_context
+            config.html_theme_options
         )
     rtd_links_prefix = PurePosixPath(config.rtd_links_prefix)
 
 
 def _get_obj_module(qualname: str) -> tuple[Any, ModuleType]:
     """Get a module/class/attribute and its original module by qualname."""
     modname = qualname
@@ -149,47 +149,54 @@
 def github_url(qualname: str) -> str:
     """Get the full GitHub URL for some object’s qualname.
 
     Args:
         qualname: The full qualified name of a function, class, method or module
 
     Returns:
-        A GitHub URL derived from the :confval:`html_context`.
+        A GitHub URL derived from the :confval:`html_context`
+        or the :confval:`html_theme_options`.
     """
     try:
         obj, module = _get_obj_module(qualname)
     except Exception:
         print(f"Error in github_url({qualname!r}):", file=sys.stderr)
         raise
     path = rtd_links_prefix / _module_path(obj, module)
     start, end = _get_linenos(obj)
     fragment = f"#L{start}-L{end}" if start and end else ""
     return f"{github_base_url}/{path}{fragment}"
 
 
-def _check_html_context(config: Config):
-    try:
-        html_context: dict[str, Any] = config.html_context
-    except AttributeError:
-        raise ValueError(
-            f"Extension {__name__} needs “html_context” to be defined in conf.py"
-        )
-    options = [
-        {"github_user", "github_repo", "github_version"},
-        {"repository_url", "repository_branch"},
-    ]
-    missing_value_sets = [opt - html_context.keys() for opt in options]
-    if all(missing_value_sets):
-        mvs = " or ".join(
-            ", ".join(repr(mv) for mv in mvs) for mvs in missing_value_sets
-        )
-        raise ValueError(
-            f"Extension {__name__} needs html_context {mvs} to be defined in conf.py.\n"
-            f"html_context = {html_context!r}"
+def _check_html_config(config: Config):
+    options = dict(
+        html_context={"github_user", "github_repo", "github_version"},
+        html_theme_options={"repository_url", "repository_branch"},
+    )
+    if not any(name in config for name in options):
+        msg = (
+            f"Extension {__name__} needs “html_context” "
+            "or “html_theme_options” to be defined in conf.py"
         )
+        raise ValueError(msg)
+    missing_value_sets = {
+        name: opts - config[name].keys() for name, opts in options.items()
+    }
+    if not all(missing_value_sets.values()):
+        return  # a valid configuration was found
+
+    mvs = " or ".join(
+        f"{name} {', '.join(repr(mv) for mv in mvs)}"
+        for name, mvs in missing_value_sets.items()
+    )
+    msg = f"Extension {__name__} needs {mvs} to be defined in conf.py."
+    for name in options:
+        if name in config:
+            msg += f"\n{name} = {config[name]!r}"
+    raise ValueError(msg)
 
 
 @_setup_sig
 def setup(app: Sphinx) -> dict[str, Any]:
     """Register the :func:`github_url` :ref:`Jinja filter <jinja:filters>`."""
 
     app.add_config_value("rtd_links_prefix", PurePosixPath("."), "")
```

### Comparing `scanpydoc-0.9.2/src/scanpydoc/rtd_github_links/_linkcode.py` & `scanpydoc-0.9.3/src/scanpydoc/rtd_github_links/_linkcode.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/theme/__init__.py` & `scanpydoc-0.9.3/src/scanpydoc/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/theme/layout.html` & `scanpydoc-0.9.3/src/scanpydoc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/src/scanpydoc/theme/theme.conf` & `scanpydoc-0.9.3/src/scanpydoc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/tests/conftest.py` & `scanpydoc-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/tests/test_base.py` & `scanpydoc-0.9.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/tests/test_definition_list_typed_field.py` & `scanpydoc-0.9.3/tests/test_definition_list_typed_field.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/tests/test_elegant_typehints.py` & `scanpydoc-0.9.3/tests/test_elegant_typehints.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/tests/test_rtd_github_links.py` & `scanpydoc-0.9.3/tests/test_rtd_github_links.py`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/LICENSE` & `scanpydoc-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/README.rst` & `scanpydoc-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/pyproject.toml` & `scanpydoc-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scanpydoc-0.9.2/PKG-INFO` & `scanpydoc-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanpydoc
-Version: 0.9.2
+Version: 0.9.3
 Summary: A series of Sphinx extensions to get maintainable numpydoc style documentation.
 Project-URL: Source, https://github.com/theislab/scanpydoc/
 Project-URL: Documentation, https://icb-scanpydoc.readthedocs-hosted.com/
 Author-email: Philipp Angerer <phil.angerer@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Sphinx :: Extension
```

