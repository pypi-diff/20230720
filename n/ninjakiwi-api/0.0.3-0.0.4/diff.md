# Comparing `tmp/ninjakiwi_api-0.0.3.tar.gz` & `tmp/ninjakiwi_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.3.tar", max compression
+gzip compressed data, was "ninjakiwi_api-0.0.4.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.3.tar` & `ninjakiwi_api-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.3/LICENSE
--rw-r--r--   0        0        0      229 2023-07-20 10:17:22.489408 ninjakiwi_api-0.0.3/README.md
--rw-r--r--   0        0        0       83 2023-07-19 19:59:45.011619 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     2995 2023-07-19 21:02:28.521583 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       84 2023-07-19 20:22:35.650851 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1083 2023-07-19 21:46:09.966399 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      149 2023-07-19 20:22:35.654184 ninjakiwi_api-0.0.3/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0      116 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0      108 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      489 2023-07-20 10:45:03.488833 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0      135 2023-07-20 10:45:23.342612 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      223 2023-07-20 10:44:10.497649 ninjakiwi_api-0.0.3/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0     2830 2023-07-20 10:44:10.477649 ninjakiwi_api-0.0.3/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2641 2023-07-20 10:45:40.236325 ninjakiwi_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      526 2023-07-19 21:43:29.909004 ninjakiwi_api-0.0.3/tests/test_main.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.4/LICENSE
+-rw-r--r--   0        0        0      229 2023-07-20 10:17:22.489408 ninjakiwi_api-0.0.4/README.md
+-rw-r--r--   0        0        0       83 2023-07-19 19:59:45.011619 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     2995 2023-07-19 21:02:28.521583 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       84 2023-07-19 20:22:35.650851 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-19 21:46:09.966399 ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      149 2023-07-19 20:22:35.654184 ninjakiwi_api-0.0.4/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-20 10:45:03.488833 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0      135 2023-07-20 10:45:23.342612 ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-20 10:44:10.497649 ninjakiwi_api-0.0.4/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     2830 2023-07-20 10:44:10.477649 ninjakiwi_api-0.0.4/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2756 2023-07-20 10:59:27.412142 ninjakiwi_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-19 21:43:29.909004 ninjakiwi_api-0.0.4/tests/test_main.py
+-rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.4/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.3/LICENSE` & `ninjakiwi_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-0.0.4/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-0.0.4/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/ninjakiwi_api/main.py` & `ninjakiwi_api-0.0.4/ninjakiwi_api/main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/pyproject.toml` & `ninjakiwi_api-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.3"
+version = "0.0.4"
 homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
-description = "Skeleton project created by Python Project Wizard (ppw)."
-authors = ["Gustavo Schip <gustavoschip@proton.me>"]
+description = "NinjaKiwi API (OpenDATA) for Python! (My first library)"
+authors = [
+    "Gustavo Schip <gustavoschip@proton.me>",
+]
+maintainers = [
+    "Gustavo Schip <gustavoschip@proton.me>",
+]
 readme = "README.md"
 license =  "MIT"
-classifiers=[
+classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3.11',
 ]
+keywords = [
+    "NinjaKiwi",
+    "API",
+]
 packages = [
     { include = "ninjakiwi_api" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0.0"
```

### Comparing `ninjakiwi_api-0.0.3/tests/test_main.py` & `ninjakiwi_api-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.3/PKG-INFO` & `ninjakiwi_api-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 0.0.3
-Summary: Skeleton project created by Python Project Wizard (ppw).
+Version: 0.0.4
+Summary: NinjaKiwi API (OpenDATA) for Python! (My first library)
 Home-page: https://github.com/GustavoSchip/ninjakiwi_api
 License: MIT
+Keywords: NinjaKiwi,API
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
+Maintainer: Gustavo Schip
+Maintainer-email: gustavoschip@proton.me
 Requires-Python: >=3.11,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.3 Summary: Skeleton
-project created by Python Project Wizard (ppw). Home-page: https://github.com/
-GustavoSchip/ninjakiwi_api License: MIT Author: Gustavo Schip Author-email:
-gustavoschip@proton.me Requires-Python: >=3.11,<4.0.0 Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Provides-Extra: dev Provides-Extra: doc Provides-
-Extra: test Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: asyncio
-(>=3.4.3,<4.0.0) Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
-Requires-Dist: flake8 (==4.0.1) ; extra == "test" Requires-Dist: flake8-
-docstrings (>=1.6.0,<2.0.0) ; extra == "test" Requires-Dist: isort (==5.10.1) ;
-extra == "test" Requires-Dist: livereload (>=2.6.3,<3.0.0) Requires-Dist: mike
-(>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ;
-extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.3.1,<0.4.0) ; extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc" Requires-
-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0) Requires-Dist: mkdocstrings
-(>=0.18.0,<0.19.0) ; extra == "doc" Requires-Dist: pip (>=22.0.3,<23.0.0) ;
-extra == "dev" Requires-Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev"
-Requires-Dist: pyreadline (>=2.1,<3.0) Requires-Dist: pytest (>=7.0.1,<8.0.0) ;
-extra == "test" Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra ==
-"test" Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test" Requires-
-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tornado
-(>=6.2,<7.0) Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev" Requires-
-Dist: twine (>=3.8.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
-(>=20.13.1,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown #
-NinjaKiwi API
+Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.4 Summary: NinjaKiwi API
+(OpenDATA) for Python! (My first library) Home-page: https://github.com/
+GustavoSchip/ninjakiwi_api License: MIT Keywords: NinjaKiwi,API Author: Gustavo
+Schip Author-email: gustavoschip@proton.me Maintainer: Gustavo Schip
+Maintainer-email: gustavoschip@proton.me Requires-Python: >=3.11,<4.0.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: dev
+Provides-Extra: doc Provides-Extra: test Requires-Dist: aiohttp
+(>=3.8.1,<4.0.0) Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: black
+(>=22.3.0,<23.0.0) ; extra == "test" Requires-Dist: flake8 (==4.0.1) ; extra ==
+"test" Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: isort (==5.10.1) ; extra == "test" Requires-Dist: livereload
+(>=2.6.3,<3.0.0) Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-
+autorefs (>=0.3.1,<0.4.0) ; extra == "doc" Requires-Dist: mkdocs-include-
+markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc" Requires-Dist: mkdocs-
+material (>=8.1.11,<9.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-
+extensions (>=1.0.3,<2.0.0) Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ;
+extra == "doc" Requires-Dist: pip (>=22.0.3,<23.0.0) ; extra == "dev" Requires-
+Dist: pre-commit (>=2.17.0,<3.0.0) ; extra == "dev" Requires-Dist: pyreadline
+(>=2.1,<3.0) Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test" Requires-
+Dist: pytest-asyncio (>=0.21.1,<0.22.0) ; extra == "test" Requires-Dist:
+pytest-cov (>=3.0.0,<4.0.0) ; extra == "test" Requires-Dist: toml
+(>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tornado (>=6.2,<7.0)
+Requires-Dist: tox (>=3.24.5,<4.0.0) ; extra == "dev" Requires-Dist: twine
+(>=3.8.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv (>=20.13.1,<21.0.0)
+; extra == "dev" Description-Content-Type: text/markdown # NinjaKiwi API
                                [Release_Status]
 # Coming soon.. Stay tuned guys
```

