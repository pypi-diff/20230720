# Comparing `tmp/kyujipy-0.5.6.tar.gz` & `tmp/kyujipy-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyujipy-0.5.6.tar", max compression
+gzip compressed data, was "kyujipy-0.5.7.tar", max compression
```

## Comparing `kyujipy-0.5.6.tar` & `kyujipy-0.5.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2021-06-06 14:12:56.118715 kyujipy-0.5.6/LICENSE
--rw-r--r--   0        0        0     1510 2021-10-12 18:08:03.078100 kyujipy-0.5.6/README.md
--rw-r--r--   0        0        0       93 2021-10-12 18:01:10.757460 kyujipy-0.5.6/kyujipy/__init__.py
--rw-r--r--   0        0        0     6460 2020-09-02 20:34:44.773662 kyujipy-0.5.6/kyujipy/converter.py
--rw-r--r--   0        0        0      850 2019-03-05 09:37:48.285775 kyujipy-0.5.6/kyujipy/export_to_json.py
--rw-r--r--   0        0        0    16420 2021-06-06 15:35:32.741041 kyujipy-0.5.6/kyujipy/kakikae_simplified.cson
--rw-r--r--   0        0        0    25066 2021-06-06 15:35:32.749410 kyujipy-0.5.6/kyujipy/kakikae_variants.cson
--rw-r--r--   0        0        0     9740 2018-09-19 16:38:48.663323 kyujipy-0.5.6/kyujipy/kyujitai.cson
--rw-r--r--   0        0        0      591 2021-10-12 18:37:27.289355 kyujipy-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     2292 2021-10-12 18:37:41.402168 kyujipy-0.5.6/setup.py
--rw-r--r--   0        0        0     2185 2021-10-12 18:37:41.402543 kyujipy-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-11-14 00:57:05.859995 kyujipy-0.5.7/LICENSE
+-rw-r--r--   0        0        0     1510 2023-07-05 11:49:55.172738 kyujipy-0.5.7/README.md
+-rw-r--r--   0        0        0       93 2021-11-14 00:57:05.860195 kyujipy-0.5.7/kyujipy/__init__.py
+-rw-r--r--   0        0        0     6460 2021-11-14 00:57:05.860273 kyujipy-0.5.7/kyujipy/converter.py
+-rw-r--r--   0        0        0      850 2021-11-14 00:57:05.860338 kyujipy-0.5.7/kyujipy/export_to_json.py
+-rw-r--r--   0        0        0    16420 2021-11-14 00:57:05.860496 kyujipy-0.5.7/kyujipy/kakikae_simplified.cson
+-rw-r--r--   0        0        0    25066 2021-11-14 00:57:05.860575 kyujipy-0.5.7/kyujipy/kakikae_variants.cson
+-rw-r--r--   0        0        0     9740 2021-11-14 00:57:05.860670 kyujipy-0.5.7/kyujipy/kyujitai.cson
+-rw-r--r--   0        0        0      573 2023-07-20 17:30:07.766385 kyujipy-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 kyujipy-0.5.7/PKG-INFO
```

### Comparing `kyujipy-0.5.6/LICENSE` & `kyujipy-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/README.md` & `kyujipy-0.5.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 Convert a text from Kyūjitai (舊字體) to Shinjitai (新字体)
 
 
 ## License
 
 [kyujipy](https://github.com/DrTurnon/kyujipy) is licensed under the MIT license.
 
-© 2017-2021 [Emmanuel Ternon](https://github.com/DrTurnon)
+© 2017-2023 [Emmanuel Ternon](https://github.com/DrTurnon)
```

### Comparing `kyujipy-0.5.6/kyujipy/converter.py` & `kyujipy-0.5.7/kyujipy/converter.py`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/kyujipy/export_to_json.py` & `kyujipy-0.5.7/kyujipy/export_to_json.py`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/kyujipy/kakikae_simplified.cson` & `kyujipy-0.5.7/kyujipy/kakikae_simplified.cson`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/kyujipy/kakikae_variants.cson` & `kyujipy-0.5.7/kyujipy/kakikae_variants.cson`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/kyujipy/kyujitai.cson` & `kyujipy-0.5.7/kyujipy/kyujitai.cson`

 * *Files identical despite different names*

### Comparing `kyujipy-0.5.6/pyproject.toml` & `kyujipy-0.5.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "kyujipy"
-version = "0.5.6"
+version = "0.5.7"
 description = "A Python library to convert Japanese texts from Shinjitai to Kyujitai and vice versa"
 authors = ["Emmanuel Ternon <emmanuel.ternon@outlook.com>"]
 license="MIT"
 readme = "README.md"
 homepage = "https://github.com/DrTurnon/kyujipy"
 repository = "https://github.com/DrTurnon/kyujipy"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 cson = "^0.8"
-poetry = "^1.1.11"
 
 [tool.poetry.dev-dependencies]
 nose = "^1.3.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kyujipy-0.5.6/setup.py` & `kyujipy-0.5.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kyujipy
+Version: 0.5.7
+Summary: A Python library to convert Japanese texts from Shinjitai to Kyujitai and vice versa
+Home-page: https://github.com/DrTurnon/kyujipy
+License: MIT
+Author: Emmanuel Ternon
+Author-email: emmanuel.ternon@outlook.com
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cson (>=0.8,<0.9)
+Project-URL: Repository, https://github.com/DrTurnon/kyujipy
+Description-Content-Type: text/markdown
 
-packages = \
-['kyujipy']
+# kyujipy
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/kyujipy.svg)](https://badge.fury.io/py/kyujipy)
 
-install_requires = \
-['cson>=0.8,<0.9', 'poetry>=1.1.11,<2.0.0']
-
-setup_kwargs = {
-    'name': 'kyujipy',
-    'version': '0.5.6',
-    'description': 'A Python library to convert Japanese texts from Shinjitai to Kyujitai and vice versa',
-    'long_description': '# kyujipy\n\n[![PyPI version](https://badge.fury.io/py/kyujipy.svg)](https://badge.fury.io/py/kyujipy)\n\n[kyujipy](https://github.com/DrTurnon/kyujipy) is a  Python library to convert Japanese texts from\n[Shinjitai](https://en.wikipedia.org/wiki/Shinjitai) (新字体) to\n[Kyūjitai](https://en.wikipedia.org/wiki/Ky%C5%ABjitai), (舊字體) and vice versa.\n\n[kyujipy](https://github.com/DrTurnon/kyujipy) is based on the\n[kyujitai.js](https://github.com/hakatashi/kyujitai.js) project, originally authored by\n[Koki Takahashi](https://github.com/hakatashi).\n\n\n## Installation (via [Pip](http://www.pip-installer.org/))\n\n    $ pip install kyujipy\n\n\n## Usage\n\nIn Python shell (or inside Python script):\n\n    \n    # Import main class\n    >>> from kyujipy import KyujitaiConverter\n    \n    # Instantiate Shinjitai <-> Kyujitai converter\n    >>> converter = KyujitaiConverter()\n    \n    # Convert a text from Shinjitai to Kyujitai\n    >>> print(converter.shinjitai_to_kyujitai("新字体"))\n    新字體\n    \n    # Convert a text from Kyujitai to Shinjitai\n    >>> print(converter.kyujitai_to_shinjitai("舊字體"))\n    旧字体\n\n\n## API Reference\n\n* __shinjitai_to_kyujitai(string)__\n\nConvert a text from Shinjitai (新字体) to Kyūjitai (舊字體)\n\n* __kyujitai_to_shinjitai(string)__\n\nConvert a text from Kyūjitai (舊字體) to Shinjitai (新字体)\n\n\n## License\n\n[kyujipy](https://github.com/DrTurnon/kyujipy) is licensed under the MIT license.\n\n© 2017-2021 [Emmanuel Ternon](https://github.com/DrTurnon)\n',
-    'author': 'Emmanuel Ternon',
-    'author_email': 'emmanuel.ternon@outlook.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/DrTurnon/kyujipy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+[kyujipy](https://github.com/DrTurnon/kyujipy) is a  Python library to convert Japanese texts from
+[Shinjitai](https://en.wikipedia.org/wiki/Shinjitai) (新字体) to
+[Kyūjitai](https://en.wikipedia.org/wiki/Ky%C5%ABjitai), (舊字體) and vice versa.
 
+[kyujipy](https://github.com/DrTurnon/kyujipy) is based on the
+[kyujitai.js](https://github.com/hakatashi/kyujitai.js) project, originally authored by
+[Koki Takahashi](https://github.com/hakatashi).
+
+
+## Installation (via [Pip](http://www.pip-installer.org/))
+
+    $ pip install kyujipy
+
+
+## Usage
+
+In Python shell (or inside Python script):
+
+    
+    # Import main class
+    >>> from kyujipy import KyujitaiConverter
+    
+    # Instantiate Shinjitai <-> Kyujitai converter
+    >>> converter = KyujitaiConverter()
+    
+    # Convert a text from Shinjitai to Kyujitai
+    >>> print(converter.shinjitai_to_kyujitai("新字体"))
+    新字體
+    
+    # Convert a text from Kyujitai to Shinjitai
+    >>> print(converter.kyujitai_to_shinjitai("舊字體"))
+    旧字体
+
+
+## API Reference
+
+* __shinjitai_to_kyujitai(string)__
+
+Convert a text from Shinjitai (新字体) to Kyūjitai (舊字體)
+
+* __kyujitai_to_shinjitai(string)__
+
+Convert a text from Kyūjitai (舊字體) to Shinjitai (新字体)
+
+
+## License
+
+[kyujipy](https://github.com/DrTurnon/kyujipy) is licensed under the MIT license.
+
+© 2017-2023 [Emmanuel Ternon](https://github.com/DrTurnon)
 
-setup(**setup_kwargs)
```

