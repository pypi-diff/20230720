# Comparing `tmp/richset-0.1.8.tar.gz` & `tmp/richset-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richset-0.1.8.tar", last modified: Sat Jan 21 17:35:19 2023, max compression
+gzip compressed data, was "richset-0.1.9.tar", last modified: Thu Jul 20 14:40:06 2023, max compression
```

## Comparing `richset-0.1.8.tar` & `richset-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.978866 richset-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-21 17:34:44.000000 richset-0.1.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-21 17:34:44.000000 richset-0.1.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.974866 richset-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.974866 richset-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-21 17:34:44.000000 richset-0.1.8/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-21 17:34:44.000000 richset-0.1.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-01-21 17:34:44.000000 richset-0.1.8/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-01-21 17:34:44.000000 richset-0.1.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-01-21 17:34:44.000000 richset-0.1.8/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-21 17:34:44.000000 richset-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-01-21 17:35:19.978866 richset-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-01-21 17:34:44.000000 richset-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    38634 2023-01-21 17:34:44.000000 richset-0.1.8/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-01-21 17:34:44.000000 richset-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-21 17:34:44.000000 richset-0.1.8/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.974866 richset-0.1.8/richset/
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-01-21 17:34:44.000000 richset-0.1.8/richset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-21 17:35:19.000000 richset-0.1.8/richset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-21 17:34:44.000000 richset-0.1.8/richset/comparable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 17:34:44.000000 richset-0.1.8/richset/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.974866 richset-0.1.8/richset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-01-21 17:35:19.000000 richset-0.1.8/richset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-01-21 17:35:19.000000 richset-0.1.8/richset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 17:35:19.000000 richset-0.1.8/richset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-21 17:35:19.000000 richset-0.1.8/richset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-21 17:35:19.978866 richset-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 17:35:19.978866 richset-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-21 17:34:44.000000 richset-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_factory_classmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_list_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_list_functional_manipulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_list_manipulations.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_magic_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_paging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_set_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_sortings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-21 17:34:44.000000 richset-0.1.8/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.246152 richset-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 14:39:40.000000 richset-0.1.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 14:39:40.000000 richset-0.1.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.234152 richset-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 14:39:40.000000 richset-0.1.9/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.238152 richset-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 14:39:40.000000 richset-0.1.9/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:39:40.000000 richset-0.1.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-20 14:39:40.000000 richset-0.1.9/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 14:39:40.000000 richset-0.1.9/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-20 14:39:40.000000 richset-0.1.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-20 14:39:40.000000 richset-0.1.9/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 14:39:40.000000 richset-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-20 14:40:06.246152 richset-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-07-20 14:39:40.000000 richset-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-07-20 14:39:40.000000 richset-0.1.9/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 14:39:40.000000 richset-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.238152 richset-0.1.9/richset/
+-rw-r--r--   0 runner    (1001) docker     (123)    17990 2023-07-20 14:39:40.000000 richset-0.1.9/richset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:40:06.000000 richset-0.1.9/richset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 14:39:40.000000 richset-0.1.9/richset/comparable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:40.000000 richset-0.1.9/richset/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.238152 richset-0.1.9/richset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-20 14:40:06.000000 richset-0.1.9/richset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-20 14:40:06.000000 richset-0.1.9/richset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:40:06.000000 richset-0.1.9/richset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 14:40:06.000000 richset-0.1.9/richset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-20 14:40:06.246152 richset-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:40:06.246152 richset-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:39:40.000000 richset-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_factory_classmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_list_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_list_functional_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_list_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_magic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_paging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-20 14:39:40.000000 richset-0.1.9/tests/test_statistics.py
```

### Comparing `richset-0.1.8/.github/workflows/pypi-publish.yml` & `richset-0.1.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/.github/workflows/python-test.yml` & `richset-0.1.9/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/.gitignore` & `richset-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/LICENSE` & `richset-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/PKG-INFO` & `richset-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richset
-Version: 0.1.8
+Version: 0.1.9
 Summary: richset interpolate between list, dict, set and iterables.
 Home-page: https://github.com/kitsuyui/python-richset
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `richset-0.1.8/README.md` & `richset-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/poetry.lock` & `richset-0.1.9/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,51 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
-
-[[package]]
-name = "attrs"
-version = "22.2.0"
-description = "Classes Without Boilerplate"
-category = "dev"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
-    {file = "attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
-]
-
-[package.extras]
-cov = ["attrs[tests]", "coverage-enable-subprocess", "coverage[toml] (>=5.3)"]
-dev = ["attrs[docs,tests]"]
-docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope.interface"]
-tests = ["attrs[tests-no-zope]", "zope.interface"]
-tests-no-zope = ["cloudpickle", "cloudpickle", "hypothesis", "hypothesis", "mypy (>=0.971,<0.990)", "mypy (>=0.971,<0.990)", "pympler", "pympler", "pytest (>=4.3.0)", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-mypy-plugins", "pytest-xdist[psutil]", "pytest-xdist[psutil]"]
+# This file is automatically @generated by Poetry 1.4.2 and should not be changed by hand.
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "23.3.0"
 description = "The uncompromising code formatter."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
-    {file = "black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
-    {file = "black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
-    {file = "black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
-    {file = "black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
-    {file = "black-22.12.0-cp37-cp37m-win_amd64.whl", hash = "sha256:1f58cbe16dfe8c12b7434e50ff889fa479072096d79f0a7f25e4ab8e94cd8350"},
-    {file = "black-22.12.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77d86c9f3db9b1bf6761244bc0b3572a546f5fe37917a044e02f3166d5aafa7d"},
-    {file = "black-22.12.0-cp38-cp38-win_amd64.whl", hash = "sha256:82d9fe8fee3401e02e79767016b4907820a7dc28d70d137eb397b92ef3cc5bfc"},
-    {file = "black-22.12.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101c69b23df9b44247bd88e1d7e90154336ac4992502d4197bdac35dd7ee3320"},
-    {file = "black-22.12.0-cp39-cp39-win_amd64.whl", hash = "sha256:559c7a1ba9a006226f09e4916060982fd27334ae1998e7a38b3f33a37f7a2148"},
-    {file = "black-22.12.0-py3-none-any.whl", hash = "sha256:436cc9167dd28040ad90d3b404aec22cedf24a6e4d7de221bec2730ec0c97bcf"},
-    {file = "black-22.12.0.tar.gz", hash = "sha256:229351e5a18ca30f447bf724d007f890f97e13af070bb6ad4c0a441cd7596a2f"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
+    {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
+    {file = "black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d"},
+    {file = "black-23.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70"},
+    {file = "black-23.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326"},
+    {file = "black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
+    {file = "black-23.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2"},
+    {file = "black-23.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
+    {file = "black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
+    {file = "black-23.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266"},
+    {file = "black-23.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab"},
+    {file = "black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
+    {file = "black-23.3.0-py3-none-any.whl", hash = "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4"},
+    {file = "black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
+packaging = ">=22.0"
 pathspec = ">=0.9.0"
 platformdirs = ">=2"
-tomli = {version = ">=1.1.0", markers = "python_full_version < \"3.11.0a7\""}
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typed-ast = {version = ">=1.4.2", markers = "python_version < \"3.8\" and implementation_name == \"cpython\""}
 typing-extensions = {version = ">=3.10.0.0", markers = "python_version < \"3.10\""}
 
 [package.extras]
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
@@ -107,89 +102,89 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.0.5"
+version = "7.2.2"
 description = "Code coverage measurement for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "coverage-7.0.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b"},
-    {file = "coverage-7.0.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89"},
-    {file = "coverage-7.0.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40"},
-    {file = "coverage-7.0.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2"},
-    {file = "coverage-7.0.5-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289"},
-    {file = "coverage-7.0.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0"},
-    {file = "coverage-7.0.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8"},
-    {file = "coverage-7.0.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809"},
-    {file = "coverage-7.0.5-cp310-cp310-win32.whl", hash = "sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21"},
-    {file = "coverage-7.0.5-cp310-cp310-win_amd64.whl", hash = "sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad"},
-    {file = "coverage-7.0.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca"},
-    {file = "coverage-7.0.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0"},
-    {file = "coverage-7.0.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196"},
-    {file = "coverage-7.0.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0"},
-    {file = "coverage-7.0.5-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc"},
-    {file = "coverage-7.0.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45"},
-    {file = "coverage-7.0.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757"},
-    {file = "coverage-7.0.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095"},
-    {file = "coverage-7.0.5-cp311-cp311-win32.whl", hash = "sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831"},
-    {file = "coverage-7.0.5-cp311-cp311-win_amd64.whl", hash = "sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea"},
-    {file = "coverage-7.0.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c"},
-    {file = "coverage-7.0.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7"},
-    {file = "coverage-7.0.5-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96"},
-    {file = "coverage-7.0.5-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029"},
-    {file = "coverage-7.0.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3"},
-    {file = "coverage-7.0.5-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2"},
-    {file = "coverage-7.0.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47"},
-    {file = "coverage-7.0.5-cp37-cp37m-win32.whl", hash = "sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882"},
-    {file = "coverage-7.0.5-cp37-cp37m-win_amd64.whl", hash = "sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d"},
-    {file = "coverage-7.0.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb"},
-    {file = "coverage-7.0.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6"},
-    {file = "coverage-7.0.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd"},
-    {file = "coverage-7.0.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a"},
-    {file = "coverage-7.0.5-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2"},
-    {file = "coverage-7.0.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7"},
-    {file = "coverage-7.0.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0"},
-    {file = "coverage-7.0.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499"},
-    {file = "coverage-7.0.5-cp38-cp38-win32.whl", hash = "sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16"},
-    {file = "coverage-7.0.5-cp38-cp38-win_amd64.whl", hash = "sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af"},
-    {file = "coverage-7.0.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab"},
-    {file = "coverage-7.0.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637"},
-    {file = "coverage-7.0.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4"},
-    {file = "coverage-7.0.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded"},
-    {file = "coverage-7.0.5-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b"},
-    {file = "coverage-7.0.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209"},
-    {file = "coverage-7.0.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78"},
-    {file = "coverage-7.0.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1"},
-    {file = "coverage-7.0.5-cp39-cp39-win32.whl", hash = "sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904"},
-    {file = "coverage-7.0.5-cp39-cp39-win_amd64.whl", hash = "sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f"},
-    {file = "coverage-7.0.5-pp37.pp38.pp39-none-any.whl", hash = "sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0"},
-    {file = "coverage-7.0.5.tar.gz", hash = "sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45"},
+    {file = "coverage-7.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7"},
+    {file = "coverage-7.2.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d"},
+    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5"},
+    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"},
+    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6"},
+    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137"},
+    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90"},
+    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2"},
+    {file = "coverage-7.2.2-cp310-cp310-win32.whl", hash = "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292"},
+    {file = "coverage-7.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab"},
+    {file = "coverage-7.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b"},
+    {file = "coverage-7.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5"},
+    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731"},
+    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd"},
+    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d"},
+    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212"},
+    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54"},
+    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57"},
+    {file = "coverage-7.2.2-cp311-cp311-win32.whl", hash = "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d"},
+    {file = "coverage-7.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512"},
+    {file = "coverage-7.2.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9"},
+    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e"},
+    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69"},
+    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0"},
+    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f"},
+    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67"},
+    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9"},
+    {file = "coverage-7.2.2-cp37-cp37m-win32.whl", hash = "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8"},
+    {file = "coverage-7.2.2-cp37-cp37m-win_amd64.whl", hash = "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25"},
+    {file = "coverage-7.2.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6"},
+    {file = "coverage-7.2.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5"},
+    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4"},
+    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd"},
+    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84"},
+    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540"},
+    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88"},
+    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2"},
+    {file = "coverage-7.2.2-cp38-cp38-win32.whl", hash = "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3"},
+    {file = "coverage-7.2.2-cp38-cp38-win_amd64.whl", hash = "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8"},
+    {file = "coverage-7.2.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d"},
+    {file = "coverage-7.2.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005"},
+    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988"},
+    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149"},
+    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8"},
+    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140"},
+    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016"},
+    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be"},
+    {file = "coverage-7.2.2-cp39-cp39-win32.whl", hash = "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc"},
+    {file = "coverage-7.2.2-cp39-cp39-win_amd64.whl", hash = "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef"},
+    {file = "coverage-7.2.2-pp37.pp38.pp39-none-any.whl", hash = "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968"},
+    {file = "coverage-7.2.2.tar.gz", hash = "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2"},
 ]
 
 [package.dependencies]
 tomli = {version = "*", optional = true, markers = "python_full_version <= \"3.11.0a6\" and extra == \"toml\""}
 
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.0"
+version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.1.0-py3-none-any.whl", hash = "sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e"},
-    {file = "exceptiongroup-1.1.0.tar.gz", hash = "sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23"},
+    {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
+    {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "flake8"
@@ -239,27 +234,27 @@
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "isort"
-version = "5.11.4"
+version = "5.11.5"
 description = "A Python utility / library to sort Python imports."
 category = "dev"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "isort-5.11.4-py3-none-any.whl", hash = "sha256:c033fd0edb91000a7f09527fe5c75321878f98322a77ddcc81adbd83724afb7b"},
-    {file = "isort-5.11.4.tar.gz", hash = "sha256:6db30c5ded9815d813932c04c2f85a360bcdd35fed496f4d8f35495ef0a261b6"},
+    {file = "isort-5.11.5-py3-none-any.whl", hash = "sha256:ba1d72fb2595a01c7895a5128f9585a5cc4b6d395f1c8d514989b9a7eb2a8746"},
+    {file = "isort-5.11.5.tar.gz", hash = "sha256:6be1f76a507cb2ecf16c7cf14a37e41609ca082330be4e3436a18ef74add55db"},
 ]
 
 [package.extras]
 colors = ["colorama (>=0.4.3,<0.5.0)"]
-pipfile-deprecated-finder = ["pipreqs", "requirementslib"]
+pipfile-deprecated-finder = ["pip-shims (>=0.5.2)", "pipreqs", "requirementslib"]
 plugins = ["setuptools"]
 requirements-deprecated-finder = ["pip-api", "pipreqs"]
 
 [[package]]
 name = "mccabe"
 version = "0.7.0"
 description = "McCabe checker, plugin for flake8"
@@ -269,74 +264,70 @@
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "mypy"
-version = "0.991"
+version = "1.4.1"
 description = "Optional static typing for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "mypy-0.991-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab"},
-    {file = "mypy-0.991-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0714258640194d75677e86c786e80ccf294972cc76885d3ebbb560f11db0003d"},
-    {file = "mypy-0.991-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0c8f3be99e8a8bd403caa8c03be619544bc2c77a7093685dcf308c6b109426c6"},
-    {file = "mypy-0.991-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bc9ec663ed6c8f15f4ae9d3c04c989b744436c16d26580eaa760ae9dd5d662eb"},
-    {file = "mypy-0.991-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4307270436fd7694b41f913eb09210faff27ea4979ecbcd849e57d2da2f65305"},
-    {file = "mypy-0.991-cp310-cp310-win_amd64.whl", hash = "sha256:901c2c269c616e6cb0998b33d4adbb4a6af0ac4ce5cd078afd7bc95830e62c1c"},
-    {file = "mypy-0.991-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:d13674f3fb73805ba0c45eb6c0c3053d218aa1f7abead6e446d474529aafc372"},
-    {file = "mypy-0.991-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:1c8cd4fb70e8584ca1ed5805cbc7c017a3d1a29fb450621089ffed3e99d1857f"},
-    {file = "mypy-0.991-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:209ee89fbb0deed518605edddd234af80506aec932ad28d73c08f1400ef80a33"},
-    {file = "mypy-0.991-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:37bd02ebf9d10e05b00d71302d2c2e6ca333e6c2a8584a98c00e038db8121f05"},
-    {file = "mypy-0.991-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:26efb2fcc6b67e4d5a55561f39176821d2adf88f2745ddc72751b7890f3194ad"},
-    {file = "mypy-0.991-cp311-cp311-win_amd64.whl", hash = "sha256:3a700330b567114b673cf8ee7388e949f843b356a73b5ab22dd7cff4742a5297"},
-    {file = "mypy-0.991-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:1f7d1a520373e2272b10796c3ff721ea1a0712288cafaa95931e66aa15798813"},
-    {file = "mypy-0.991-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:641411733b127c3e0dab94c45af15fea99e4468f99ac88b39efb1ad677da5711"},
-    {file = "mypy-0.991-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3d80e36b7d7a9259b740be6d8d906221789b0d836201af4234093cae89ced0cd"},
-    {file = "mypy-0.991-cp37-cp37m-win_amd64.whl", hash = "sha256:e62ebaad93be3ad1a828a11e90f0e76f15449371ffeecca4a0a0b9adc99abcef"},
-    {file = "mypy-0.991-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:b86ce2c1866a748c0f6faca5232059f881cda6dda2a893b9a8373353cfe3715a"},
-    {file = "mypy-0.991-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ac6e503823143464538efda0e8e356d871557ef60ccd38f8824a4257acc18d93"},
-    {file = "mypy-0.991-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:0cca5adf694af539aeaa6ac633a7afe9bbd760df9d31be55ab780b77ab5ae8bf"},
-    {file = "mypy-0.991-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a12c56bf73cdab116df96e4ff39610b92a348cc99a1307e1da3c3768bbb5b135"},
-    {file = "mypy-0.991-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:652b651d42f155033a1967739788c436491b577b6a44e4c39fb340d0ee7f0d70"},
-    {file = "mypy-0.991-cp38-cp38-win_amd64.whl", hash = "sha256:4175593dc25d9da12f7de8de873a33f9b2b8bdb4e827a7cae952e5b1a342e243"},
-    {file = "mypy-0.991-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:98e781cd35c0acf33eb0295e8b9c55cdbef64fcb35f6d3aa2186f289bed6e80d"},
-    {file = "mypy-0.991-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6d7464bac72a85cb3491c7e92b5b62f3dcccb8af26826257760a552a5e244aa5"},
-    {file = "mypy-0.991-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:c9166b3f81a10cdf9b49f2d594b21b31adadb3d5e9db9b834866c3258b695be3"},
-    {file = "mypy-0.991-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b8472f736a5bfb159a5e36740847808f6f5b659960115ff29c7cecec1741c648"},
-    {file = "mypy-0.991-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5e80e758243b97b618cdf22004beb09e8a2de1af481382e4d84bc52152d1c476"},
-    {file = "mypy-0.991-cp39-cp39-win_amd64.whl", hash = "sha256:74e259b5c19f70d35fcc1ad3d56499065c601dfe94ff67ae48b85596b9ec1461"},
-    {file = "mypy-0.991-py3-none-any.whl", hash = "sha256:de32edc9b0a7e67c2775e574cb061a537660e51210fbf6006b0b36ea695ae9bb"},
-    {file = "mypy-0.991.tar.gz", hash = "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06"},
+    {file = "mypy-1.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8"},
+    {file = "mypy-1.4.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878"},
+    {file = "mypy-1.4.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd"},
+    {file = "mypy-1.4.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc"},
+    {file = "mypy-1.4.1-cp310-cp310-win_amd64.whl", hash = "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258"},
+    {file = "mypy-1.4.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2"},
+    {file = "mypy-1.4.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7"},
+    {file = "mypy-1.4.1-cp311-cp311-win_amd64.whl", hash = "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01"},
+    {file = "mypy-1.4.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b"},
+    {file = "mypy-1.4.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"},
+    {file = "mypy-1.4.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7"},
+    {file = "mypy-1.4.1-cp37-cp37m-win_amd64.whl", hash = "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3"},
+    {file = "mypy-1.4.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6"},
+    {file = "mypy-1.4.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f"},
+    {file = "mypy-1.4.1-cp38-cp38-win_amd64.whl", hash = "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3"},
+    {file = "mypy-1.4.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816"},
+    {file = "mypy-1.4.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c"},
+    {file = "mypy-1.4.1-cp39-cp39-win_amd64.whl", hash = "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f"},
+    {file = "mypy-1.4.1-py3-none-any.whl", hash = "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4"},
+    {file = "mypy-1.4.1.tar.gz", hash = "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b"},
 ]
 
 [package.dependencies]
-mypy-extensions = ">=0.4.3"
+mypy-extensions = ">=1.0.0"
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typed-ast = {version = ">=1.4.0,<2", markers = "python_version < \"3.8\""}
-typing-extensions = ">=3.10"
+typing-extensions = ">=4.1.0"
 
 [package.extras]
 dmypy = ["psutil (>=4.0)"]
 install-types = ["pip"]
 python2 = ["typed-ast (>=1.4.0,<2)"]
 reports = ["lxml"]
 
 [[package]]
 name = "mypy-extensions"
-version = "0.4.3"
-description = "Experimental type system extensions for programs checked with the mypy typechecker."
+version = "1.0.0"
+description = "Type system extensions for programs checked with the mypy type checker."
 category = "dev"
 optional = false
-python-versions = "*"
+python-versions = ">=3.5"
 files = [
-    {file = "mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
-    {file = "mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
+    {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
+    {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
 version = "23.0"
 description = "Core utilities for Python packages"
 category = "dev"
@@ -357,42 +348,42 @@
 files = [
     {file = "pastel-0.2.1-py2.py3-none-any.whl", hash = "sha256:4349225fcdf6c2bb34d483e523475de5bb04a5c10ef711263452cb37d7dd4364"},
     {file = "pastel-0.2.1.tar.gz", hash = "sha256:e6581ac04e973cac858828c6202c1e1e81fee1dc7de7683f3e1ffe0bfd8a573d"},
 ]
 
 [[package]]
 name = "pathspec"
-version = "0.10.3"
+version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pathspec-0.10.3-py3-none-any.whl", hash = "sha256:3c95343af8b756205e2aba76e843ba9520a24dd84f68c22b9f93251507509dd6"},
-    {file = "pathspec-0.10.3.tar.gz", hash = "sha256:56200de4077d9d0791465aa9095a01d421861e405b5096955051deefd697d6f6"},
+    {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
+    {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "2.6.2"
+version = "3.2.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-2.6.2-py3-none-any.whl", hash = "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490"},
-    {file = "platformdirs-2.6.2.tar.gz", hash = "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"},
+    {file = "platformdirs-3.2.0-py3-none-any.whl", hash = "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"},
+    {file = "platformdirs-3.2.0.tar.gz", hash = "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08"},
 ]
 
 [package.dependencies]
-typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
+typing-extensions = {version = ">=4.5", markers = "python_version < \"3.8\""}
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 description = "plugin and hook calling mechanisms for python"
 category = "dev"
 optional = false
@@ -407,22 +398,22 @@
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "poethepoet"
-version = "0.18.1"
+version = "0.19.0"
 description = "A task runner that works well with poetry."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "poethepoet-0.18.1-py3-none-any.whl", hash = "sha256:e85727bf6f4a10bf6c1a43026bdeb40df689bea3c4682d03cbe531cabc8f2ba6"},
-    {file = "poethepoet-0.18.1.tar.gz", hash = "sha256:5f3566b14c2f5dccdfbc3bb26f0096006b38dc0b9c74bd4f8dd1eba7b0e29f6a"},
+    {file = "poethepoet-0.19.0-py3-none-any.whl", hash = "sha256:87038be589077e4b407050a9da644d9cd9e4076ccfc8abc7f855cf6870d5c6c2"},
+    {file = "poethepoet-0.19.0.tar.gz", hash = "sha256:897eb85ec15876d79befc7d19d4c80ce7c8b214d1bb0dcfec640abd81616bfed"},
 ]
 
 [package.dependencies]
 pastel = ">=0.2.1,<0.3.0"
 tomli = ">=1.2.2"
 
 [package.extras]
@@ -465,81 +456,80 @@
 ]
 
 [package.dependencies]
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 
 [[package]]
 name = "pytest"
-version = "7.2.1"
+version = "7.4.0"
 description = "pytest: simple powerful testing with Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pytest-7.2.1-py3-none-any.whl", hash = "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5"},
-    {file = "pytest-7.2.1.tar.gz", hash = "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"},
+    {file = "pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {file = "pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 
 [package.dependencies]
-attrs = ">=19.2.0"
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 importlib-metadata = {version = ">=0.12", markers = "python_version < \"3.8\""}
 iniconfig = "*"
 packaging = "*"
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "pytest-cov"
-version = "4.0.0"
+version = "4.1.0"
 description = "Pytest plugin for measuring coverage."
 category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "pytest-cov-4.0.0.tar.gz", hash = "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"},
-    {file = "pytest_cov-4.0.0-py3-none-any.whl", hash = "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b"},
+    {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
+    {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
 ]
 
 [package.dependencies]
 coverage = {version = ">=5.2.1", extras = ["toml"]}
 pytest = ">=4.6"
 
 [package.extras]
 testing = ["fields", "hunter", "process-tests", "pytest-xdist", "six", "virtualenv"]
 
 [[package]]
 name = "pyupgrade"
-version = "3.3.1"
+version = "3.3.2"
 description = "A tool to automatically upgrade syntax for newer versions."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pyupgrade-3.3.1-py2.py3-none-any.whl", hash = "sha256:3b93641963df022d605c78aeae4b5956a5296ea24701eafaef9c487527b77e60"},
-    {file = "pyupgrade-3.3.1.tar.gz", hash = "sha256:f88bce38b0ba92c2a9a5063c8629e456e8d919b67d2d42c7ecab82ff196f9813"},
+    {file = "pyupgrade-3.3.2-py2.py3-none-any.whl", hash = "sha256:c05b82c911934b3a638b29f48f48dc6e0ef6c57c55ec36f2b41ae9dbf6711b4b"},
+    {file = "pyupgrade-3.3.2.tar.gz", hash = "sha256:bcfed63d38811809f179fd269dec246680b0aaa5bbe662b535826e5fa2275219"},
 ]
 
 [package.dependencies]
 tokenize-rt = ">=3.2.0"
 
 [[package]]
 name = "setuptools"
-version = "66.1.1"
+version = "67.6.0"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "setuptools-66.1.1-py3-none-any.whl", hash = "sha256:6f590d76b713d5de4e49fe4fbca24474469f53c83632d5d0fd056f7ff7e8112b"},
-    {file = "setuptools-66.1.1.tar.gz", hash = "sha256:ac4008d396bc9cd983ea483cb7139c0240a07bbc74ffb6232fceffedc6cf03a8"},
+    {file = "setuptools-67.6.0-py3-none-any.whl", hash = "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"},
+    {file = "setuptools-67.6.0.tar.gz", hash = "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
 testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
@@ -622,37 +612,37 @@
     {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
     {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
     {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.5.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {file = "typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
+    {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
+    {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.11.0"
+version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "zipp-3.11.0-py3-none-any.whl", hash = "sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa"},
-    {file = "zipp-3.11.0.tar.gz", hash = "sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766"},
+    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
+    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
 [package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)"]
-testing = ["flake8 (<5)", "func-timeout", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
 content-hash = "1a3ce0f1e3289d04275cb3cffe4c988c32330f23bf2c3fa5475ef4bd37ba6b5c"
```

### Comparing `richset-0.1.8/pyproject.toml` & `richset-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/richset/__init__.py` & `richset-0.1.9/richset/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeVar,
     overload,
 )
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
-    from typing_extensions import Literal
+    from typing_extensions import Literal  # pragma: no cover
 
 from .comparable import Comparable
 
 T = TypeVar("T")
 S = TypeVar("S")
 Key = TypeVar("Key", bound=Hashable)
 Fill = TypeVar("Fill")
@@ -458,15 +458,15 @@
                     )
                 )
             )
         return RichSet.from_list(
             list(itertools.zip_longest(self.records, other.records))
         )
 
-    # sortings
+    # sorting
 
     def sorted(
         self,
         *,
         key: Callable[[T], Comparable],
         reverse: bool = False,
     ) -> RichSet[T]:
```

### Comparing `richset-0.1.8/richset/comparable.py` & `richset-0.1.9/richset/comparable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
-    from typing_extensions import Protocol
+    from typing_extensions import Protocol  # pragma: no cover
 
 from typing import TypeVar, Union
 
 T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class SupportsDunderLT(Protocol[T_contra]):  # pragma: no cover
```

### Comparing `richset-0.1.8/richset.egg-info/PKG-INFO` & `richset-0.1.9/richset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richset
-Version: 0.1.8
+Version: 0.1.9
 Summary: richset interpolate between list, dict, set and iterables.
 Home-page: https://github.com/kitsuyui/python-richset
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `richset-0.1.8/richset.egg-info/SOURCES.txt` & `richset-0.1.9/richset.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 .editorconfig
 .gitignore
 .gitignore.in
 LICENSE
 README.md
 poetry.lock
 pyproject.toml
-renovate.json
 setup.cfg
+.github/renovate.json5
 .github/workflows/happy.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/python-test.yml
+.github/workflows/spellcheck.yml
 richset/__init__.py
 richset/_version.py
 richset/comparable.py
 richset/py.typed
 richset.egg-info/PKG-INFO
 richset.egg-info/SOURCES.txt
 richset.egg-info/dependency_links.txt
@@ -26,9 +27,9 @@
 tests/test_list_accessors.py
 tests/test_list_functional_manipulations.py
 tests/test_list_manipulations.py
 tests/test_magic_methods.py
 tests/test_paging.py
 tests/test_search.py
 tests/test_set_operations.py
-tests/test_sortings.py
+tests/test_sorting.py
 tests/test_statistics.py
```

### Comparing `richset-0.1.8/setup.cfg` & `richset-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_conversions.py` & `richset-0.1.9/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_grouping.py` & `richset-0.1.9/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_list_accessors.py` & `richset-0.1.9/tests/test_list_accessors.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_list_functional_manipulations.py` & `richset-0.1.9/tests/test_list_functional_manipulations.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_list_manipulations.py` & `richset-0.1.9/tests/test_list_manipulations.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_magic_methods.py` & `richset-0.1.9/tests/test_magic_methods.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_paging.py` & `richset-0.1.9/tests/test_paging.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_search.py` & `richset-0.1.9/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_set_operations.py` & `richset-0.1.9/tests/test_set_operations.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_sortings.py` & `richset-0.1.9/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `richset-0.1.8/tests/test_statistics.py` & `richset-0.1.9/tests/test_statistics.py`

 * *Files identical despite different names*

