# Comparing `tmp/async_interrupt-0.0.0.tar.gz` & `tmp/async_interrupt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_interrupt-0.0.0.tar", max compression
+gzip compressed data, was "async_interrupt-1.1.0.tar", max compression
```

## Comparing `async_interrupt-0.0.0.tar` & `async_interrupt-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0    11345 2023-07-20 02:42:01.363661 async_interrupt-0.0.0/LICENSE
--rw-r--r--   0        0        0     3355 2023-07-20 02:42:01.358508 async_interrupt-0.0.0/README.md
--rw-r--r--   0        0        0     1957 2023-07-20 02:42:01.382216 async_interrupt-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-20 02:42:01.385307 async_interrupt-0.0.0/src/async_interrupt/__init__.py
--rw-r--r--   0        0        0       53 2023-07-20 02:42:01.386498 async_interrupt-0.0.0/src/async_interrupt/main.py
--rw-r--r--   0        0        0        0 2023-07-20 02:42:01.385881 async_interrupt-0.0.0/src/async_interrupt/py.typed
--rw-r--r--   0        0        0     4080 1970-01-01 00:00:00.000000 async_interrupt-0.0.0/setup.py
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 async_interrupt-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/README.md
+-rw-r--r--   0        0        0     1957 2023-07-20 16:39:36.380228 async_interrupt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4245 2023-07-20 16:39:36.336228 async_interrupt-1.1.0/src/async_interrupt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/src/async_interrupt/py.typed
+-rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 async_interrupt-1.1.0/PKG-INFO
```

### Comparing `async_interrupt-0.0.0/LICENSE` & `async_interrupt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_interrupt-0.0.0/README.md` & `async_interrupt-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,30 @@
   <a href="https://pypi.org/project/async_interrupt/">
     <img src="https://img.shields.io/pypi/v/async_interrupt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
   <img src="https://img.shields.io/pypi/pyversions/async_interrupt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/async_interrupt.svg?style=flat-square" alt="License">
 </p>
 
-Context manager to raise an exception when a future is done
+Interrupt context manager for asyncio.
+
+This module provides a context manager that can be used to interrupt
+a block of code as soon as possible when a future is done.
+
+The purpose is to raise as soon as possible to avoid any race conditions.
+
+This is based loosely on async_timeout by Andrew Svetlov and cpython asyncio.timeout
+
+## Usage
+
+```python
+async with interrupt(future, ValueError, "message"):
+    future.set_result(None)
+    await asyncio.sleep(0)
+```
 
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install async_interrupt`
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
 # async_interrupt
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
-Context manager to raise an exception when a future is done ## Installation
-Install this via pip (or your favourite package manager): `pip install
-async_interrupt` ## Contributors â¨ Thanks goes to these wonderful people (
-[emoji key](https://allcontributors.org/docs/en/emoji-key)):       This project
-follows the [all-contributors](https://github.com/all-contributors/all-
+Interrupt context manager for asyncio. This module provides a context manager
+that can be used to interrupt a block of code as soon as possible when a future
+is done. The purpose is to raise as soon as possible to avoid any race
+conditions. This is based loosely on async_timeout by Andrew Svetlov and
+cpython asyncio.timeout ## Usage ```python async with interrupt(future,
+ValueError, "message"): future.set_result(None) await asyncio.sleep(0) ``` ##
+Installation Install this via pip (or your favourite package manager): `pip
+install async_interrupt` ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):       This
+project follows the [all-contributors](https://github.com/all-contributors/all-
 contributors) specification. Contributions of any kind welcome! ## Credits This
 package was created with [Copier](https://copier.readthedocs.io/) and the
 [browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
 template) project template.
```

### Comparing `async_interrupt-0.0.0/pyproject.toml` & `async_interrupt-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_interrupt"
-version = "0.0.0"
+version = "1.1.0"
 description = "Context manager to raise an exception when a future is done"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/async_interrupt"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `async_interrupt-0.0.0/setup.py` & `async_interrupt-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: async-interrupt
+Version: 1.1.0
+Summary: Context manager to raise an exception when a future is done
+Home-page: https://github.com/bdraco/async_interrupt
+License: Apache Software License 2.0
+Author: J. Nick Koston
+Author-email: nick@koston.org
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Project-URL: Bug Tracker, https://github.com/bdraco/async_interrupt/issues
+Project-URL: Changelog, https://github.com/bdraco/async_interrupt/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/bdraco/async_interrupt
+Description-Content-Type: text/markdown
+
+# async_interrupt
+
+<p align="center">
+  <a href="https://github.com/bdraco/async_interrupt/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/async_interrupt/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://codecov.io/gh/bdraco/async_interrupt">
+    <img src="https://img.shields.io/codecov/c/github/bdraco/async_interrupt.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/async_interrupt/">
+    <img src="https://img.shields.io/pypi/v/async_interrupt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/async_interrupt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/async_interrupt.svg?style=flat-square" alt="License">
+</p>
+
+Interrupt context manager for asyncio.
+
+This module provides a context manager that can be used to interrupt
+a block of code as soon as possible when a future is done.
+
+The purpose is to raise as soon as possible to avoid any race conditions.
+
+This is based loosely on async_timeout by Andrew Svetlov and cpython asyncio.timeout
+
+## Usage
+
+```python
+async with interrupt(future, ValueError, "message"):
+    future.set_result(None)
+    await asyncio.sleep(0)
+```
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install async_interrupt`
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-enable -->
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['async_interrupt']
-
-package_data = \
-{'': ['*']}
-
-setup_kwargs = {
-    'name': 'async-interrupt',
-    'version': '0.0.0',
-    'description': 'Context manager to raise an exception when a future is done',
-    'long_description': '# async_interrupt\n\n<p align="center">\n  <a href="https://github.com/bdraco/async_interrupt/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/async_interrupt/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/async_interrupt">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/async_interrupt.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/async_interrupt/">\n    <img src="https://img.shields.io/pypi/v/async_interrupt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/async_interrupt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/async_interrupt.svg?style=flat-square" alt="License">\n</p>\n\nContext manager to raise an exception when a future is done\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install async_interrupt`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-    'author': 'J. Nick Koston',
-    'author_email': 'nick@koston.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bdraco/async_interrupt',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,24 +1,32 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['async_interrupt'] package_data = \ {'': ['*']}
-setup_kwargs = { 'name': 'async-interrupt', 'version': '0.0.0', 'description':
-'Context manager to raise an exception when a future is done',
-'long_description': '# async_interrupt\n\n
-            \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nContext manager to raise an exception when a future is done\n\n##
-Installation\n\nInstall this via pip (or your favourite package manager):
-\n\n`pip install async_interrupt`\n\n## Contributors â¨\n\nThanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors](https://
-github.com/all-contributors/all-contributors) specification. Contributions of
-any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier]
-(https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template]
-(https://github.com/browniebroke/pypackage-template)\nproject template.\n',
-'author': 'J. Nick Koston', 'author_email': 'nick@koston.org', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/bdraco/
-async_interrupt', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: async-interrupt Version: 1.1.0 Summary: Context
+manager to raise an exception when a future is done Home-page: https://
+github.com/bdraco/async_interrupt License: Apache Software License 2.0 Author:
+J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: Other/Proprietary License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
+Libraries Project-URL: Bug Tracker, https://github.com/bdraco/async_interrupt/
+issues Project-URL: Changelog, https://github.com/bdraco/async_interrupt/blob/
+main/CHANGELOG.md Project-URL: Repository, https://github.com/bdraco/
+async_interrupt Description-Content-Type: text/markdown # async_interrupt
+                    [CI_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+Interrupt context manager for asyncio. This module provides a context manager
+that can be used to interrupt a block of code as soon as possible when a future
+is done. The purpose is to raise as soon as possible to avoid any race
+conditions. This is based loosely on async_timeout by Andrew Svetlov and
+cpython asyncio.timeout ## Usage ```python async with interrupt(future,
+ValueError, "message"): future.set_result(None) await asyncio.sleep(0) ``` ##
+Installation Install this via pip (or your favourite package manager): `pip
+install async_interrupt` ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):       This
+project follows the [all-contributors](https://github.com/all-contributors/all-
+contributors) specification. Contributions of any kind welcome! ## Credits This
+package was created with [Copier](https://copier.readthedocs.io/) and the
+[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
+template) project template.
```

