# Comparing `tmp/python_jmap-0.0.0.tar.gz` & `tmp/python_jmap-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_jmap-0.0.0.tar", max compression
+gzip compressed data, was "python_jmap-0.0.1.tar", max compression
```

## Comparing `python_jmap-0.0.0.tar` & `python_jmap-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-07-08 21:36:05.992688 python_jmap-0.0.0/LICENSE
--rw-r--r--   0        0        0     2376 2023-07-08 21:36:05.992688 python_jmap-0.0.0/README.md
--rw-r--r--   0        0        0     1799 2023-07-08 21:36:25.473817 python_jmap-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-07-08 21:36:05.992688 python_jmap-0.0.0/src/python_jmap/__init__.py
--rw-r--r--   0        0        0      142 2023-07-08 21:36:05.992688 python_jmap-0.0.0/src/python_jmap/__main__.py
--rw-r--r--   0        0        0        0 2023-07-08 21:36:05.992688 python_jmap-0.0.0/src/python_jmap/py.typed
--rw-r--r--   0        0        0       34 2023-07-08 21:36:05.992688 python_jmap-0.0.0/src/python_jmap/types/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-08 21:36:05.992688 python_jmap-0.0.0/src/python_jmap/types/id.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 python_jmap-0.0.0/setup.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 python_jmap-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-08 21:38:23.639853 python_jmap-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2376 2023-07-08 21:38:23.639853 python_jmap-0.0.1/README.md
+-rw-r--r--   0        0        0     1799 2023-07-08 21:38:38.951729 python_jmap-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/py.typed
+-rw-r--r--   0        0        0       34 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/types/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/types/id.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 python_jmap-0.0.1/setup.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 python_jmap-0.0.1/PKG-INFO
```

### Comparing `python_jmap-0.0.0/LICENSE` & `python_jmap-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_jmap-0.0.0/README.md` & `python_jmap-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_jmap-0.0.0/pyproject.toml` & `python_jmap-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-jmap"
-version = "0.0.0"
+version = "0.0.1"
 description = "Python JMAP Bindings"
 authors = ["Josh Finch <josh@boop.email>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/boopmail/python-jmap"
 repository = "https://github.com/boopmail/python-jmap"
 documentation = "https://python-jmap.readthedocs.io"
```

### Comparing `python_jmap-0.0.0/src/python_jmap/types/id.py` & `python_jmap-0.0.1/src/python_jmap/types/id.py`

 * *Files identical despite different names*

### Comparing `python_jmap-0.0.0/setup.py` & `python_jmap-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['python-jmap = python_jmap.__main__:main']}
 
 setup_kwargs = {
     'name': 'python-jmap',
-    'version': '0.0.0',
+    'version': '0.0.1',
     'description': 'Python JMAP Bindings',
     'long_description': "# Python JMAP Bindings\n\n[![PyPI](https://img.shields.io/pypi/v/python-jmap.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/python-jmap.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/python-jmap)][pypi status]\n[![License](https://img.shields.io/pypi/l/python-jmap)][license]\n\n[![Read the documentation at https://python-jmap.readthedocs.io/](https://img.shields.io/readthedocs/python-jmap/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/boopmail/python-jmap/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/boopmail/python-jmap/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/python-jmap/\n[read the docs]: https://python-jmap.readthedocs.io/\n[tests]: https://github.com/boopmail/python-jmap/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/boopmail/python-jmap\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Python JMAP Bindings_ via [pip] from [PyPI]:\n\n```console\n$ pip install python-jmap\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Python JMAP Bindings_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/boopmail/python-jmap/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/boopmail/python-jmap/blob/main/LICENSE\n[contributor guide]: https://github.com/boopmail/python-jmap/blob/main/CONTRIBUTING.md\n[command-line reference]: https://python-jmap.readthedocs.io/en/latest/usage.html\n",
     'author': 'Josh Finch',
     'author_email': 'josh@boop.email',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/boopmail/python-jmap',
```

### Comparing `python_jmap-0.0.0/PKG-INFO` & `python_jmap-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jmap
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python JMAP Bindings
 Home-page: https://github.com/boopmail/python-jmap
 License: MIT
 Author: Josh Finch
 Author-email: josh@boop.email
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

