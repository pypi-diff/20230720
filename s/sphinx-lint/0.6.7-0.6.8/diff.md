# Comparing `tmp/sphinx-lint-0.6.7.tar.gz` & `tmp/sphinx-lint-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-lint-0.6.7.tar", last modified: Tue Oct 18 14:23:04 2022, max compression
+gzip compressed data, was "sphinx-lint-0.6.8.tar", last modified: Thu Jul 20 15:39:32 2023, max compression
```

## Comparing `sphinx-lint-0.6.7.tar` & `sphinx-lint-0.6.8.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-10-18 14:23:04.859121 sphinx-lint-0.6.7/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2490 2022-01-24 14:27:56.000000 sphinx-lint-0.6.7/LICENSE
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3064 2022-10-18 14:23:04.859121 sphinx-lint-0.6.7/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2344 2022-10-06 23:21:15.000000 sphinx-lint-0.6.7/README.md
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1116 2022-10-18 10:07:29.000000 sphinx-lint-0.6.7/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2022-10-18 14:23:04.859121 sphinx-lint-0.6.7/setup.cfg
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-10-18 14:23:04.859121 sphinx-lint-0.6.7/sphinx_lint.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3064 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      258 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       48 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       12 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       11 2022-10-18 14:23:04.000000 sphinx-lint-0.6.7/sphinx_lint.egg-info/top_level.txt
--rwxr-xr-x   0 mdk       (1000) mdk       (1000)    39725 2022-10-18 14:20:57.000000 sphinx-lint-0.6.7/sphinxlint.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-20 15:39:32.549997 sphinx-lint-0.6.8/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2490 2022-01-24 14:27:56.000000 sphinx-lint-0.6.8/LICENSE
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4120 2023-07-20 15:39:32.545997 sphinx-lint-0.6.8/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3400 2023-07-19 20:35:50.000000 sphinx-lint-0.6.8/README.md
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1123 2022-11-06 20:19:43.000000 sphinx-lint-0.6.8/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-07-20 15:39:32.549997 sphinx-lint-0.6.8/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-20 15:39:32.545997 sphinx-lint-0.6.8/sphinx_lint.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4120 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      542 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       57 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       12 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       11 2023-07-20 15:39:32.000000 sphinx-lint-0.6.8/sphinx_lint.egg-info/top_level.txt
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-20 15:39:32.545997 sphinx-lint-0.6.8/sphinxlint/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      142 2023-07-20 15:38:09.000000 sphinx-lint-0.6.8/sphinxlint/__init__.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7265 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/sphinxlint/__main__.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16723 2023-07-20 15:38:00.000000 sphinx-lint-0.6.8/sphinxlint/checkers.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10811 2023-07-20 15:38:00.000000 sphinx-lint-0.6.8/sphinxlint/rst.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1967 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/sphinxlint/sphinxlint.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6894 2022-11-28 15:41:40.000000 sphinx-lint-0.6.8/sphinxlint/utils.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-20 15:39:32.545997 sphinx-lint-0.6.8/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      726 2022-11-06 20:19:43.000000 sphinx-lint-0.6.8/tests/test_default_role_re.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2368 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/tests/test_enable_disable.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7945 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/tests/test_filter_out_literal.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      383 2022-11-06 20:19:43.000000 sphinx-lint-0.6.8/tests/test_po2rst.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3253 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/tests/test_sphinxlint.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      764 2023-07-20 15:37:59.000000 sphinx-lint-0.6.8/tests/test_xpass_friends.py
```

### Comparing `sphinx-lint-0.6.7/LICENSE` & `sphinx-lint-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-lint-0.6.7/PKG-INFO` & `sphinx-lint-0.6.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: sphinx-lint
-Version: 0.6.7
-Summary: Check for stylistic and formal issues in .rst and .py files included in the documentation.
-Author-email: Georg Brandl <georg@python.org>, Julien Palard <julien@palard.fr>
-License: PSF License
-Project-URL: repository, https://github.com/sphinx-contrib/sphinx-lint
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Documentation :: Sphinx
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Sphinx Lint
 
 [![PyPI](https://img.shields.io/pypi/v/sphinx-lint)
  ![Monthly downloads](https://img.shields.io/pypi/dm/sphinx-lint)
  ![Supported Python Version](https://img.shields.io/pypi/pyversions/sphinx-lint.svg)
 ](https://pypi.org/project/sphinx-lint)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sphinx-contrib/sphinx-lint/Tests/main)](https://github.com/sphinx-contrib/sphinx-lint/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/sphinx-contrib/sphinx-lint/tests.yml?branch=main)](https://github.com/sphinx-contrib/sphinx-lint/actions)
 
 Sphinx Lint is based on [rstlint.py from
 CPython](https://github.com/python/cpython/blob/e0433c1e7/Doc/tools/rstlint.py).
 
 
 ## What is Sphinx Lint, what is it not?
 
@@ -53,14 +36,49 @@
 ```
 
 as Sphinx Lint works line by line it will inevitably think the `:meth:` role is not closed properly.
 
 To avoid false positives, some rules are skipped if we're in a table.
 
 
+## Contributing
+
+A quick way to test if some syntax is valid from a pure
+reStructuredText point of view, one case use `docutils`'s `pseudoxml`
+writer, like:
+
+```text
+$ docutils --writer=pseudoxml tests/fixtures/xpass/role-in-code-sample.rst
+<document source="tests/fixtures/xpass/role-in-code-sample.rst">
+    <paragraph>
+        Found in the pandas documentation, this is valid:
+    <bullet_list bullet="*">
+        <list_item>
+            <paragraph>
+                A pandas class (in the form
+                <literal>
+                    :class:`pandas.Series`
+                )
+        <list_item>
+            <paragraph>
+                A pandas method (in the form
+                <literal>
+                    :meth:`pandas.Series.sum`
+                )
+        <list_item>
+            <paragraph>
+                A pandas function (in the form
+                <literal>
+                    :func:`pandas.to_datetime`
+                )
+    <paragraph>
+        it's documenting roles using code samples (double backticks).
+```
+
+
 ## Releasing
 
 First test with friends projects by running:
 
     sh download-more-tests.sh
     python -m pytest
```

### Comparing `sphinx-lint-0.6.7/pyproject.toml` & `sphinx-lint-0.6.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 dynamic = ["version"]
 
 
 [project.urls]
 repository = "https://github.com/sphinx-contrib/sphinx-lint"
 
 [project.scripts]
-sphinx-lint = "sphinxlint:main"
+sphinx-lint = "sphinxlint.__main__:main"
 
 [tool.setuptools]
-py-modules = ["sphinxlint"]
+packages = ["sphinxlint"]
 include-package-data = false
 dynamic.version.attr = "sphinxlint.__version__"
 
 [tool.black]
 
 [tool.pylint.variables]
 callbacks = ["check_"]
```

### Comparing `sphinx-lint-0.6.7/sphinx_lint.egg-info/PKG-INFO` & `sphinx-lint-0.6.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-lint
-Version: 0.6.7
+Version: 0.6.8
 Summary: Check for stylistic and formal issues in .rst and .py files included in the documentation.
 Author-email: Georg Brandl <georg@python.org>, Julien Palard <julien@palard.fr>
 License: PSF License
 Project-URL: repository, https://github.com/sphinx-contrib/sphinx-lint
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 
 # Sphinx Lint
 
 [![PyPI](https://img.shields.io/pypi/v/sphinx-lint)
  ![Monthly downloads](https://img.shields.io/pypi/dm/sphinx-lint)
  ![Supported Python Version](https://img.shields.io/pypi/pyversions/sphinx-lint.svg)
 ](https://pypi.org/project/sphinx-lint)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sphinx-contrib/sphinx-lint/Tests/main)](https://github.com/sphinx-contrib/sphinx-lint/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/sphinx-contrib/sphinx-lint/tests.yml?branch=main)](https://github.com/sphinx-contrib/sphinx-lint/actions)
 
 Sphinx Lint is based on [rstlint.py from
 CPython](https://github.com/python/cpython/blob/e0433c1e7/Doc/tools/rstlint.py).
 
 
 ## What is Sphinx Lint, what is it not?
 
@@ -53,14 +53,49 @@
 ```
 
 as Sphinx Lint works line by line it will inevitably think the `:meth:` role is not closed properly.
 
 To avoid false positives, some rules are skipped if we're in a table.
 
 
+## Contributing
+
+A quick way to test if some syntax is valid from a pure
+reStructuredText point of view, one case use `docutils`'s `pseudoxml`
+writer, like:
+
+```text
+$ docutils --writer=pseudoxml tests/fixtures/xpass/role-in-code-sample.rst
+<document source="tests/fixtures/xpass/role-in-code-sample.rst">
+    <paragraph>
+        Found in the pandas documentation, this is valid:
+    <bullet_list bullet="*">
+        <list_item>
+            <paragraph>
+                A pandas class (in the form
+                <literal>
+                    :class:`pandas.Series`
+                )
+        <list_item>
+            <paragraph>
+                A pandas method (in the form
+                <literal>
+                    :meth:`pandas.Series.sum`
+                )
+        <list_item>
+            <paragraph>
+                A pandas function (in the form
+                <literal>
+                    :func:`pandas.to_datetime`
+                )
+    <paragraph>
+        it's documenting roles using code samples (double backticks).
+```
+
+
 ## Releasing
 
 First test with friends projects by running:
 
     sh download-more-tests.sh
     python -m pytest
```

