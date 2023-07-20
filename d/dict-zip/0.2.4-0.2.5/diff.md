# Comparing `tmp/dict_zip-0.2.4.tar.gz` & `tmp/dict_zip-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict_zip-0.2.4.tar", last modified: Mon Jan  9 11:17:18 2023, max compression
+gzip compressed data, was "dict_zip-0.2.5.tar", last modified: Thu Jul 20 14:39:13 2023, max compression
```

## Comparing `dict_zip-0.2.4.tar` & `dict_zip-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.575750 dict_zip-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-09 11:16:54.000000 dict_zip-0.2.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.567750 dict_zip-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.571750 dict_zip-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-09 11:16:54.000000 dict_zip-0.2.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-01-09 11:16:54.000000 dict_zip-0.2.4/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-09 11:16:54.000000 dict_zip-0.2.4/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-01-09 11:16:54.000000 dict_zip-0.2.4/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-09 11:16:54.000000 dict_zip-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-09 11:16:54.000000 dict_zip-0.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-09 11:17:18.575750 dict_zip-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-01-09 11:16:54.000000 dict_zip-0.2.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-01-09 11:16:54.000000 dict_zip-0.2.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-01-09 11:16:54.000000 dict_zip-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.571750 dict_zip-0.2.4/dict_zip/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-09 11:16:54.000000 dict_zip-0.2.4/dict_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-01-09 11:16:54.000000 dict_zip-0.2.4/dict_zip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-09 11:17:18.000000 dict_zip-0.2.4/dict_zip/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 11:16:54.000000 dict_zip-0.2.4/dict_zip/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.575750 dict_zip-0.2.4/dict_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-09 11:17:18.000000 dict_zip-0.2.4/dict_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-09 11:17:18.000000 dict_zip-0.2.4/dict_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 11:17:18.000000 dict_zip-0.2.4/dict_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-09 11:17:18.000000 dict_zip-0.2.4/dict_zip.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1421 2023-01-09 11:16:54.000000 dict_zip-0.2.4/generate_type_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-09 11:16:54.000000 dict_zip-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-09 11:16:54.000000 dict_zip-0.2.4/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.575750 dict_zip-0.2.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      387 2023-01-09 11:16:54.000000 dict_zip-0.2.4/scripts/test_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-09 11:17:18.575750 dict_zip-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 11:17:18.575750 dict_zip-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 11:16:54.000000 dict_zip-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-09 11:16:54.000000 dict_zip-0.2.4/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-09 11:16:54.000000 dict_zip-0.2.4/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-09 11:16:54.000000 dict_zip-0.2.4/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.185663 dict_zip-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.181663 dict_zip-0.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.181663 dict_zip-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-20 14:38:50.000000 dict_zip-0.2.5/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 14:38:50.000000 dict_zip-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-20 14:39:13.185663 dict_zip-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-20 14:38:50.000000 dict_zip-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.181663 dict_zip-0.2.5/dict_zip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-20 14:38:50.000000 dict_zip-0.2.5/dict_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-20 14:38:50.000000 dict_zip-0.2.5/dict_zip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:39:13.000000 dict_zip-0.2.5/dict_zip/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:38:50.000000 dict_zip-0.2.5/dict_zip/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.181663 dict_zip-0.2.5/dict_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-20 14:39:13.000000 dict_zip-0.2.5/dict_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-20 14:39:13.000000 dict_zip-0.2.5/dict_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:39:13.000000 dict_zip-0.2.5/dict_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 14:39:13.000000 dict_zip-0.2.5/dict_zip.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1421 2023-07-20 14:38:50.000000 dict_zip-0.2.5/generate_type_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42854 2023-07-20 14:38:50.000000 dict_zip-0.2.5/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:38:50.000000 dict_zip-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.181663 dict_zip-0.2.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      387 2023-07-20 14:38:50.000000 dict_zip-0.2.5/scripts/test_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-20 14:39:13.185663 dict_zip-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:13.185663 dict_zip-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:38:50.000000 dict_zip-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 14:38:50.000000 dict_zip-0.2.5/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 14:38:50.000000 dict_zip-0.2.5/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-20 14:38:50.000000 dict_zip-0.2.5/tests/test_types.py
```

### Comparing `dict_zip-0.2.4/.github/workflows/pypi-publish.yml` & `dict_zip-0.2.5/.github/workflows/pypi-publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,53 @@
-name: Upload PyPI package release
+name: Packaging
 
 on:
+  push:
   release:
     # "released" events are emitted either when directly be released or be edited from pre-released.
     types: [prereleased, released]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v4
+      - name: Set up Python
+        id: setup-python
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.x"
-          cache: "pipenv"
+          python-version: "3.11"
 
-      - run: pipx install pipenv
+      - name: Set up poetry
+        uses: abatilo/actions-poetry@v2
 
-      - run: pipenv sync --dev
+      - name: Cache
+        uses: actions/cache@v3
+        with:
+          path: ~/.cache/pypoetry/virtualenvs
+          key: ${{ runner.os }}-build-${{ matrix.python }}-${{ hashFiles('**/poetry.lock') }}
+          restore-keys: |
+            ${{ runner.os }}-build-${{ matrix.python }}-${{ hashFiles('**/poetry.lock') }}
+            ${{ runner.os }}-build-${{ matrix.python }}-
+            ${{ runner.os }}-
+
+      - run: poetry install
 
       - name: Build
-        run: |
-          pipenv run python3 -m build .
-          pipenv run python3 -m pip install dist/*.whl
+        # I use poetry just as a package manager, so this is not `poetry build`
+        run: poetry run poe build
 
       - name: Publish distribution to Test PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         if: github.event_name == 'release' && github.event.release.prerelease
         with:
           user: __token__
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
 
       - name: Publish distribution to PyPI
         if: github.event_name == 'release' && !github.event.release.prerelease
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `dict_zip-0.2.4/.gitignore` & `dict_zip-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/LICENSE` & `dict_zip-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/PKG-INFO` & `dict_zip-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict_zip
-Version: 0.2.4
+Version: 0.2.5
 Summary: zip and zip_longest for dict
 Home-page: https://github.com/kitsuyui/dict_zip
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dict_zip-0.2.4/README.md` & `dict_zip-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/dict_zip/__init__.py` & `dict_zip-0.2.5/dict_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/dict_zip/__init__.pyi` & `dict_zip-0.2.5/dict_zip/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,18 @@
 ) -> dict[_K, tuple[_T1 | _Fill]]: ...
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1], dict2: dict[_K, _T2]
 ) -> dict[_K, tuple[_T1 | None, _T2 | None]]: ...
 @overload
 def dict_zip_longest(
-    dict1: dict[_K, _T1], dict2: dict[_K, _T2], *, fillvalue: _Fill | None = None
+    dict1: dict[_K, _T1],
+    dict2: dict[_K, _T2],
+    *,
+    fillvalue: _Fill | None = None,
 ) -> dict[_K, tuple[_T1 | _Fill, _T2 | _Fill]]: ...
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1], dict2: dict[_K, _T2], dict3: dict[_K, _T3]
 ) -> dict[_K, tuple[_T1 | None, _T2 | None, _T3 | None]]: ...
 @overload
 def dict_zip_longest(
@@ -129,15 +132,17 @@
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1],
     dict2: dict[_K, _T2],
     dict3: dict[_K, _T3],
     dict4: dict[_K, _T4],
     dict5: dict[_K, _T5],
-) -> dict[_K, tuple[_T1 | None, _T2 | None, _T3 | None, _T4 | None, _T5 | None]]: ...
+) -> dict[
+    _K, tuple[_T1 | None, _T2 | None, _T3 | None, _T4 | None, _T5 | None]
+]: ...
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1],
     dict2: dict[_K, _T2],
     dict3: dict[_K, _T3],
     dict4: dict[_K, _T4],
     dict5: dict[_K, _T5],
@@ -151,29 +156,39 @@
     dict1: dict[_K, _T1],
     dict2: dict[_K, _T2],
     dict3: dict[_K, _T3],
     dict4: dict[_K, _T4],
     dict5: dict[_K, _T5],
     dict6: dict[_K, _T6],
 ) -> dict[
-    _K, tuple[_T1 | None, _T2 | None, _T3 | None, _T4 | None, _T5 | None, _T6 | None]
+    _K,
+    tuple[
+        _T1 | None, _T2 | None, _T3 | None, _T4 | None, _T5 | None, _T6 | None
+    ],
 ]: ...
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1],
     dict2: dict[_K, _T2],
     dict3: dict[_K, _T3],
     dict4: dict[_K, _T4],
     dict5: dict[_K, _T5],
     dict6: dict[_K, _T6],
     *,
     fillvalue: _Fill | None = None,
 ) -> dict[
     _K,
-    tuple[_T1 | _Fill, _T2 | _Fill, _T3 | _Fill, _T4 | _Fill, _T5 | _Fill, _T6 | _Fill],
+    tuple[
+        _T1 | _Fill,
+        _T2 | _Fill,
+        _T3 | _Fill,
+        _T4 | _Fill,
+        _T5 | _Fill,
+        _T6 | _Fill,
+    ],
 ]: ...
 @overload
 def dict_zip_longest(
     dict1: dict[_K, _T1],
     dict2: dict[_K, _T2],
     dict3: dict[_K, _T3],
     dict4: dict[_K, _T4],
```

### Comparing `dict_zip-0.2.4/dict_zip.egg-info/PKG-INFO` & `dict_zip-0.2.5/dict_zip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict-zip
-Version: 0.2.4
+Version: 0.2.5
 Summary: zip and zip_longest for dict
 Home-page: https://github.com/kitsuyui/dict_zip
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dict_zip-0.2.4/dict_zip.egg-info/SOURCES.txt` & `dict_zip-0.2.5/dict_zip.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .editorconfig
 .gitignore
 .gitignore.in
 LICENSE
-Makefile
-Pipfile
-Pipfile.lock
 README.md
 generate_type_stub.py
+poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
+.github/renovate.json5
+.github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 dict_zip/__init__.py
 dict_zip/__init__.pyi
 dict_zip/_version.py
 dict_zip/py.typed
 dict_zip.egg-info/PKG-INFO
 dict_zip.egg-info/SOURCES.txt
 dict_zip.egg-info/dependency_links.txt
```

### Comparing `dict_zip-0.2.4/generate_type_stub.py` & `dict_zip-0.2.5/generate_type_stub.py`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/setup.cfg` & `dict_zip-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/tests/test_basis.py` & `dict_zip-0.2.5/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `dict_zip-0.2.4/tests/test_types.py` & `dict_zip-0.2.5/tests/test_types.py`

 * *Files identical despite different names*

