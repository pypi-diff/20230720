# Comparing `tmp/laskea-2023.6.18.tar.gz` & `tmp/laskea-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laskea-2023.6.18.tar", last modified: Sun Jun 18 13:22:48 2023, max compression
+gzip compressed data, was "laskea-2023.7.20.tar", last modified: Thu Jul 20 20:32:08 2023, max compression
```

## Comparing `laskea-2023.6.18.tar` & `laskea-2023.7.20.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.607404 laskea-2023.6.18/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 laskea-2023.6.18/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 laskea-2023.6.18/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3138 2023-06-18 13:22:48.607265 laskea-2023.6.18/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2083 2023-03-14 22:26:03.000000 laskea-2023.6.18/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.602380 laskea-2023.6.18/laskea/
--rw-r--r--   0 ruth       (501) staff       (20)     3844 2023-06-18 13:20:46.000000 laskea-2023.6.18/laskea/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      149 2022-07-09 20:48:21.000000 laskea-2023.6.18/laskea/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     8660 2022-11-08 15:35:37.000000 laskea-2023.6.18/laskea/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    14211 2022-11-07 22:13:00.000000 laskea-2023.6.18/laskea/config.py
--rw-r--r--   0 ruth       (501) staff       (20)     5241 2022-11-06 18:21:02.000000 laskea-2023.6.18/laskea/embed.py
--rw-r--r--   0 ruth       (501) staff       (20)     1950 2022-03-07 18:40:17.000000 laskea-2023.6.18/laskea/env.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2022-03-09 16:17:00.000000 laskea-2023.6.18/laskea/laskea.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.604638 laskea-2023.6.18/laskea.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3138 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      449 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      249 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        7 2023-06-18 13:22:48.000000 laskea-2023.6.18/laskea.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2865 2023-06-18 13:01:25.000000 laskea-2023.6.18/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 13:22:48.607440 laskea-2023.6.18/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 13:22:48.607091 laskea-2023.6.18/test/
--rw-r--r--   0 ruth       (501) staff       (20)     5717 2022-11-08 15:35:47.000000 laskea-2023.6.18/test/test_api.py
--rw-r--r--   0 ruth       (501) staff       (20)     5484 2022-11-03 16:33:55.000000 laskea-2023.6.18/test/test_cfg.py
--rw-r--r--   0 ruth       (501) staff       (20)     1092 2022-11-08 14:54:36.000000 laskea-2023.6.18/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     8473 2022-11-08 16:29:50.000000 laskea-2023.6.18/test/test_embed.py
--rw-r--r--   0 ruth       (501) staff       (20)      162 2022-03-05 17:53:30.000000 laskea-2023.6.18/test/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)      679 2022-03-05 17:51:41.000000 laskea-2023.6.18/test/test_laskea.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-07-20 20:32:08.976057 laskea-2023.7.20/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 laskea-2023.7.20/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 laskea-2023.7.20/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3280 2023-07-20 20:32:08.975922 laskea-2023.7.20/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2225 2023-07-01 17:02:39.000000 laskea-2023.7.20/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-07-20 20:32:08.971164 laskea-2023.7.20/laskea/
+-rw-r--r--   0 ruth       (501) staff       (20)     3890 2023-07-20 20:30:47.000000 laskea-2023.7.20/laskea/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      149 2022-07-09 20:48:21.000000 laskea-2023.7.20/laskea/__main__.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-07-20 20:32:08.973696 laskea-2023.7.20/laskea/api/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-26 20:23:00.000000 laskea-2023.7.20/laskea/api/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3260 2022-09-21 18:11:48.000000 laskea-2023.7.20/laskea/api/excel.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16845 2023-07-20 20:16:03.000000 laskea-2023.7.20/laskea/api/jira.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6169 2023-06-18 13:19:59.000000 laskea-2023.7.20/laskea/api/tabulator.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8660 2022-11-08 15:35:37.000000 laskea-2023.7.20/laskea/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14211 2022-11-07 22:13:00.000000 laskea-2023.7.20/laskea/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5319 2023-07-20 20:12:02.000000 laskea-2023.7.20/laskea/embed.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1950 2022-03-07 18:40:17.000000 laskea-2023.7.20/laskea/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2022-03-09 16:17:00.000000 laskea-2023.7.20/laskea/laskea.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-07-20 20:32:08.972473 laskea-2023.7.20/laskea.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3280 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      535 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      250 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        7 2023-07-20 20:32:08.000000 laskea-2023.7.20/laskea.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2880 2023-07-20 20:21:43.000000 laskea-2023.7.20/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-07-20 20:32:08.976090 laskea-2023.7.20/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-07-20 20:32:08.975752 laskea-2023.7.20/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     5717 2022-11-08 15:35:47.000000 laskea-2023.7.20/test/test_api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5484 2022-11-03 16:33:55.000000 laskea-2023.7.20/test/test_cfg.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1092 2022-11-08 14:54:36.000000 laskea-2023.7.20/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8473 2022-11-08 16:29:50.000000 laskea-2023.7.20/test/test_embed.py
+-rw-r--r--   0 ruth       (501) staff       (20)      162 2022-03-05 17:53:30.000000 laskea-2023.7.20/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)      679 2022-03-05 17:51:41.000000 laskea-2023.7.20/test/test_laskea.py
```

### Comparing `laskea-2023.6.18/LICENSE` & `laskea-2023.7.20/LICENSE`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/PKG-INFO` & `laskea-2023.7.20/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laskea
-Version: 2023.6.18
+Version: 2023.7.20
 Summary: Calculate (Finnish: laskea) some parts.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/laskea
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/laskea
 Project-URL: Documentation, https://codes.dilettant.life/docs/laskea
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/laskea
@@ -31,14 +31,15 @@
 Third party dependencies are documented in the folder [docs/third-party](docs/docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![downloads](https://pepy.tech/badge/laskea/month)](https://pepy.tech/project/laskea)
 [![wheel](https://img.shields.io/pypi/wheel/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
+[![maintenance-status](https://img.shields.io/github/commit-activity/y/sthagen/laskea.svg?style=flat)](https://git.sr.ht/~sthagen/laskea/log)
 
 ## Documentation
 
 User and developer [documentation of laskea](https://codes.dilettant.life/docs/laskea).
 
 ## Bug Tracker
```

### Comparing `laskea-2023.6.18/laskea/__init__.py` & `laskea-2023.7.20/laskea/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """Calculate (Finnish: laskea) some parts."""
 import os
+import pathlib
 
 # [[[fill git_describe()]]]
-__version__ = '2023.6.18+parent.e984ef8f'
-# [[[end]]] (checksum: acaf14066cd24e0140e2bfe3687a469c)
+__version__ = '2023.7.20+parent.g8bf4f662'
+# [[[end]]] (checksum: c1f0dbc200580a462e0e8b732a2ab333)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
-APP_NAME = 'Calculate (Finnish: laskea) some parts.'
-APP_ALIAS = 'laskea'
-APP_ENV = 'LASKEA'
+APP_ALIAS = str(pathlib.Path(__file__).parent.name)
+APP_ENV: str = APP_ALIAS.upper()
+APP_NAME = locals()['__doc__']
+DEBUG = bool(os.getenv(f'{APP_ENV}_DEBUG', ''))
+VERBOSE = bool(os.getenv(f'{APP_ENV}_VERBOSE', ''))
+QUIET = False
+STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
+ENCODING = 'utf-8'
+ENCODING_ERRORS_POLICY = 'ignore'
+DEFAULT_CONFIG_NAME = f'.{APP_ALIAS}.json'
+
 CACHE_EXPIRY_SECONDS = int(os.getenv(f'{APP_ENV}_CACHE_EXPIRY_SECONDS', '180'))
 REQUESTS_TIMEOUT_SECS = 30
 
 FIELD_SEPARATORS = (
     CARET := '^',
     COLON := ':',
     COMMA := ',',
@@ -26,22 +35,15 @@
     SEMI := ';',
     SPACE := ' ',
     TAB := '\t',
     USCORE := '_',
 )
 FS_SLUG = '$FIELD_SEPARATOR$'
 
-DEBUG = bool(os.getenv(f'{APP_ENV}_DEBUG', ''))
 DRY_RUN = False
-VERBOSE = bool(os.getenv(f'{APP_ENV}_VERBOSE', ''))
-QUIET = False
-STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
-ENCODING = 'utf-8'
-ENCODING_ERRORS_POLICY = 'ignore'
-DEFAULT_CONFIG_NAME = '.laskea.json'
 OPEN_BRACKET = '['
 CLOSE_BRACKET = ']'
 DEFAULT_MARKERS = f'{OPEN_BRACKET * 3}fill {CLOSE_BRACKET * 3} {OPEN_BRACKET * 3}end{CLOSE_BRACKET * 3}'
 DEFAULT_LF_ONLY = 'YES'
 DEFAULT_JOIN_STRING = ' <br>'
 BASE_MARKERS = os.getenv(f'{APP_ENV}_MARKERS', DEFAULT_MARKERS)
 BASE_LF_ONLY = bool(os.getenv(f'{APP_ENV}_LF_ONLY', DEFAULT_LF_ONLY))
```

### Comparing `laskea-2023.6.18/laskea/cli.py` & `laskea-2023.7.20/laskea/cli.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/laskea/config.py` & `laskea-2023.7.20/laskea/config.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/laskea/embed.py` & `laskea-2023.7.20/laskea/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,23 @@
             api.separated_values_list(
                 DB['handle'], query_text, key_magic=key_magic, field_sep=field_sep, replacement=replacement, data=data
             )
         )
 
 
 @no_type_check
-def table(query_text: str = '', data=None) -> None:
+def table(query_text: str = '', column_fields=None, data=None) -> None:
     """Public document interface."""
     if data is None:
         if not DB.get('handle', None):
             DB['handle'] = api.login()
 
-        print(api.markdown_table(DB['handle'], query_text))
+        print(api.markdown_table(DB['handle'], query_text, column_fields=column_fields))
     else:
-        print(api.markdown_table(DB['handle'], query_text, data=data))
+        print(api.markdown_table(DB['handle'], query_text, column_fields=column_fields, data=data))
 
 
 @no_type_check
 def dl(query_text: str = '', data=None) -> None:
     """Public document interface for definition list."""
     if data is None:
         if not DB.get('handle', None):
```

### Comparing `laskea-2023.6.18/laskea/env.py` & `laskea-2023.7.20/laskea/env.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/laskea/laskea.py` & `laskea-2023.7.20/laskea/laskea.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/laskea.egg-info/PKG-INFO` & `laskea-2023.7.20/laskea.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laskea
-Version: 2023.6.18
+Version: 2023.7.20
 Summary: Calculate (Finnish: laskea) some parts.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/laskea
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/laskea
 Project-URL: Documentation, https://codes.dilettant.life/docs/laskea
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/laskea
@@ -31,14 +31,15 @@
 Third party dependencies are documented in the folder [docs/third-party](docs/docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![downloads](https://pepy.tech/badge/laskea/month)](https://pepy.tech/project/laskea)
 [![wheel](https://img.shields.io/pypi/wheel/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/laskea.svg?style=flat)](https://pypi.python.org/pypi/laskea/)
+[![maintenance-status](https://img.shields.io/github/commit-activity/y/sthagen/laskea.svg?style=flat)](https://git.sr.ht/~sthagen/laskea/log)
 
 ## Documentation
 
 User and developer [documentation of laskea](https://codes.dilettant.life/docs/laskea).
 
 ## Bug Tracker
```

### Comparing `laskea-2023.6.18/pyproject.toml` & `laskea-2023.7.20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laskea"
-version = "2023.6.18"
+version = "2023.7.20"
 description = "Calculate (Finnish: laskea) some parts."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -21,16 +21,16 @@
 keywords = ["code-generation", "developer-tools", "markdown", "validation", "erification"]
 dependencies = [
     "atlassian-python-api >= 3.39.0",
     "cogapp >= 3.3.0",
     "defusedxml >= 0.7.1",
     "jmespath >= 1.0.1",
     "openpyxl >= 3.1.2",
-    "pydantic >= 1.10.9",
-    "requests-cache >= 1.0.1",
+    "pydantic >= 1.10.10",
+    "requests-cache >= 1.1.0",
     "scooby >= 0.7.2",
     "typer >= 0.9.0",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff", "types-jmespath"]
@@ -42,15 +42,15 @@
 Source-Code = "https://git.sr.ht/~sthagen/laskea"
 Test-Coverage = "https://codes.dilettant.life/coverage/laskea"
 
 [project.scripts]
 laskea = "laskea.cli:app"
 
 [tool.setuptools.packages.find]
-include = ["laskea"]
+include = ["laskea", "laskea.api"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ["py39", "py310", "py311", "py312"]
 
@@ -91,15 +91,15 @@
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-target-version = "py310"
+target-version = "py311"
 unfixable = ["F401"]
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "single"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `laskea-2023.6.18/test/test_api.py` & `laskea-2023.7.20/test/test_api.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/test/test_cfg.py` & `laskea-2023.7.20/test/test_cfg.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/test/test_cli.py` & `laskea-2023.7.20/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/test/test_embed.py` & `laskea-2023.7.20/test/test_embed.py`

 * *Files identical despite different names*

### Comparing `laskea-2023.6.18/test/test_laskea.py` & `laskea-2023.7.20/test/test_laskea.py`

 * *Files identical despite different names*

