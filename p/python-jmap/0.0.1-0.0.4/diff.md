# Comparing `tmp/python_jmap-0.0.1.tar.gz` & `tmp/python_jmap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_jmap-0.0.1.tar", max compression
+gzip compressed data, was "python_jmap-0.0.4.tar", max compression
```

## Comparing `python_jmap-0.0.1.tar` & `python_jmap-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-07-08 21:38:23.639853 python_jmap-0.0.1/LICENSE
--rw-r--r--   0        0        0     2376 2023-07-08 21:38:23.639853 python_jmap-0.0.1/README.md
--rw-r--r--   0        0        0     1799 2023-07-08 21:38:38.951729 python_jmap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       28 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/__init__.py
--rw-r--r--   0        0        0      142 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/__main__.py
--rw-r--r--   0        0        0        0 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/py.typed
--rw-r--r--   0        0        0       34 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/types/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-08 21:38:23.639853 python_jmap-0.0.1/src/python_jmap/types/id.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 python_jmap-0.0.1/setup.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 python_jmap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-20 14:09:31.099972 python_jmap-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2376 2023-07-20 14:09:31.099972 python_jmap-0.0.4/README.md
+-rw-r--r--   0        0        0     1812 2023-07-20 14:09:53.451948 python_jmap-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/py.typed
+-rw-r--r--   0        0        0      221 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/types/__init__.py
+-rw-r--r--   0        0        0     2128 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/types/date.py
+-rw-r--r--   0        0        0     3739 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/types/id.py
+-rw-r--r--   0        0        0     2123 2023-07-20 14:09:31.103972 python_jmap-0.0.4/src/python_jmap/types/int.py
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 python_jmap-0.0.4/setup.py
+-rw-r--r--   0        0        0     3234 1970-01-01 00:00:00.000000 python_jmap-0.0.4/PKG-INFO
```

### Comparing `python_jmap-0.0.1/LICENSE` & `python_jmap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_jmap-0.0.1/README.md` & `python_jmap-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python_jmap-0.0.1/pyproject.toml` & `python_jmap-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-jmap"
-version = "0.0.1"
+version = "v0.0.4"
 description = "Python JMAP Bindings"
 authors = ["Josh Finch <josh@boop.email>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/boopmail/python-jmap"
 repository = "https://github.com/boopmail/python-jmap"
 documentation = "https://python-jmap.readthedocs.io"
@@ -12,15 +12,16 @@
     "Development Status :: 1 - Planning",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/boopmail/python-jmap/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
+pydantic = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -35,20 +36,20 @@
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
-sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 nox = "^2023.4.22"
 nox-poetry = "^1.0.2"
+flaky = "^3.7.0"
 
 [tool.poetry.scripts]
 python-jmap = "python_jmap.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `python_jmap-0.0.1/src/python_jmap/types/id.py` & `python_jmap-0.0.4/src/python_jmap/types/id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""JMAP Identifier type."""
+"""JMAP Identifier type.
+
+Spec: https://jmap.io/spec-core.html#the-id-data-type
+"""
 import re
 import secrets
 import string
 import warnings
 from typing import Optional
 from typing import Type
 
 
 class ID(str):
-    """JMAP Identifier type.
+    """Helper type for generating JMAP spec-compliant ID strings.
 
     Example:
     >>> id = ID("test_id")
     >>> print(id)
     test_id
     """
```

### Comparing `python_jmap-0.0.1/setup.py` & `python_jmap-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 
 packages = \
 ['python_jmap', 'python_jmap.types']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['pydantic>=2.0.2,<3.0.0']
+
 entry_points = \
 {'console_scripts': ['python-jmap = python_jmap.__main__:main']}
 
 setup_kwargs = {
     'name': 'python-jmap',
-    'version': '0.0.1',
+    'version': '0.0.4',
     'description': 'Python JMAP Bindings',
     'long_description': "# Python JMAP Bindings\n\n[![PyPI](https://img.shields.io/pypi/v/python-jmap.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/python-jmap.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/python-jmap)][pypi status]\n[![License](https://img.shields.io/pypi/l/python-jmap)][license]\n\n[![Read the documentation at https://python-jmap.readthedocs.io/](https://img.shields.io/readthedocs/python-jmap/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/boopmail/python-jmap/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/boopmail/python-jmap/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/python-jmap/\n[read the docs]: https://python-jmap.readthedocs.io/\n[tests]: https://github.com/boopmail/python-jmap/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/boopmail/python-jmap\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Python JMAP Bindings_ via [pip] from [PyPI]:\n\n```console\n$ pip install python-jmap\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Python JMAP Bindings_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/boopmail/python-jmap/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/boopmail/python-jmap/blob/main/LICENSE\n[contributor guide]: https://github.com/boopmail/python-jmap/blob/main/CONTRIBUTING.md\n[command-line reference]: https://python-jmap.readthedocs.io/en/latest/usage.html\n",
     'author': 'Josh Finch',
     'author_email': 'josh@boop.email',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/boopmail/python-jmap',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `python_jmap-0.0.1/PKG-INFO` & `python_jmap-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: python-jmap
-Version: 0.0.1
+Version: 0.0.4
 Summary: Python JMAP Bindings
 Home-page: https://github.com/boopmail/python-jmap
 License: MIT
 Author: Josh Finch
 Author-email: josh@boop.email
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Project-URL: Changelog, https://github.com/boopmail/python-jmap/releases
 Project-URL: Documentation, https://python-jmap.readthedocs.io
 Project-URL: Repository, https://github.com/boopmail/python-jmap
 Description-Content-Type: text/markdown
 
 # Python JMAP Bindings
```

