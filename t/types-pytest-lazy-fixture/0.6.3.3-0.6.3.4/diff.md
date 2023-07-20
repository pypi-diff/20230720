# Comparing `tmp/types-pytest-lazy-fixture-0.6.3.3.tar.gz` & `tmp/types-pytest-lazy-fixture-0.6.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pytest-lazy-fixture-0.6.3.3.tar", last modified: Tue Feb 21 01:28:02 2023, max compression
+gzip compressed data, was "types-pytest-lazy-fixture-0.6.3.4.tar", last modified: Thu Jul 20 15:19:20 2023, max compression
```

## Comparing `types-pytest-lazy-fixture-0.6.3.3.tar` & `types-pytest-lazy-fixture-0.6.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:02.469864 types-pytest-lazy-fixture-0.6.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-21 01:28:01.000000 types-pytest-lazy-fixture-0.6.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:28:01.000000 types-pytest-lazy-fixture-0.6.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-21 01:28:02.469864 types-pytest-lazy-fixture-0.6.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:02.469864 types-pytest-lazy-fixture-0.6.3.3/pytest_lazyfixture-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 01:28:01.000000 types-pytest-lazy-fixture-0.6.3.3/pytest_lazyfixture-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-21 01:28:01.000000 types-pytest-lazy-fixture-0.6.3.3/pytest_lazyfixture-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:28:02.473864 types-pytest-lazy-fixture-0.6.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-21 01:28:01.000000 types-pytest-lazy-fixture-0.6.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:02.469864 types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-21 01:28:02.000000 types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-21 01:28:02.000000 types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:28:02.000000 types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-21 01:28:02.000000 types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:20.755436 types-pytest-lazy-fixture-0.6.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 15:19:19.000000 types-pytest-lazy-fixture-0.6.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:19.000000 types-pytest-lazy-fixture-0.6.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-20 15:19:20.755436 types-pytest-lazy-fixture-0.6.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:20.751436 types-pytest-lazy-fixture-0.6.3.4/pytest_lazyfixture-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 15:19:19.000000 types-pytest-lazy-fixture-0.6.3.4/pytest_lazyfixture-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 15:19:19.000000 types-pytest-lazy-fixture-0.6.3.4/pytest_lazyfixture-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:20.755436 types-pytest-lazy-fixture-0.6.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-20 15:19:19.000000 types-pytest-lazy-fixture-0.6.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:20.755436 types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-20 15:19:20.000000 types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 15:19:20.000000 types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:20.000000 types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 15:19:20.000000 types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/top_level.txt
```

### Comparing `types-pytest-lazy-fixture-0.6.3.3/CHANGELOG.md` & `types-pytest-lazy-fixture-0.6.3.4/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.6.3.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.6.3.3 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 0.6.3.2 (2022-11-20)
```

### Comparing `types-pytest-lazy-fixture-0.6.3.3/PKG-INFO` & `types-pytest-lazy-fixture-0.6.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pytest-lazy-fixture
-Version: 0.6.3.3
+Version: 0.6.3.4
 Summary: Typing stubs for pytest-lazy-fixture
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytest-lazy-fixture.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pytest-lazy-fixture`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytest-lazy-fixture. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pytest-lazy-fixture-0.6.3.3/setup.py` & `types-pytest-lazy-fixture-0.6.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pytest-lazy-fixture`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytest-lazy-fixture. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.6.3.3",
+      version="0.6.3.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytest-lazy-fixture.md",
```

### Comparing `types-pytest-lazy-fixture-0.6.3.3/types_pytest_lazy_fixture.egg-info/PKG-INFO` & `types-pytest-lazy-fixture-0.6.3.4/types_pytest_lazy_fixture.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pytest-lazy-fixture
-Version: 0.6.3.3
+Version: 0.6.3.4
 Summary: Typing stubs for pytest-lazy-fixture
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytest-lazy-fixture.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pytest-lazy-fixture`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytest-lazy-fixture. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

